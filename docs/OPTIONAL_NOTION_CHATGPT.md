# Optional: Notion memory for ChatGPT users

**ChatGPT only.** The normal Gemini app can't connect to Notion.
**Optional.** The coach works fully without it. See [INSTALL_CHATGPT.md](INSTALL_CHATGPT.md) for the standard setup.

## Why use it?
With the standard setup you replace two files in your ChatGPT Project after every session. With Notion connected, ChatGPT may be able to **update your memory pages for you** after you say "yes". Whether that works depends on your plan and the current Notion app in ChatGPT, so **test it first** (Step 3).

| What | Works? |
|---|---|
| ChatGPT **reading** your Notion memory pages | Usually yes, wherever the Notion app is available on your plan |
| ChatGPT **writing** (updating) your Notion pages | Only if your plan and the Notion app support write actions. Not confirmed for every plan, including Free and Go |

If writing doesn't work for you, Notion still works as a **read-only** memory store: ChatGPT reads it, and you paste the updates in yourself.

## Step 1: Create the Notion pages
1. Sign up for or log in to [Notion](https://www.notion.com) (the free plan is fine).
2. Create a page named **`English-Coach-Memory`**.
3. Inside it, create two sub-pages named exactly:
   - **`ECC learner_memory`**: paste the contents of [`templates/learner_memory.md`](../templates/learner_memory.md)
   - **`ECC session_log`**: paste the contents of [`templates/session_log.md`](../templates/session_log.md)

## Step 2: Connect Notion to ChatGPT
1. In ChatGPT, open **Settings → Apps** (older versions may call it *Connectors*).
2. Find **Notion** and click **Connect**.
3. On the Notion permission screen, **select only the `English-Coach-Memory` page**. Don't give access to your whole workspace. This is a real technical limit: ChatGPT can only see the pages you select here.
4. Approve.

If you don't see Notion in Apps, your plan or region doesn't have it yet. Use the standard Project Files setup.

## Step 3: Test whether ChatGPT can write (2 minutes)
In a chat inside your **English Coach** project, type:

> Read my Notion page "ECC session_log", then add the line "write test OK" under "Archived".

Then open the page in Notion.

| Result | What it means |
|---|---|
| ✅ The line appeared | Writing works. The coach can update your memory after each session. |
| ❌ It says it can't edit, or nothing changed | Read-only on your plan. Use Notion for reading and paste updates yourself, or stay with Project Files. |

Remove the test line afterwards.

## How sessions work with Notion
1. Type `start`. The coach reads `ECC learner_memory` and `ECC session_log` from Notion.
2. Practise as usual.
3. Type `end session`. The coach:
   - shows your report,
   - prints both memory files as a backup (always),
   - asks **"Update your Notion pages now?"**,
   - on **yes**, replaces both pages, reads them back, and tells you the real result: **"Saved to Notion (verified)"**, or an error.
4. If it says anything other than *verified*, paste the printed files into the Notion pages yourself.

## Safety tips
- **Don't use both Notion and Project Files for memory.** Pick one, so you never have two different versions. If you switch, copy the latest content across first.
- **Keep a backup.** Notion has page history (⋯ → *Page history*), so if an update goes wrong you can restore an earlier version.
- **Don't keep other private content** inside `English-Coach-Memory`. The coach can see everything in that page.
- To disconnect: ChatGPT **Settings → Apps → Notion → Disconnect**, and/or Notion **Settings → Connections** → remove ChatGPT.

## Troubleshooting
| Problem | Fix |
|---|---|
| "I can't find your Notion pages" | Check the page names are exact, and that you selected `English-Coach-Memory` when connecting. Reconnect if needed. |
| The coach says "saved" but Notion didn't change | It should never say this without verifying. Paste the files manually and [report it](../CONTRIBUTING.md). |
| The formatting looks odd in Notion | That's fine. The coach reads the text. Keep the headings and the `schema: ecc-v1` line. |
