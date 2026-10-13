# Install Claude Code

If you don't already have it, here is a primer for install. These are based on Windows / Powershell.

## Installation Steps

Windows (PowerShell):
> powershell irm https://claude.ai/install.ps1 | iex

### Verify the installation

claude --version

### Configuration

User Global Settings

> ~/.claude.json

> ~/.claude/settings.json

Project Shared Settings

> <project_root>/.claude/settings.json

## Claude Desktop

Config for Connectors

> %APPDATA%\Claude\claude_desktop_config.json

Will allow NPX but only as manual configuration
