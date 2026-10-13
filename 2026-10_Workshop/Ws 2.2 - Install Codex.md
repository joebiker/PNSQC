# Install AI

If you don't already have it, here is a primer for install. These are based on Windows / Powershell.

## Installation Steps

PowerShell

> powershell -ExecutionPolicy ByPass -c "irm https://chatgpt.com/codex/install.ps1 | iex"

Node.js (npm) Run: (requires Node.js 18+)

> npm install -g @openai/codex

### Verify the installation

You must open a new Terminal window after creating the environment variable above!!!

> codex --version

### Configuration

User (local computer) config:

> C:\Users\Joe\\.codex\config.toml

Workspace / Project-scoped: (loaded only when you mark the project as trusted)

> .codex/config.toml in the repository root

## ChatGPT App

Custom MCP Server. No option for NPX command
