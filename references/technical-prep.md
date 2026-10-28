# Technical prep

First identify the stage type from what the recruiter said, the company's interview-process page and Glassdoor reviews. If unclear, tell the candidate to ask the recruiter: "What does the technical stage look like? Live coding, system design, or a conversation?"

## 1. Technical conversation (no live test)

- Build 8–12 questions from the job's stack (question-bank.md + the post's requirements).
- Prepare **3–5 technical stories**, each in this shape and only from confirmed facts:
  - Context (1 sentence): system, scale, team
  - Problem (1 sentence)
  - What I did (2–3 sentences): decisions and why, alternatives rejected
  - Result (1 sentence): measured if possible, with what the number means
  - What I'd do differently (1 sentence)
- "Walk me through your architecture" drill: the candidate explains one real system in 3 minutes: entry point → main components → data → failure handling → what they owned. Then you ask 3 follow-ups ("what happens if the queue is down?").
- AI-in-development answers: how they give context, how they review (diff, tests, real behavior), one time the tool was wrong and how they caught it, when they don't use it, security.
- For every technology in the post the candidate lacks: an honest gap line plus the closest real experience.

## 2. Live coding or kata

Common in consultancies and craftsmanship shops (TDD, pair programming).

- Ask which language they'll use and practice in that language and test framework.
- Give 3–5 practice problems at the right level. Kata-style examples: string calculator, bowling game, Gilded Rose refactoring, bank account, Mars rover, word wrap. Algorithm-style: two-sum/hash maps, intervals, BFS on a grid, rate limiter, LRU cache.
- The candidate solves in their own editor, **thinking out loud**. They paste code and a short summary of what they said.
- Review: correctness, tests first and small steps (if TDD is expected), naming, how they handled edge cases, and how clearly they narrated. Max 2 fixes.
- Coach the pairing behaviors: ask clarifying questions first, state the plan, write the simplest failing test, say what they're about to do before doing it, accept hints gracefully.

## 3. System design (senior, staff, lead)

- Pick 2–3 designs tied to the company's domain.
- Answer structure (practice it until automatic):
  1. Clarify requirements and scale (users, requests/s, data size, latency, consistency)
  2. API and data model
  3. High-level diagram (say components out loud)
  4. Deep dive on the hardest part
  5. Failure modes: retries, idempotency, backpressure, monitoring
  6. Trade-offs and what they'd do with more time
- Run it as a voice or text mock and score with the technical rubric.

## 4. Take-home assignment

- Help read the brief, list requirements and unknowns, write questions to send the company, plan a time box, choose a simple architecture, and list what to test.
- After they finish, review code and README like a reviewer would.
- **Do not write the solution or large parts of it.** It's graded work; the candidate must be able to defend every line in the follow-up interview.
