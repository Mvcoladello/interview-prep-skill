# Honesty rules

Interviewers dig. A claim the candidate can't defend under two follow-up questions costs more than the gap it was hiding. These rules are not optional.

## 1. Never invent

- No experience, metric, title, team size, tool, employer, date or result that is not in `profile.md` as **confirmed**.
- Résumé lines start as `unconfirmed`. Ask before using them in an answer ("Your résumé says 40% lower latency. What was measured, before and after, and how?").
- If an answer needs a number you don't have, write the answer without the number and add a gap. Never "round up" or estimate for them.

## 2. Inconsistency check

Before every mock and before the interview, scan `profile.md`, the résumé and past debriefs for the same fact told in different ways (e.g. a metric given as 30% on the résumé and "almost half" in a mock; a title that differs between résumé and LinkedIn). Flag each one and ask which is true. Write the answer with its definition ("checkout errors dropped from 4% to 1% of orders, measured over the month after the release").

## 3. Résumé vs reality

If the résumé lists something the candidate says is not production experience (a cloud, a framework, a language), the answer must say so plainly and pivot to what is real:

> "My production experience is Azure. I've studied AWS and the concepts map well: SQS is close to what I did with Service Bus."

Add a red flag to the mock prompt so the voice interviewer catches overclaiming.

## 4. Salary

- Research the market range for the role, level, region and contract type (see SKILL.md, Research).
- Strategy:
  - Give a number (or a narrow range) at or slightly above the middle of the realistic range.
  - Hold it calmly through the first pushback. "I understand. Based on the scope and my experience, I'm comfortable at X. I'm open to talking about the full package."
  - Don't negotiate against yourself (no "but I could do less").
  - If they ask before you know the scope: "I'd like to understand the role better. Could you share the budget range?"
- Current or last salary: teach a polite redirect ("I'd rather focus on what this role is worth. My expectation is X."). In places where they insist and it's legal to ask, the candidate may answer truthfully or decline. **Never suggest lying about current salary.**
- Everything said about money goes into "On the record" for that company.

## 5. On the record

Whatever the candidate tells a company in a real interview (numbers, salary, availability, notice period, stack preferences, reasons for leaving) is recorded in `profile.md` under "On the record" with company and date. Before every later stage with the same company, remind them of it so they stay consistent.

## 6. Gaps are fine

A plain gap with a learning plan beats a weak claim:

> "I haven't used GraphQL in production. I've designed REST APIs with typed schemas and versioning, so the concepts are familiar, and I'd ramp up quickly."

## 7. Assessments and take-homes

Help plan, practice on similar problems and review after submission. Do not solve a graded assessment or write a take-home for them.
