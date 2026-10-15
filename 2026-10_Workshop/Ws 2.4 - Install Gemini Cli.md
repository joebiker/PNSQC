# Install Gemini CLI

If you don't already have it, here is a primer for install. These are based on Windows / Powershell.

## Installation Steps for Gemini CLI

https://geminicli.com/docs/get-started/

Open your Terminal (Command Prompt, PowerShell, or equivalent for your OS).

Run the following command to install Gemini CLI globally using npm:

> npm install -g @google/gemini-cli

You can auth with Google Login or with API Key.

### Google Login

The authentication was successful, and the following products are now authorized to access your account:

Gemini Code Assist
Cloud Code with Gemini Code Assist
Gemini CLI
Antigravity (see Plans for availability)

### Auth with API Key

**Add a new environment variable**

 - Click New...
 - Variable name: GEMINI_API_KEY
 - Variable value: (tbd)
 - Get your key from google: https://aistudio.google.com/app/api-keys
   - Create New.
   - Copy and paste into Environment variable.

[See Usage](https://aistudio.google.com/app/usage?project=gen-lang-client-0176795628&timeRange=last-1-day)

[Rate Limits](https://aistudio.google.com/app/rate-limit?timeRange=last-1-day&project=gen-lang-client-0176795628)

| Model ID | Model Name | Rate Per Day |
| --- | --- | --- |
| gemini-3.1-pro-preview | Gemini 3.1 Pro Preview | TBD |
| gemini-3-flash-preview | Gemini 3 Flash Preview | TBD |
| gemini-3.5-flash-lite | Gemini 3.5 Flash Lite | 15 |
| gemini-3.1-flash-lite | Gemini 3.1 Flash Lite | 15 |
| gemini-2.5-pro | Gemini 2.5 Pro | 0 |
| gemini-2.5-flash-lite | Gemini 2.5 Flash Lite | 10 |
| gemini-3.8-flash | Gemini 3.8 Flash | 5 |
| gemini-3.7-flash | Gemini 3.7 Flash | 5 |
| gemini-3.6-flash | Gemini 3.6 Flash | 5 |

### Verify the installation

You must open a new Terminal window after creating the environment variable above!!!

In the new Terminal, type `gemini` (it takes multiple seconds to load on my machine)

### Other Install Notes

Talks about rate limits.
https://www.npmjs.com/package/@google/gemini-cli

Learn about how they use our data.
https://github.com/google-gemini/gemini-cli/blob/main/docs/tos-privacy.md

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

- gemini-3.1-pro-preview

#### Configuration

User (local computer) config

> C:\Users\Joe\\.gemini>

Workspace

>.gemini/settings.json
