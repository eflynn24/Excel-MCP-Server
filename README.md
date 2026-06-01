## MCP Server + Local LLM (Ollama)
Run a local LLM with custom MCP servers to enable tool usage (files, APIs, automation) directly from your model.

This setup connects:
- A local LLM (Ollama)
- A custom MCP server

So your model can:
- Access external tools
- Read/write files
- Run custom automation workflows

MCP Server → exposes tools (functions)
MCP Client → connects those tools to the LLM
Ollama → runs the local model

The LLM can then call tools dynamically during responses.

## Steps to set up your own LLM with Custom MCP Server -
Install dependencies
pip install mcp-client-for-ollama
pip install mcp openpyxl pandas xlwings

Install Model
ollama pull qwen2.5:7b

Run MCP client
python -m mcp_client_for_ollama --servers-json "your path\servers.json"

## Example Use Cases -
- Query Excel
- Generate reports
- Automate workflows
