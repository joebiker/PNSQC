# Weather

## National Weather Service

https://github.com/modelcontextprotocol/quickstart-resources/tree/main/weather-server-typescript

https://github.com/adarshem/mcp-server-learn

https://smithery.ai/servers/adarshem/mcp-server-learn

### Setup

> codex mcp add ns node 'C:\Users\Joe\source\weather\build\index.js'

> gemini mcp add weather node "C:\\Users\\Joe\\source\\quickstart-resources\\weather-server-typescript\\build\\index.js"

### Usage

**We will ask:**

> using the weather mcp check the weather in portalnd, or. Give a detailed report for today.

## Accuweather

Not a great Weather App. Underlying API is limited to 15 day trial and too expensive monthly fee.

Source: https://github.com/TimLukaHorstmann/mcp-weather

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
