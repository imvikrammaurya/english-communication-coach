# Install on ChatGPT

Works on any ChatGPT plan that has **Projects**, including Free, Go and Plus. You do not need a custom GPT. Personal plans currently can't create new custom GPTs, so this setup uses a Project instead.

> Menu names in ChatGPT change from time to time. If a button below has a slightly different name, look for the closest match.

## What you need from this repository
- `skill/coach_instructions.md`: pasted as the Project instructions
- `skill/coach_playbook.md`: uploaded as a Project file
- `templates/learner_memory.md` and `templates/session_log.md`: only needed later, after your first session

To get them: on GitHub, open each file and click the **Copy raw file** or **Download raw file** button, or click **Code → Download ZIP** on the main page and unzip it.

## Step 1: Create the Project
1. Open [chatgpt.com](https://chatgpt.com) and sign in.
2. In the left sidebar, click **New project** (under *Projects*).
3. Name it **English Coach**.
4. If ChatGPT asks about memory, choose **Project-only** memory. This keeps your other chats from mixing into your coaching.

## Step 2: Add the instructions
1. Open the project, then open its settings (the **⋯** or gear icon next to the project name) and find **Instructions**.
2. Open `skill/coach_instructions.md`, copy **all** of it, and paste it in.
3. Save.

## Step 3: Add the playbook
1. In the project, click **Add files** (or **Files → Upload**).
2. Upload `skill/coach_playbook.md`.

## Step 4: First session
1. Start a **new chat inside the English Coach project**. Chats outside the project won't follow the coach rules.
2. Type: `start`
3. Answer the few setup questions and start practising.
4. When you're done, type: `end session`
5. The coach gives you a report and two files: `learner_memory.md` and `session_log.md`.

## Step 5: Save your memory (after every session)
ChatGPT **can't save files by itself.** You save them:

1. Download the two files if the coach offers download links. Otherwise click **Copy** on each code block and paste it into a text file with that exact name. Notepad works; save as `learner_memory.md`.
2. In the project's **Files**, delete the old `learner_memory.md` and `session_log.md` (if any) and upload the new ones.

From then on, every new chat in the project reads your memory automatically. You don't need to attach anything per chat.

> **Quicker option:** skip uploading to project Files and attach the two files to each new chat with the 📎 button instead. Either works; project Files is less effort.

## Voice practice
Open a chat in the project and tap the **voice** icon. In ChatGPT voice mode the coach hears your actual voice, so besides grammar, words and tone it can coach your **delivery**:
- pronunciation of specific words and word stress;
- pace, pauses and volume;
- how your voice sounds (calm, angry, rushed, unsure) and whether that fits the situation, e.g. "your words were polite, but you sounded impatient; say it again more calmly."

Then it asks you to say it again, the same as grammar corrections. Delivery scores appear in your report as **Delivery**.

Notes:
- Your accent is never treated as a mistake; only clarity and suitability are.
- Audio feedback is a helpful estimate, not a professional pronunciation test.
- If voice mode seems to ignore the coach rules, say "Follow the English Coach rules". If it still doesn't, use text chat for strict grammar practice. Voice behaviour varies by app version.
- Type `end session` in text after a voice chat if the report doesn't appear in voice.

## Optional: Google Drive
On ChatGPT, using project Files is simpler and more reliable than Drive. If your plan offers a Google Drive app or connector, you can keep backups of the two files in a Drive folder named `English-Coach-Memory`. ChatGPT still can't **write** to that folder, so you replace the files there yourself.

## Optional: Notion
Want ChatGPT to update your memory for you? If your plan's Notion app supports writing, it can. See [OPTIONAL_NOTION_CHATGPT.md](OPTIONAL_NOTION_CHATGPT.md), which includes a 2-minute test.

## Troubleshooting
| Problem | Fix |
|---|---|
| The coach doesn't correct me | Make sure you're chatting **inside** the project. Type `mode strict`. |
| It forgot me | The memory files aren't in the project Files, or they're old copies. Re-upload the latest ones. |
| It says it saved my files | It can't. Report this as a bug (see CONTRIBUTING). Always save the files yourself. |
| The instructions won't fit | Paste `coach_instructions.md` only. The playbook goes in Files, not in instructions. |
