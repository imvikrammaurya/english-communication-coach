# Install on Gemini (Gems)

Works on Gemini with any plan that supports **Gems**, including Google AI Pro. The coach is a Gem: a saved custom assistant with its own instructions and knowledge files.

> Menu names in Gemini change from time to time. If a button below has a slightly different name, look for the closest match.

## What you need from this repository
- `skill/coach_instructions.md`: pasted as the Gem instructions
- `skill/coach_playbook.md`: added as Gem knowledge
- `templates/learner_memory.md` and `templates/session_log.md`: your memory files

To get them: on GitHub, open each file and click **Copy raw file** or **Download raw file**, or click **Code → Download ZIP** on the main page.

## Step 1: Create the Gem
1. Open [gemini.google.com](https://gemini.google.com) and sign in.
2. In the left sidebar, open **Gems** (or **Explore Gems**), then click **New Gem**.
3. Name it **English Coach**.
4. In **Instructions**, paste **all** of `skill/coach_instructions.md`.
5. Under **Knowledge**, click **+** and upload `skill/coach_playbook.md`.
6. Click **Save**. If you change knowledge files later, click **Update** too, or the change may not stick.

## Step 2: Choose how to store your memory

### Option A: Google Drive folder (recommended on Gemini)
Your memory lives in your own Google Drive, and the Gem reads only the two files you give it.

1. In [Google Drive](https://drive.google.com), create a folder named exactly **`English-Coach-Memory`**.
2. Inside it, create two **Google Docs** named **`learner_memory`** and **`session_log`**.
3. Paste the contents of `templates/learner_memory.md` into the first doc and `templates/session_log.md` into the second.
4. Edit your Gem → **Knowledge → + → Add from Google Drive** → pick both docs → **Update / Save**.

**What happens each session:**
- **Reading is automatic.** The Gem reads the two docs at the start of every chat.
- **Saving is a paste (about 30 seconds).** Gemini can't write into your Drive docs by itself. After `end session`, open each doc, select all, delete, and paste the new version the coach gave you. Copy and paste the whole block.

**Check once that updates are picked up:** after your first save, start a **new** chat with the Gem and type `show memory`. If it shows your latest details, you're set. If it shows old content, Gemini is using a snapshot. In that case, remove the two docs from the Gem's Knowledge and add them again after each save, then click **Update**.

**Why "only that folder"?** The Gem only sees files you added to its Knowledge. Adding the two docs this way (rather than giving Gemini general access to your whole Drive) keeps it limited to your memory files. The instructions also tell the coach never to open anything else. That's a rule the AI follows, not a technical lock, so the Knowledge method is the safer one.

### Option B: No Drive (files only)
1. Start the first session without memory files (the coach will onboard you).
2. After `end session`, copy the two code blocks into text files named `learner_memory.md` and `session_log.md` and save them anywhere you like.
3. Before every new chat, either add them to the Gem's **Knowledge** (replacing the old ones, then **Update**) or attach them to the chat with **+ → Upload files**.

## Step 3: First session
1. Open the **English Coach** Gem and start a chat.
2. Type: `start`
3. Answer the setup questions and practise.
4. Finish with: `end session`
5. Save the two files (Option A or B above).

## Voice practice
Use Gemini Live or the microphone inside the Gem chat if your app version supports it there. The coach works from the transcript, so it ignores punctuation and doesn't grade pronunciation from transcripts. For the strictest grammar and tone correction, text chat gives the most reliable results.

## Troubleshooting
| Problem | Fix |
|---|---|
| The coach doesn't correct me | Make sure you opened the **English Coach** Gem, not a normal chat. Type `mode strict`. |
| It doesn't know me | Your docs aren't in Knowledge, or Gemini cached an old copy. Re-add them and click **Update**. |
| It reads other Drive files | Remove general Drive access from the chat and use only the Gem's Knowledge (Option A). Report the issue. |
| It says it saved my files | It can't. Always paste the new content into your docs yourself. |
