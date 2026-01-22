# Jam 2026 - Install AI

If you don't already have these, here is a primer for install. These are based on Windows / Powershell. 

## Installation Steps for GitHub Copilot CLI

https://docs.github.com/en/copilot/how-tos/set-up/install-copilot-cli

Open your Terminal (Command Prompt, PowerShell, or equivalent for your OS).

> npm install -g @github/copilot

Now type `copilot` and follow prompts / authentication steps.


## Installation Steps for Gemini CLI

https://geminicli.com/docs/get-started/

Gemini Version 0.25.0

Open your Terminal (Command Prompt, PowerShell, or equivalent for your OS).

Run the following command to install Gemini CLI globally using npm:

> npm install -g @google/gemini-cli

You can auth with Google Login or with API Key. 

### Auth with API Key

**Add a new environment variable**

 - Click New...
 - Variable name: GEMINI_API_KEY
 - Variable value: (tbd)
 - Get your key from google: https://aistudio.google.com/app/api-keys
   - Create New. 
   - Copy and paste into Environment variable.

### Verify the installation

You must open a new Terminal window after creating the environment variable above!!!

In the new Terminal, type `gemini` (it takes multiple seconds to load on my machine)

#### Settings

In Gemini type `/settings`

Some suggested changes: 

- Preview Features - true
- Disable Auto Update
- Enable Prompt Completion
- Enable Session Cleanup - true
- Hide Context Window Percentage - false


#### Model

In Gemini type `/model`

- gemini-3-flash-preview
- gemini-2.5-flash
- gemini-2.5-flash-lite

