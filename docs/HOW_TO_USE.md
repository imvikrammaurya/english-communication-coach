# How to Use the English Communication Coach

## The daily loop

```
open the coach  →  type "start"  →  talk / write  →  fix mistakes until correct  →  "end session"  →  save the 2 files
```

1. **Open the coach:** a new chat in the *English Coach* ChatGPT Project, or the *English Coach* Gem in Gemini.
2. **Type `start`.** The coach reads your memory, reminds you of last time's goal, and begins.
3. **Practise.** Talk about anything: your job, an interview, a presentation, your weekend. The coach asks one question at a time and keeps the conversation going.
4. **Fix your mistakes.** When you make an important mistake, the coach stops, shows exactly what was wrong, explains why, and asks you to **say it again**. It keeps going until you get it right. Type `skip` if you want to move on (it's recorded as *skipped*, not *learned*).
5. **Type `end session`.** You get a report with scores, your top mistakes, priorities and an exercise, plus your two memory files.
6. **Save the two files.** This is the step that gives the coach memory. See below.

## What gets corrected

| Area | Examples |
|---|---|
| Grammar | tenses, articles (a/an/the), prepositions, word order, agreement |
| Words | wrong word, unnatural word combinations, repetition, fillers |
| Speech & phrasing | complete sentences, natural phrasing, clarity, structure |
| Tone | too direct, too casual, too formal for the person you're talking to |

**Not graded from text:** pronunciation, accent and speaking speed. The coach is honest that it can't judge these from a transcript.

## Strictness: choose how hard the coach pushes

| Command | What happens | Best for |
|---|---|---|
| `mode balanced` *(default)* | Stops you for important mistakes and makes you retry; small ones go into the report | Most learners |
| `mode strict` | Stops you for **every** meaningful mistake until it's right | Serious, fast improvement |
| `mode fluency` | Never interrupts; everything goes into the report | Building confidence, speaking practice |

In every mode, the mistakes that do get retried are retried **until you get them right** or type `skip`.

## All commands

| Command | Does |
|---|---|
| `start` | Begin (reads your memory) |
| `help` | Show commands |
| `skip` | Move on from the current correction |
| `mode strict` / `mode balanced` / `mode fluency` | Change strictness |
| `practice mode` / `coaching mode` | Conversation vs. more teaching and drills |
| `new topic` | Get topic ideas, or name your own |
| `explain in Hindi` *(or any language)* | Explanations in your language, examples in English |
| `report` | Quick report so far |
| `full report` | Detailed report with study plan and free videos |
| `end session` | Final report + your 2 memory files |
| `save` | Get your 2 memory files now, keep practising |
| `show memory` | See what the coach remembers about you |
| `forget <something>` | Remove a detail from memory |
| `consolidate` | Tidy up a long memory file |

## Saving memory: the important part

The coach **cannot save anything by itself**, on ChatGPT or Gemini. At `end session` it gives you two files:

| File | What's inside |
|---|---|
| `learner_memory.md` | Your profile, goals, strengths, recurring mistakes, topics, score history |
| `session_log.md` | Short records of your last 10 sessions |

Save them using the method you chose during install:

| Your setup | What to do after `end session` |
|---|---|
| **ChatGPT Project Files** | Replace the two files in the project's Files with the new ones |
| **Gemini + Google Drive** | Paste the new content into your two Google Docs in `English-Coach-Memory` |
| **No Drive / files only** | Save both files on your device and attach them to your next chat (or Gem Knowledge) |

**If you forget to save:** the coach won't remember that session. Type `save` mid-session if you think you might leave suddenly.

**Never edit the `schema: ecc-v1` line** or the headings in the files. You *can* fix wrong details in the text, or just tell the coach "that's wrong, I actually…".

## Tips for faster progress
- **Talk in full sentences.** One-word answers give the coach nothing to correct.
- **Practise real situations:** "Let's do a mock interview for a sales job", "Help me practise asking my manager for leave", "Let's role-play a client call."
- **Do the exercise** at the end of each report before your next session.
- **Use `mode strict`** when you have time, and `mode fluency` when you just want to talk.
- **Use `full report` once a week** to get a study plan and free video lessons.

## Example session start

> **You:** start
>
> **Coach:** Hi Priya! Practice mode, balanced. Last time we worked on present perfect with *since/for*. Today's goal: use it correctly 5 times while talking about your work. So, how long have you been working at your current company?
