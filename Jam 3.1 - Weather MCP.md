# Jam 2026 - Our first MCP server: Weather

## Accuweather-mcp

There are many to choose from, here's one that requires authentication to help us work with API Keys.

Source: https://github.com/TimLukaHorstmann/mcp-weather

**We will ask:**

> check the weather in colorado springs, co. Give a detailed report for today.

> check the weather in portalnd, or. Give a detailed report for today.

### Setup in Copilot CLI

- /mcp add
- Server Name: `AccuWeather`
- Server Type: `2` STDIO
- Command: `npx -y @timlukahorstmann/mcp-weather`
- Env: 
  - `ACCUWEATHER_API_KEY=zpka_8d0282cff6c1458597f39ff1d8e7e016_43bba44b`
  - `ACCUWEATHER_API_KEY=${env:ACCUWEATHER_API_KEY}`


### Setup direct JSON

file: C:\Users\Joe\.copilot\mcp-config.json

```json
{
  "mcpServers": {
    "AccuWeather-mcp": {
      "tools": [
        "*"
      ],
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
  }
}
```


