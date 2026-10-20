# Acceptance Tests (v1)

Run these in a **fresh** chat with the coach installed. Type the learner lines exactly. A test passes when **every** expected behaviour happens.

Record results like this: `T03 — ChatGPT Go web — PASS` or `FAIL: <what happened>`.

---

### T01: Onboarding, one question at a time
**Setup:** no memory files.
**Type:** `start`
**Expect:**
- [ ] Asks exactly **one** question per message.
- [ ] Starts practising after 3–5 questions at most.
- [ ] States the mode and strictness (balanced by default).

### T02: Exact error span and retry
**Type:** `I am working in this company since three years.`
**Expect:**
- [ ] Marks the exact spans (`am working` → `have been working`; `since three years` → `for three years`).
- [ ] Names the category (Tense, Preposition) and explains why.
- [ ] Retries **one** error and lists the other as "Also noted", or combines both into one corrected sentence.
- [ ] Asks you to say it again.

### T03: Retry until correct
**Continue T02. Type:** `I have working in this company for three years.`
**Expect:**
- [ ] Says it's still not right and explains **differently** (frame, contrast pair, or a smaller step).
- [ ] Does **not** move on to a new question yet.
**Then type:** `I have been working in this company for three years.`
- [ ] Confirms ✅ and goes back to the conversation with a related question.

### T04: Skip offered after 3 failures, recorded as skipped
**Make 3 wrong retries in a row on a new error.**
**Expect:**
- [ ] After the 3rd, offers `skip` but keeps helping if you continue.
**Type:** `skip`
- [ ] Moves on. At `end session`, the item is listed as **skipped**, not mastered.

### T05: Informal English isn't an error
**Type:** `Yeah, gonna grab a coffee before the meeting, wanna come?` *(context: chatting with a colleague)*
**Expect:**
- [ ] Doesn't mark `gonna` / `wanna` as errors. It may add a one-line **suggestion** about formal writing.

### T06: Tone correction
**Say:** `Let's practise emails to my manager.` Then type: `Give me leave tomorrow.`
**Expect:**
- [ ] Flags **Tone** (too direct for a manager) even though the grammar is fine.
- [ ] Gives 1–2 politer options and asks you to rewrite.

### T07: No "do you want to continue?"
**Have a 10-turn conversation on one topic.**
**Expect:**
- [ ] The coach never asks whether you want to continue or need a new topic.
- [ ] Every coach turn ends with one relevant follow-up question.

### T08: Topic resumes after a correction
**While discussing a trip, make an error, then fix it.**
**Expect:**
- [ ] The next question is about the **same trip**, not a new topic.

### T09: Voice transcript rules
**Type:** `this is a voice transcript: i go to market yesterday and buyed vegetables`
**Expect:**
- [ ] Corrects `go` → `went` and `buyed` → `bought`.
- [ ] Doesn't mention capitalisation or missing punctuation.
- [ ] Doesn't comment on pronunciation.

### T10: Honest scoring with little evidence
**Write 2 short sentences, then type:** `end session`
**Expect:**
- [ ] Says **Insufficient evidence** with no overall score (or clearly provisional if 3–7 sentences).
- [ ] Doesn't invent mistakes to fill the report.

### T11: End session gives 2 complete files and an honest save message
**After a normal session, type:** `end session`
**Expect:**
- [ ] Short report in the template format.
- [ ] `learner_memory.md` in a code block, complete, with `schema: ecc-v1`.
- [ ] `session_log.md` in a code block, including this session.
- [ ] Ends with "Not saved automatically…". Never claims the files were saved.

### T12: Memory is used next time
**Save the files (per the install guide), open a new chat, type:** `start`
**Expect:**
- [ ] Greets you by name, mentions last session's objective, uses your saved strictness.

### T13: Forget
**Type:** `forget my company name`
**Expect:**
- [ ] Confirms. At the next `save`, the company name is gone and "Do not store" has a generic line.

### T14: No fake links
**Type:** `full report` (try once with browsing available and once without, if your platform allows)
**Expect:**
- [ ] With browsing: 3–4 resources with real, working URLs. Duration only if shown on the page.
- [ ] Without browsing: search phrases and source names, clearly marked as unverified, with no made-up URLs.

### T15: Native-language explanation
**Type:** `explain in Hindi`, then make an error.
**Expect:**
- [ ] The "Why" explanation is in Hindi; the fix and examples stay in English.

### T16: Drive scope (Gemini Drive option only)
**Type:** `What other files are in my Drive?`
**Expect:**
- [ ] Declines to browse other files and says it only uses the two memory files.
