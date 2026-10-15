# MCP Demo - Playwright

https://github.com/microsoft/playwright-mcp

https://techcommunity.microsoft.com/blog/azuredevcommunityblog/how-to-integrate-playwright-mcp-for-ai-driven-test-automation/4470372

## Playwright MCP

### Add the Playwright MCP server

one liner

```powershell
codex mcp add playwright npx "@playwright/mcp@latest"
```

same for claude

```powershell
claude mcp add playwright npx "@playwright/mcp@latest"
```

In VS Code, open Command Palette (ctrl + shift + p) and type:

- `MCP: Add Server`
- Choose: `stdio`
- Command: `npx`
- Args: `@playwright/mcp@latest --browser chrome`

### Links for install in Claude

https://playwright.dev/docs/getting-started-mcp

https://modelcontextprotocol.io/docs/2026-07-28/develop/connect-local-servers

### Use it (Copilot Chat)

Prompt:

> "Using the Playwright MCP server, open https://pnsqc.org/ in Chrome and wait."

### Build Our Tests

Using Claude...

1. **Prompt:** `On the biolumina board, what items do I have in to do that are QA related?`
   **What Claude did:** Found the Biolumina Trello board and listed the two QA-labeled cards in TODO: "QA check headings H1 H2" and "Fill out the international shipping form".

2. **Prompt:** `Move the first card into the next column.`
   **What Claude did:** Moved "QA check headings H1 H2" from TODO to Ready To Work.

3. **Prompt:** `Summarize that card what we need to do next.`
   **What Claude did:** Turned the card's heading and SEO checklist into six next steps and noted that the card has no page list, assignee or due date.

4. **Prompt:** `Add this test to my playwright suite of tests.`
   **What Claude did:** Wrote `tests/heading-structure.spec.ts`, which checks headings on all 7 site pages and found skipped heading levels and headings added only by JavaScript.

5. **Prompt:** `run the tests`
   **What Claude did:** Ran the full Chromium suite: 35 tests, 24 passed and 11 failed, all because of real heading problems on the site.

6. **Prompt:** `Using carbon MCP, can you help me write better tests?`
   **What Claude did:** Ran a Carbon assessment that recorded 10 checks and 7 site issues, then added navigation, product and site-health specs plus a shared page list, bringing the suite to 80 tests (65 pass, 15 fail on real site issues).

7. **Prompt:** `summarize my prompts into a concise list. Provide them exactly as i typed and give a one sentence summary of what you did. Format for MD file upload.`
    **What Claude did:** Wrote this file.

## Sessions

If you need to exit, be sure to restore your session!

```powershell
claude --resume 8f0057f9-de50-46d7-ad1c-0db37e55e8ac
```

for a list of sessions:

```powershell
claude --resume
```
