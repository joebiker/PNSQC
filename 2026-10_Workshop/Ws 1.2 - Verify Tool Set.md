# Tool Verification

- Ensure Setup of Chrome
- VS Code
  - Extensions
  - Plugins
- Claude Code
- Codex
- Gemini CLI, free calls
  1. Job search `use mcp dice-job-search to find jobs in Portland, OR related to QA or software quality`
  2. Weather `using the AccuWeather-mcp get a forcast for Portland, OR for the next 3 days`
    - Fail AccuWeather API error (403): Request failed with status code 403
    - This typically means:
    - The AccuWeather API key configured for the MCP server is invalid, missing, or unauthorized.
    - The free tier request quota or specific endpoint permission for the API key has been exceeded or restricted.
  3. Rename files in this folder that start with Jam to Ws. ~\source\joebiker\PNSQC\2026-10_Workshop

## System Path

**Set the path for the current user, ie: Joe (super important)**

1. Open Environment Variables
1. User variables (top section)
1. Find Path, select it, then click Edit...
1. Copy the following path:
1. C:\Users\Joe\AppData\Roaming\npm\
1. On the Edit environment variable screen click New
1. Paste the path, click OK.

## CLI Version information

### Check  Codex

### Check Claude Code

### Check Gemini CLI is working

> gemini --version

0.25.0

### Check GitHub Copilot is working

> copilot --version

0.0.393

 ● Configured MCP servers: weather-national-service, playwrigt-mcp
 ● Loaded custom instructions: .github/copilot-instructions.md (769 chars)
 ● Copilot CLI version 1.0.95 downloaded. Restart to update.
