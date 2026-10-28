# Question bank

Pick 10–15 for the stage and the job post. Rewrite role-specific ones with the company's stack and domain. Answers go in `notes.md`, built only from confirmed facts.

## Screening (recruiter)

- Tell me about yourself.
- Why are you looking for a new opportunity? / Why did you leave your last job?
- Why this company? Why this role?
- This is a contractor / B2B contract. Are you comfortable with that?
- What are your salary expectations?
- When could you start? What's your notice period?
- The team is in <time zone>. Does that work for you?
- How would you rate your English?
- Are you in other processes?
- What do you know about us?

## Behavioral (problem → what I did → result)

- What's the technical achievement you're most proud of?
- Tell me about a disagreement with a teammate or manager. How did it end?
- Tell me about feedback you initially disagreed with.
- Tell me about a mistake you made and what you changed afterwards.
- Tell me about a time you had to deliver under a tight deadline.
- How do you mentor junior engineers?
- How do you work in a remote, distributed team?
- Tell me about a time you had to learn something fast.
- What's your biggest weakness? (a real one, with what you're doing about it)
- Tell me about a time you pushed back on a product or business decision.

## Questions to ask them

Recruiter call:
- What does success look like in the first 3 months?
- What are the next steps and the timeline?
- How is the team organized, and who would I work with day to day?
- What's the biggest challenge the team is facing right now?

Technical / team interview:
- How do you ship to production? How often, and what's the review process?
- How do you use AI coding tools as a team? Any rules?
- What does on-call look like?
- What's the part of the system you'd most like to rewrite, and why?
- (From research) "I saw <fact>. How did that change the engineering work?"

## AI in software development

- How do you use coding agents (Claude Code, Codex, Cursor, Copilot) day to day?
- How do you give an agent good context in a large codebase?
- How do you review and validate code an agent generated?
- Tell me about a time an agent got something wrong. How did you catch it?
- When would you NOT use a coding agent?
- What are the security risks of coding agents, and how do you manage them?
- How would you know if agents are actually making the team faster?
- Have you shipped LLM-powered features? What did you learn? (evaluation, cost, latency, hallucinations)
- What is MCP? What is RAG? When would you use each?
- Will AI replace software engineers?

## Backend & architecture

- How do you make communication between services reliable?
- How do you implement idempotency?
- What's the outbox pattern and when do you need it?
- Queue/stream delivery guarantees: at-least-once vs exactly-once, and how you design consumers.
- A service is slow or using too much memory in production. How do you investigate?
- How would you extract a piece of a monolith into a service?
- What's your testing strategy for a service? Unit, integration, contract, end-to-end.
- How do you evolve an API or event schema without breaking consumers?
- How do you set up observability (logs, metrics, traces, alerts)?

## Databases

- SQL or NoSQL for <use case>: how do you choose?
- How do you find and fix a slow query?
- How do you change a schema without downtime?
- Transactions and isolation levels: a bug you've seen because of them.

## Delivery & reliability

- What are DORA metrics, and how would you improve them?
- Walk me through a CI/CD pipeline you've built or used.
- Tell me how you handle a production incident.
- How do you decide between speed and quality on a time-boxed project?

## System design (adapt to the company's domain)

- Design an order and payment flow for a marketplace.
- Prepare the system for a big traffic spike (campaign, launch).
- Design a notification system (email, SMS, push).
- Integrate safely with third-party webhooks.
- Design <a feature from the company's product> with an LLM in the loop.

## Product & domain

- What does "product mindset" mean to you?
- How do you turn a vague business request into something you can build?
- How do you know a feature was successful?
- How do you prioritize when everything seems urgent?
- What do you know about <company's market>? What makes it hard?
