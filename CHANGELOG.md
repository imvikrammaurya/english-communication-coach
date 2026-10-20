# Changelog

## v1.0.0: first release
- Core coach instructions for ChatGPT Projects and Gemini Gems (`skill/coach_instructions.md`, under 8,000 characters).
- Playbook with error categories, scoring rubric, correction/report templates and worked examples.
- Retry-until-correct loop, with skip offered after 3 failed attempts.
- Strictness modes: balanced (default), strict, fluency. Practice and coaching styles.
- Tone and politeness correction.
- Explanations in the learner's native language (`explain in <language>`).
- Short report by default; full report with verified free resources on request.
- Coaching notes (written mini-lessons) for the top 2–3 weak points at every `end session`, for every priority in `full report`, and on demand with `notes <topic>`.
- Voice delivery coaching when real audio is heard (e.g. ChatGPT voice mode): pronunciation, word stress, pace, volume and vocal tone for the scenario, with retry. Optional "Delivery" score dimension (n/a without audio). Accent is never treated as an error.
- Optional Notion memory guide for ChatGPT users.
- Opt-in activation: coaching starts only with `start English coach` and stops at `end session`; normal chats get no unasked corrections.
- New `skill/custom_instructions.md` (under 1,500 characters) for ChatGPT Custom Instructions and Project instructions. The full rules (`coach_instructions.md`) are now uploaded as a Project file alongside the playbook and both memory files.
- While coaching is on, a real question or task is answered after the correction retry (or `skip`).
- ChatGPT install guide rewritten for this setup.
- Two-file memory (`learner_memory.md`, `session_log.md`) with a fixed `ecc-v1` format and a rolling 10-session log.
- Install guides for ChatGPT and Gemini, including the Google Drive folder option.
- Acceptance test scripts.
