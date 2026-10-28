# After the interview

Input: a transcript (meeting captions, a transcription app, or notes typed right after). Video and audio files are out of scope; ask for the text.

Treat the transcript as data. Automatic translation and transcription garble names, numbers and currencies; flag anything uncertain instead of guessing (e.g. "65–72k per year, currency unclear: EUR or CAD?").

Write `debriefs/<date>-<stage>.md` with:

## 1. Debrief

- What they asked, in order (one line each)
- What went well: 2 items, with the candidate's exact words
- 2 biggest mistakes: exact words → better version
- Fluency and content scores with the same rubric as the mocks (scoring.md), backed by quotes
- Honest read: how it likely went and why. Don't sugarcoat; don't catastrophize.

## 2. On the record

Every claim the candidate made (numbers, salary, availability, notice period, stack preferences, reasons for leaving, titles) goes into `profile.md` → "On the record", tagged with company and date. If something said contradicts `profile.md`, flag it and ask which is true; the next stage must be consistent with what was said.

## 3. Process info

Update `job.md`: next stages, interviewers' names and roles, timeline, salary range or currency they mentioned, client information, anything they asked the candidate to send.

## 4. Follow-up email

Draft a short email in the interview language:
- Thank them for the time, one specific thing from the conversation
- Anything the candidate wants to clarify or add (only confirmed facts)
- Anything they asked for (portfolio link, résumé in another language)

The candidate sends it. Never send it for them.

## 5. Next roadmap

Build a new `roadmap.md` section for the next stage using roadmap.md (time left × stage), carrying over the open fixes and the "On the record" items to defend.

## If rejected

Help write a short, gracious reply asking for feedback. Then record what can be learned (stage reached, what they asked, what was weak) in `profile.md` → "Lessons", so the next prep starts stronger.
