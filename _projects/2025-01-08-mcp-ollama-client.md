---
layout: default
title: "MCP‑Ollama Client"
year: 2025
stack: "Python • Ollama • MCP • CLI"
excerpt: "Offline chat client that merges tools from multiple Model‑Context‑Protocol servers into one local LLM."
tags: [MCP, Ollama, CLI, Tools]
image: assets/img/projects/mcp-ollama-client.png
---

{% if page.image %}
<figure>
  <img src="{{ page.image | relative_url }}" alt="{{ page.title }} screenshot" loading="lazy">
  <figcaption>{{ page.title }}</figcaption>
</figure>
{% endif %}

YOU CAN REPLICATE THIS PROJECT -> https://github.com/Nagharjun17/MCP-Ollama-Client

* Runs **entirely offline** on a local LLM via **Ollama** (default: `qwen3:14b`, but any function‑calling model works).
* Connects to **multiple MCP servers** at once (e.g., `postgres`, `filesystem`) declared in a single `config.json`.
* On startup: launches servers → fetches tool schemas → **prefixes tools** as `<server>.<tool>` → hands the merged set to the LLM.
* The model then decides **which server/tool to call** per user request.
* Everything is configurable in **one file**; add/remove servers without editing code.

### Requirements (tested)
- Python ≥ **3.12**
- Ollama ≥ **0.8.0**
- MCP servers with **stdio** transport (e.g., `postgres-mcp`, server‑filesystem)

### Quick start
```bash
# 1) clone
git clone https://github.com/Nagharjun17/MCP-Ollama-Client.git
cd mcp-ollama-client

# 2) env
uv venv && source .venv/bin/activate
uv pip sync pyproject.toml    # or: uv pip install -r uv.lock

# 3) local model
ollama pull qwen3:14b

# 4) config + servers (example)
uv pip install postgres-mcp    # and set DATABASE_URI etc. in config.json

# 5) run
uv run client.py
```
Example boot:
```
🔌 Starting MCP server: postgres
🔌 Starting MCP server: filesystem
🛠️  Aggregated tools: ['postgres.list_schemas', 'filesystem.read_file', ...]
>>>
MCP Client Startup
```
Type natural language queries; the LLM will call tools as needed.

### `config.json` (schema excerpt)
```json
{
  "llm": {
    "model": "qwen3:14b",
    "temperature": 0.7,
    "max_tokens": 2048
  },
  "mcpServers": {
    "postgres": {
      "command": "postgres-mcp",
      "args": ["--access-mode=restricted"],
      "env": {
        "DATABASE_URI": "postgresql://user:pass@localhost:5432/db"
      }
    },
    "filesystem": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-filesystem", "/mnt/smbshare/"]
    }
  }
}
```
* Keys under `mcpServers` become **prefixes** (`postgres.*`, `filesystem.*`).  
* Each server is launched as its own **stdio subprocess**.  
* **Local‑first**: no cloud keys required.

[GitHub Repo](https://github.com/Nagharjun17/MCP-Ollama-Client)

<div style="margin-top: 2rem;">
  <a href="/projects" style="text-decoration: none; font-weight: bold;">← Back to Projects</a>
</div>
