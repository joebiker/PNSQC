# Setup Dice MCP Server

Follow directions at [dice.com](https://www.dice.com/career-advice/how-to-connect-the-dice-mcp-server-to-your-ai-assistant)

## Copilot CLI

I tried different combinations with Copilot CLI, but was unable to get it setup there. It complained about type 'SSE' and 'http' didn't work.

## Gemini CLI

when pasting JSON from the website directions, I was able to get it to work correctly.

My config file (c:\users\joe\\.gemini\settings.json)

```json
{
  "mcpServers": {
    "dice-job-search": {
      "url": "https://mcp.dice.com/mcp"
    },
    "AccuWeather-mcp": {
      "type": "stdio",
      "command": "npx",
      "args": [
        "-y",
        "@timlukahorstmann/mcp-weather"
      ],
      "env": {
        "ACCUWEATHER_API_KEY": "zpka_8d0282cff6c1458597f39ff1d8e7e016_43bba44b"
      }
    }
  },
  "security": {
    "auth": {
      "selectedType": "gemini-api-key"
    }
  },
  "ui": {
    "footer": {
      "hideModelInfo": false,
      "hideContextPercentage": false
    }
  }
}
```
