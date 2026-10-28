# interview-prep

A [Claude Code](https://claude.com/claude-code) skill that coaches you for a **specific job interview**, in English: recruiter screens, technical rounds, hiring-manager and client interviews.

You give it your résumé, the job post and the interview date. It researches the company, builds a prep roadmap sized to the time you have left, writes a cheat sheet you can glance at during the call, makes you close the gaps in your stories, generates voice mock interviews for ChatGPT / Claude / Gemini voice mode, scores your mocks, drills your spoken English, and debriefs the real interview afterwards.

It never puts words in your mouth that aren't true. Every answer is built from facts you confirmed.

---

## Contents

- [What it does](#what-it-does)
- [Install](#install)
- [Quick start](#quick-start)
- [A typical prep, step by step](#a-typical-prep-step-by-step)
- [Your workspace](#your-workspace)
- [Voice mocks](#voice-mocks)
- [Commands you can say](#commands-you-can-say)
- [Rules the coach follows](#rules-the-coach-follows)
- [FAQ](#faq)
- [Update](#update)
- [Português (resumo)](#português-resumo)

---

## What it does

| Module | What you get |
|---|---|
| **Intake** | Reads your résumé and the job post, asks only what's missing (stage, date, hours you have, English level, salary, what worries you). Under 5 minutes. |
| **Research** | What the company does, likely client (for consultancies), hiring process, salary range, culture words to mirror, 3 facts to mention. With sources. |
| **Roadmap** | A checklist sized to the time left (under 24h / 1–3 days / 4+ days) and focused on the stage (HR, technical, manager, client). Each item has a time estimate and a "done when". |
| **Gaps** | Questions you must answer before your answers are final: requirements without a story, numbers without a definition, résumé items that aren't production experience. |
| **Cheat sheet** | `notes.md`: pitch, why this company, requirement → story map, likely questions, salary lines, your questions, rescue phrases. Scannable in 3 seconds. |
| **Voice mocks** | Prompts that turn a voice assistant into the recruiter or interviewer for *this* job, with realistic pushback and a scoring block at the end. |
| **Feedback loop** | Paste the mock result back; the coach re-checks the scores, gives you the 2 fixes that matter, updates your answers and the roadmap. |
| **Technical prep** | Stack questions, technical stories, architecture walk-throughs, kata / live-coding practice with code review, system design. Take-homes: planning and review only. |
| **English** | Fluency drills and a study plan sized to your time, built around *your* recurring mistakes. |
| **Interview day** | Checklists for 2h, 30 min and 15 min before, plus a salary and nerves playbook. |
| **After the interview** | Paste the transcript: debrief with scores, what you said "on the record", process info, a follow-up email draft, and the roadmap for the next stage. |

---

## Install

You need [Claude Code](https://docs.claude.com/en/docs/claude-code/overview) installed and logged in.

```bash
git clone https://github.com/Mvcoladello/interview-prep-skill.git ~/.claude/skills/interview-prep
```

That's it. Claude Code picks up skills from `~/.claude/skills/` automatically. Restart any open Claude Code session.

To check it's installed, open Claude Code and type `/` — you should see `interview-prep` in the list.

---

## Quick start

1. Create a folder for your job search and open Claude Code there:

   ```bash
   mkdir -p ~/job-search && cd ~/job-search
   claude
   ```

2. Start the skill:

   ```
   /interview-prep
   ```

   or just say: *"I have an interview with Acme on Friday, help me prepare"*.

3. Give it your résumé and the job post:

   ```
   My résumé is ~/Downloads/resume.pdf and the job is https://jobs.example.com/senior-backend
   ```

4. Answer the short intake. You'll get a roadmap, a cheat sheet and your first voice mock prompt.

Come back any time with `/interview-prep` — it shows your jobs, the time left and the next step.

---

## A typical prep, step by step

**Day 1 (interview in 3 days)**

1. `/interview-prep` → *new job* → résumé + job post → intake questions.
2. The coach researches the company and writes `job.md`, `roadmap.md`, `notes.md` and `gaps.md`.
3. Answer the gaps (3–5 questions at a time). Your confirmed answers go into `profile.md` and are reused for every future job.
4. Read `notes.md`. Ask for changes: *"make my pitch shorter"*, *"I don't like the why-this-company answer"*.
5. Ask for a mock: *"give me an HR mock"*. Copy the prompt into ChatGPT / Claude / Gemini voice mode and do the call.
6. Say **"feedback"** to the voice assistant, then paste the whole feedback (and transcript, if the app shows it) back into Claude Code.
7. The coach checks the scores, gives you 2 fixes, updates `notes.md` and ticks the roadmap.

**Day 2**

8. Two more mocks with the loop above. A fluency drill if your English is the bottleneck.
9. Technical round coming? *"prep me for the technical interview"* → stack questions, stories, a kata or a design question.

**Interview day**

10. *"interview day"* → short checklists for 2h, 30 min and 15 min before.

**After**

11. Paste the transcript or your notes: *"here's the transcript of the call"*.
12. You get a debrief, a follow-up email to send yourself, and the roadmap for the next stage.

---

## Your workspace

Everything is saved as Markdown in the folder where you run Claude Code:

```
interview-prep/
  profile.md                 your facts, shared by every job
  acme-senior-backend/
    job.md                   job post, research, process, salary data
    roadmap.md               your checklist + mock score history
    notes.md                 the cheat sheet you use during the call
    gaps.md                  open questions about your experience
    mocks/
      1-hr-prompt.txt        paste into voice mode
      1-hr-result.md         your result + the coach's analysis
    debriefs/
      2026-11-03-hr.md       after the real interview
```

- **`profile.md` is the source of truth.** Facts start as `résumé (unconfirmed)` and only become usable after you confirm them. It also keeps what you told each company ("On the record") so you stay consistent across stages.
- These files contain personal data. Don't commit them to a public repository.

---

## Voice mocks

1. Ask for a mock: *"HR mock"*, *"technical mock"*, *"hiring manager mock"*, *"final mock"*, *"fluency drill"*.
2. Copy the prompt from the code block.
3. Paste it into a voice assistant:
   - **ChatGPT** app → voice mode
   - **Claude** app → voice mode
   - **Gemini** app → Gemini Live
4. Talk. The assistant stays in character and won't correct you mid-call.
5. Say **"feedback"**. You get fluency and content scores (each criterion backed by a quote), the top 2 fixes, one thing to repeat, and red flags.
6. Paste it back into Claude Code. Voice assistants tend to be generous; the coach re-checks against the quotes.

Can't talk right now? Say *"text mock"* and do it in the terminal.

**Scores:** fluency /10 (past tense, no word-for-word translation, short sentences, few fillers, main point first) and content /10 (fit, specifics, honesty, ownership, salary). Two mocks in a row with both ≥ 8 and no red flags = ready.

---

## Commands you can say

You don't need exact commands; plain language works. Some examples:

| Say | What happens |
|---|---|
| `/interview-prep` | Lists your jobs and the next step |
| "new job" / paste a job link | Starts intake for a new interview |
| "what's next?" | Next unchecked roadmap item |
| "HR mock" / "technical mock" / "final mock" | Generates a voice mock prompt |
| *(paste mock feedback)* | Scores, 2 fixes, updated notes |
| "fluency drill" | 15–20 min English speaking drill |
| "prep me for the technical round" | Stack questions, stories, kata or system design |
| "salary" | Market range, your number, pushback lines |
| "interview day" | Checklists for the hours before |
| *(paste the interview transcript)* | Debrief + follow-up email + next roadmap |
| "show my gaps" | Open questions about your experience |

---

## Rules the coach follows

- **English only** in coaching, so you practice the whole time.
- **Never invents** experience, numbers, titles or tools. Missing facts become questions.
- **Flags inconsistencies** (the same metric told two ways) and résumé items that aren't production experience.
- **Short answers**: 3–4 sentences, your words and motivation, no corporate filler.
- **Max 2 corrections at a time.**
- **Salary**: market research and a strategy to hold your number; never suggests lying about your current salary.
- **No live-interview cheating tools** (apps that listen to the call and feed you answers). Captions for accessibility and a paper sheet of topics are fine.
- **Never sends anything for you.** It drafts emails; you send them.
- **Take-home assignments**: helps plan and reviews, doesn't write the solution.

---

## FAQ

**Does it work for non-tech jobs?**
The method (intake, research, stories, mocks, debrief) works for any interview. The question bank and technical prep are tuned for software engineering.

**Does it need internet access?**
Research and job-post links need web access in Claude Code. Without it, paste the job text and the coach tells you what to look up.

**My interview isn't in English.**
Coaching stays in English; your answers, mocks and questions are generated in the interview's language.

**Can I use it for several jobs at once?**
Yes. Each job has its own folder and roadmap; `profile.md` is shared, so you confirm each story only once.

**Where's my data?**
Only in the `interview-prep/` folder on your machine, plus whatever Claude Code sends to the model during the session.

---

## Update

```bash
cd ~/.claude/skills/interview-prep && git pull
```

---

## Português (resumo)

Skill do Claude Code que prepara você para uma entrevista específica, em inglês.

1. **Instalar:** `git clone https://github.com/Mvcoladello/interview-prep-skill.git ~/.claude/skills/interview-prep`
2. **Usar:** crie uma pasta, abra o `claude` nela e digite `/interview-prep`. Passe o currículo (PDF ou texto) e o link da vaga.
3. Ela pesquisa a empresa e monta um roadmap pelo tempo que falta. Também gera uma cola (`notes.md`), perguntas sobre lacunas da sua experiência e prompts de mock para o modo de voz do ChatGPT, do Claude ou do Gemini.
4. Faça o mock por voz, diga **"feedback"**, cole o resultado no Claude Code e repita até tirar 8+ em fluência e conteúdo.
5. Depois da entrevista, cole a transcrição: você recebe a análise, um e-mail de follow-up e o roadmap da próxima etapa.

O coach fala só em inglês e nunca inventa experiência ou números. Seus dados ficam na pasta `interview-prep/`; não suba essa pasta para um repositório público.

---

## License

MIT
