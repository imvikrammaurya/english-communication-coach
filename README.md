# 🗣️ English Communication Coach

**A free, strict, personal English coach that runs inside ChatGPT or Gemini.** No app, no code, no website. You copy two files into ChatGPT or Gemini and start practising.

It talks with you about real situations (work, interviews, presentations, daily life). When you make an important mistake in **grammar, word choice, phrasing or tone**, it stops you, shows exactly what was wrong, explains why, and **makes you say it again until you get it right**. At the end you get an honest report with scores and a study plan. Your progress is remembered between sessions.

---

## ✨ What it does

- **Corrects you until you're right.** Exact mistake, why it's wrong, the fix, a rule, then *your turn*. No giving up after one try.
- **Fixes tone, not just grammar.** "Send me the report" to your manager? It'll show you politer, more professional options.
- **Keeps a real conversation going.** One question at a time, follows your answers, and doesn't keep asking "do you want to continue?"
- **Honest scores.** Six skill areas scored 0–10, marked *provisional* when there isn't enough evidence. No inflated marks, no invented mistakes.
- **Remembers you.** Your goals, recurring mistakes and topics are kept in two small files that **you own**.
- **Explains in your language** if you want (`explain in Hindi`), with examples kept in English.
- **Coaching notes after every session.** Written mini-lessons on your top weak points: the rule, when to use it and when not to, your own mistake corrected, examples from your conversation, common traps, and a short practice with answers. Ask for one any time with `notes <topic>`.
- **Voice coaching on ChatGPT.** In voice mode it can also tell you how you *sounded*: too loud, angry, rushed or unsure for the situation, plus word stress and pronunciation, and then has you say it again.
- **Free video lessons** matched to your weak points (only verified links, never made up).

---

## 🚀 Quick start (5 minutes)

| Platform | Guide |
|---|---|
| **ChatGPT** (Free, Go, Plus…) | 👉 [docs/INSTALL_CHATGPT.md](docs/INSTALL_CHATGPT.md) |
| **Gemini** (Gems; Google AI Pro, etc.) | 👉 [docs/INSTALL_GEMINI.md](docs/INSTALL_GEMINI.md) |

Then read 👉 **[docs/HOW_TO_USE.md](docs/HOW_TO_USE.md)** for commands, modes and saving memory.

**Short version:**
1. Create a ChatGPT **Project** or a Gemini **Gem** called *English Coach*.
2. Paste [`skill/coach_instructions.md`](skill/coach_instructions.md) into its instructions.
3. Upload [`skill/coach_playbook.md`](skill/coach_playbook.md) as a file / knowledge.
4. Open a chat, type **`start`**, and practise.
5. Type **`end session`** and save the two memory files it gives you.

---

## 💾 How memory works (please read)

ChatGPT and Gemini **cannot save files on their own**, and nothing in this project pretends they can. Memory works like this:

| Setup | Reading memory | Saving memory |
|---|---|---|
| **ChatGPT Project Files** | Automatic in every project chat | Replace 2 files in project Files after each session |
| **Gemini + Google Drive folder `English-Coach-Memory`** | Automatic (the Gem reads only those 2 docs) | Paste the new content into the 2 docs (about 30 seconds) |
| **No Drive** | Attach the 2 files to a new chat | Save the 2 files on your device |
| **ChatGPT + Notion** *(optional, [guide](docs/OPTIONAL_NOTION_CHATGPT.md))* | Automatic | The coach updates Notion after you say yes, **if your plan supports writing**. Otherwise you paste |

At every `end session`, the coach gives you **`learner_memory.md`** and **`session_log.md`**. Save them, and next time it remembers you.

---

## 📁 What's in this repository

```
english-communication-coach/
├── README.md                     ← you are here
├── skill/
│   ├── coach_instructions.md     ← paste into ChatGPT Project / Gemini Gem instructions
│   └── coach_playbook.md         ← upload as a file / knowledge (rubric, templates, examples)
├── templates/
│   ├── learner_memory.md         ← blank memory file
│   └── session_log.md            ← blank session log
├── docs/
│   ├── INSTALL_CHATGPT.md
│   ├── INSTALL_GEMINI.md
│   ├── HOW_TO_USE.md
│   └── OPTIONAL_NOTION_CHATGPT.md
├── examples/
│   └── sample_session.md         ← a full example session (fictional learner)
├── tests/
│   └── acceptance_tests.md       ← scripted checks that the coach behaves correctly
├── PRIVACY.md
├── CONTRIBUTING.md
├── CHANGELOG.md
└── LICENSE
```

---

## ⚠️ Honest limitations

- **Not an exam.** Scores are coaching estimates, not IELTS/TOEFL/CEFR results.
- **Pronunciation and voice-tone feedback needs real audio.** In ChatGPT voice mode the coach can comment on pronunciation, stress, pace and how your voice sounds (calm, angry, unsure) for the situation. This feedback is approximate, not a lab-grade pronunciation test. In typed chat, or when only a transcript is available (often the case in Gemini), it doesn't judge these. Your accent is never treated as a mistake; only clarity and suitability are.
- **AI can make mistakes.** Rarely, it may mark something as wrong that is acceptable. Ask "Are you sure? Isn't that also correct?" and it should reconsider honestly.
- **Platform features change.** ChatGPT and Gemini update their menus and plans often. If a step in the guides looks different, look for the closest option, or [open an issue](../../issues).
- **Usage limits.** Long sessions use your plan's message limits. Shorter, regular sessions work best.

---

## 🔒 Privacy

Your memory files stay with you: on your device, in your ChatGPT project, or in your own Google Drive. **Never commit your personal memory files to a public repository.** The `.gitignore` here blocks the usual locations. See [PRIVACY.md](PRIVACY.md).

---

## 🤝 Contributing

Bug reports, test results on different plans, and improvements are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md).

## 📄 License

[MIT](LICENSE): free to use, share and modify.
