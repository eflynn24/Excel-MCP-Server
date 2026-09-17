# MCP Server + Local LLM (Ollama)

A local AI system that enables **LLMs to interact with Excel workbooks through the Model Context Protocol (MCP)**.

The project connects a locally hosted LLM through **Ollama** to Python-based Excel tools exposed through an MCP server, allowing natural-language requests to be translated into structured workbook operations.

## How It Works

```text
User Request
     ↓
Local LLM (Ollama)
     ↓
MCP Tool Call
     ↓
Python Excel Tools
     ↓
Excel Workbook
     ↓
Tool Result → LLM → User
```

The LLM handles request interpretation and tool selection, while Python performs the actual Excel operations.

## Architecture

<img width="1000" alt="MCP Server + Local LLM Architecture" src="https://github.com/user-attachments/assets/35ff84d6-5aa2-49e0-b79f-dd706bd912d5" />

<img width="1000" alt="MCP Excel Tool Flow" src="https://github.com/user-attachments/assets/759ee0e8-d2fe-4f17-9acd-239174f16d41" />

## Features

* 🧠 Local LLM inference with Ollama
* 🔌 Model Context Protocol (MCP) integration
* 📊 Excel workbook interaction
* 🐍 Python-based tool execution
* 🛠️ Structured tool calling
* 📖 Workbook and worksheet inspection
* 🔎 Excel data retrieval and analysis
* ✏️ Programmatic workbook operations
* 🔒 Local execution without cloud LLM APIs

## Technology Stack

* **Python** — application and tool implementation
* **Ollama** — local LLM runtime
* **MCP** — model-to-tool communication
* **OpenPyXL** — Excel workbook manipulation
* **Pandas** — data processing
* **Xlwings** — Excel integration

