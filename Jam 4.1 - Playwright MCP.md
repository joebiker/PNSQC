# MCP Demo - 3 Playwright

https://github.com/microsoft/playwright-mcp?tab=readme-ov-file

https://techcommunity.microsoft.com/blog/azuredevcommunityblog/how-to-integrate-playwright-mcp-for-ai-driven-test-automation/4470372

## VS Code + Playwright MCP: open pnsqc.org

### Add the Playwright MCP server

In VS Code, open Command Palette and run:

- `MCP: Add Server`
- Type: `stdio`
- Command: `npx`
- Args: `@playwright/mcp@latest --browser chrome`

### Use it (Copilot Chat)

Prompt:

"Using the Playwright MCP server, open https://pnsqc.org/ in Chrome and wait."

### Register Test

Here are the prompts provided to develop the register test:

- create playwright scaffold.
- open chrome to the page https://pnsqc.org/
- on the chrome page click the link with text "PNSQC Quality Jam"
- create a new test called "register". Click the page click the link with text "PNSQC Quality Jam", then click the button register." (Request to scaffold the new test and navigate to the first registration link)
- on the new page, next click on the button "Register for this event" (Direction to handle the new tab and proceed to the form)
- after clicking the register link, fill in the form with general info and select the radio button "Online". Then wait 3 seconds to review the output.  (Final logic to populate the attendee details and select the attendance type)
