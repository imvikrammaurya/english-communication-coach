# Install on ChatGPT

Works on any ChatGPT plan that has **Projects** and **Custom Instructions**, including Free, Go and Plus. You don't need a custom GPT; personal plans currently can't create new ones.

> Menu names in ChatGPT change from time to time. If a button below has a slightly different name, look for the closest match.

## How it works
The coach is **opt-in**. It stays off until you switch it on.

| You do | ChatGPT does |
|---|---|
| Normal chat, e.g. "Suggest some SEO strategies." | Answers normally. No English corrections. |
| Say **"start English coach"** | Coaching turns **on**: corrections, retries, conversation, report |
| Say **"end session"** | Gives your report, coaching notes and memory files, then coaching turns **off** |

You never need to change settings to switch between normal chats and English practice. The phrase *start English coach* is the switch.

## What you need from this repository

| File | Where it goes |
|---|---|
| `skill/custom_instructions.md` (under 1,500 characters) | ChatGPT **Custom Instructions**, and the **Project instructions** |
| `skill/coach_instructions.md` | Uploaded to the Project's **files** (full coaching rules) |
| `skill/coach_playbook.md` | Uploaded to the Project's **files** (templates, scoring, coaching notes) |
| `templates/learner_memory.md` | Uploaded to the Project's **files** (your memory, blank at first) |
| `templates/session_log.md` | Uploaded to the Project's **files** (your session history, blank at first) |

To get them: on GitHub, open each file and click **Download raw file** (or **Copy raw file**). Or click **Code → Download ZIP** on the main page and unzip it.

## Step 1: Add the Custom Instructions (global switch)
1. Open [chatgpt.com](https://chatgpt.com) → click your profile picture → **Personalization** (or **Settings → Personalization**) → **Custom instructions**.
2. Open `skill/custom_instructions.md`, copy **all** of it, and paste it into the box that asks how ChatGPT should respond (*"What traits should ChatGPT have?"* or similar).
3. Save.

This box allows at most **1,500 characters**. The file is about 1,340, so it fits. Don't paste `coach_instructions.md` here; it's far too long.

## Step 2: Create the Project
1. In the left sidebar, click **New project** (under *Projects*).
2. Name it **English Communication Coach**.
3. If ChatGPT asks about memory, choose **Project-only** memory, so your other chats don't mix into your coaching.
4. Open the project settings (the **⋯** or gear icon next to the project name) → **Instructions**, paste **all** of `skill/custom_instructions.md` again, and save.

## Step 3: Upload the four files to the Project
In the project, click **Add files** (or **Files → Upload**) and upload:
1. `coach_instructions.md`
2. `coach_playbook.md`
3. `learner_memory.md` (the blank template)
4. `session_log.md` (the blank template)

## Step 4: First session
1. Start a **new chat inside the English Communication Coach project**.
2. Say or type: **`start English coach`**
3. Answer the few setup questions (name, goal, strictness…) and start practising.
4. When you're done, type: **`end session`**
5. You get a report, coaching notes, and two updated files: `learner_memory.md` and `session_log.md`. Coaching then switches off.

**Why start inside the Project?** The Custom Instructions can switch the coach on in any chat, but only the Project has the four files. Outside the Project the coach works from the short rules alone: it still corrects you, but without the full rules, templates or your memory. It will tell you the files aren't available.

## Step 5: Save your memory (after every session)
ChatGPT **can't save files by itself.** You save them:

1. Download the two files if the coach offers download links. Otherwise click **Copy** on each code block and paste it into a text file with that exact name. Notepad works; save as `learner_memory.md` and `session_log.md`.
2. In the project's **Files**, delete the old `learner_memory.md` and `session_log.md` and upload the new ones.

Every new chat in the project then reads your latest memory. You don't need to attach anything per chat.

## Voice practice
1. Open a chat **inside the Project** and tap the **voice** icon.
2. Say **"start English coach"**.

In voice mode the coach hears your actual voice, so besides grammar, words and tone it can coach your **delivery**:
- pronunciation of specific words and word stress;
- pace, pauses and volume;
- how your voice sounds (calm, angry, rushed, unsure) and whether that fits the situation. For example: "your words were polite, but you sounded impatient. Say it again more calmly."

Then it asks you to say it again, the same as grammar corrections. Delivery scores appear in your report as **Delivery**.

Notes:
- Your accent is never treated as a mistake; only clarity and suitability are.
- Audio feedback is a helpful estimate, not a professional pronunciation test.
- Voice sessions may not load every Project file or follow every rule perfectly. Starting inside the Project makes it most reliable. If the coach drifts, say "Follow the English Coach rules."
- If the report or files don't appear properly in voice, type `end session` in text after the voice chat.

## Optional: Google Drive
On ChatGPT, project Files are simpler and more reliable than Drive. If your plan offers a Google Drive app, you can keep backups of the two memory files in a Drive folder named `English-Coach-Memory`. ChatGPT still can't **write** to that folder, so you replace the files there yourself.

## Optional: Notion
Want ChatGPT to update your memory for you? If your plan's Notion app supports writing, it can. See [OPTIONAL_NOTION_CHATGPT.md](OPTIONAL_NOTION_CHATGPT.md), which includes a 2-minute test.

## Troubleshooting
| Problem | Fix |
|---|---|
| It corrects my English in normal chats | Custom Instructions are an older version. Paste the current `skill/custom_instructions.md` again. Coaching should only start after "start English coach". |
| Nothing happens after "start English coach" | Check that `custom_instructions.md` is saved in Custom Instructions **and** in the Project instructions, and that you're in a chat inside the Project. |
| "Too long" when saving Custom Instructions | You pasted the wrong file. Use `skill/custom_instructions.md` (under 1,500 characters), not `coach_instructions.md`. |
| It says it can't find the ECC files | You're outside the Project, or the files aren't uploaded. Open a chat inside the Project and check its Files. |
| It forgot me | The memory files in the Project are old copies. Upload the latest ones. |
| It says it saved my files | It can't. Report this as a bug (see CONTRIBUTING). Always save the files yourself. |
| The coach is too soft | Type `mode strict`. |
