# Privacy

## Where your data lives
This project has no server, app or database. Your coaching data exists only in:
1. **Your chats** on ChatGPT or Gemini, under those companies' own privacy policies and your account settings.
2. **Your two memory files** (`learner_memory` and `session_log`), stored wherever **you** put them: your device, your ChatGPT project Files, or your Google Drive folder `English-Coach-Memory`.

The project authors never receive your data.

## What the coach is told never to store
Passwords, ID numbers, bank or card details, health information, and private details about other people. It keeps only what helps your English: goals, recurring mistakes, topics and scores.

## Your control
- `show memory`: see what is stored.
- `forget <detail>`: remove something. It disappears from the next files the coach gives you; save those files to make it permanent.
- You can open and edit the memory files yourself at any time. Keep the headings and the `schema: ecc-v1` line.
- Delete the files (and the project or Gem) to remove everything.

## Google Drive
If you use the Drive option, add only the two memory docs to the Gem's Knowledge. That limits what the coach can see. Giving Gemini general access to your whole Drive is **not** needed. The "only read `English-Coach-Memory`" rule is an instruction the AI follows, not a technical lock.

## Platform settings worth checking
- ChatGPT and Gemini may use chats to improve their models depending on your settings. Review **Data controls** (ChatGPT) and **Gemini Apps Activity** (Gemini) if this matters to you.
- ChatGPT's general **Memory** feature is separate from this coach's files. Choosing *Project-only* memory keeps things tidy.

## For contributors
**Never commit real learner files.** Only blank templates and fictional examples belong in this repository. The `.gitignore` blocks `my-memory/`, `memory/` and `private/` folders.
