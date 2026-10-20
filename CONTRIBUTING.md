# Contributing

Thanks for helping make this coach better. You don't need to know how to code. Most contributions are text.

## Ways to help
1. **Report a bug:** open an issue with:
   - Platform and plan (e.g. "ChatGPT Go, web" or "Gemini, Google AI Pro, Android")
   - What you typed
   - What the coach did
   - What it should have done (see [tests/acceptance_tests.md](tests/acceptance_tests.md))
   - **Remove any personal details** before posting.
2. **Run the acceptance tests** on your platform and post the results in an issue.
3. **Update the install guides** when ChatGPT or Gemini change their menus.
4. **Improve the playbook:** better examples, clearer rules, more error categories.

## Rules for changes
- Keep `skill/custom_instructions.md` **under 1,500 characters**, ChatGPT's Custom Instructions limit.
- Keep `skill/coach_instructions.md` **under 8,000 characters** (it's also pasted into Gemini Gem instructions). Check with any online character counter. Put detail in `coach_playbook.md` instead.
- Keep the activation phrase `start English coach` the same in all files.
- Don't change the `ecc-v1` memory format without bumping it to `ecc-v2` and explaining how to move old files over.
- Every change to coaching behaviour should pass the acceptance tests on at least one platform.
- Only blank templates and **fictional** examples. Never real learner data.
- Never add claims that the coach can save files, hear pronunciation from text, or do anything the platforms don't actually support.
