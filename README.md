# ThreadBridge

**ThreadBridge** is a local-first Chrome extension that helps you capture Reddit discussion context, draft page-aware replies with ChatGPT, organise company workspaces, and queue drafts for review before manual submission.

## Download

The repository's **Code → Download ZIP** download contains the source checked into this repository. The Chrome Web Store package and complete release kit are currently available as release files in the original project delivery; they still need to be attached here as downloadable GitHub release assets.

## What it does

- Keeps each company or brand's positioning and outreach rules in a separate local workspace.
- Imports ChatGPT research output from pasted text or JSON.
- Captures the current Reddit post and visible comments, sorting by detected scores when available.
- Builds a page-specific prompt for ChatGPT.
- Formats each sentence of a comment as its own paragraph.
- Approves and schedules drafts at least 10 minutes apart.
- Opens the target and tries to fill a Reddit editor when scheduled; the user reviews and submits manually.

## Safety and limitations

ThreadBridge does **not** press Reddit's Submit button. It does not vote, follow, direct-message, or perform engagement actions automatically. The timer and draft data are local to the browser profile. If Reddit changes its interface, editor detection may fail; manual copy/paste remains the fallback.

Use the extension in accordance with each community's rules. Do not use it for repetitive mass outreach, fake conversations, or coordinated inauthentic engagement.

## Install from source

1. Download the repository using **Code → Download ZIP** and extract it.
2. Open `chrome://extensions` in Chrome.
3. Enable **Developer mode**.
4. Click **Load unpacked** and select the folder containing `manifest.json`.
5. Refresh any Reddit tabs that were already open.

## Testing

The project includes automated checks; run `npm test` from the extension project folder with Node.js 18 or later. Passing automated tests is not a substitute for testing against Reddit's live interface.

## Privacy

Drafts and workspace settings are stored locally in the browser profile. Do not put confidential information into a shared browser profile. The extension does not require your Reddit password or an API key.

## Project status

Version 0.3.1. This is an independently maintained community tool, not an official product of Reddit or OpenAI.
