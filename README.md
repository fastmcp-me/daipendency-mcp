[![Add to Cursor](https://fastmcp.me/badges/cursor_dark.svg)](https://fastmcp.me/MCP/Details/1717/daipendency)
[![Add to VS Code](https://fastmcp.me/badges/vscode_dark.svg)](https://fastmcp.me/MCP/Details/1717/daipendency)
[![Add to Claude](https://fastmcp.me/badges/claude_dark.svg)](https://fastmcp.me/MCP/Details/1717/daipendency)
[![Add to ChatGPT](https://fastmcp.me/badges/chatgpt_dark.svg)](https://fastmcp.me/MCP/Details/1717/daipendency)
[![Add to Codex](https://fastmcp.me/badges/codex_dark.svg)](https://fastmcp.me/MCP/Details/1717/daipendency)
[![Add to Gemini](https://fastmcp.me/badges/gemini_dark.svg)](https://fastmcp.me/MCP/Details/1717/daipendency)

# Daipendency MCP Server

Model Context Protocol (MCP) server for [Daipendency](https://github.com/daipendency/daipendency).

## Install

Use `npx -y @daipendency/mcp` to run this MCP server with stdio.

## API

### Tools

#### `get_dependency_docs`

Extract narrative and API documentation for a dependency of a local project.

This is equivalent to [`daipendency extract-dep`](https://github.com/daipendency/daipendency#daipendency-extract-dep-extract-the-documentation-of-a-dependency).

## Architectural Decisions

Although Daipendency itself is implemented in Rust,
this project is implemented in TypeScript so that we could use one of the official, feature-rich MCP SDKs.
This required implementing [JS bindings for Daipendency](https://github.com/daipendency/daipendency-js).
