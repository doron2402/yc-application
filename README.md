# yc-application

A [Claude Code](https://claude.com/claude-code) skill that helps founders **apply to Y Combinator with the best application they can honestly write.**

- **Better applications:** good teams shouldn't be rejected for a bad write-up.
- **More founders applying:** one question at a time, plain language, so the form stops feeling intimidating.
- **Respect for the partners' time:** YC partners put huge care into reading thousands of applications. Clear, short, honest, number-backed answers make their job easier, and that's what helps you most too.

It interviews you like a co-founder who has read a thousand YC applications: **at least 20 questions, one at a time, no half-answers.** Every key answer needs a name, a number, a date, or something a real person did. Then it writes every answer on the live YC form.

It digs deepest on what YC actually funds:

1. **Team**: what each founder has built, how long you've worked together, who writes the code
2. **Problem**: a specific customer, what it costs them today, evidence they want it solved
3. **Market**: bottom-up sizing, competitors, and the insight they're missing

…then covers progress, revenue, equity, and why YC.

You get:

- Every field on the current YC application, in form order, in plain and specific language
- A 50-character description (counted)
- A 1-minute founder video script
- A **Partner Read**: interview odds, a Team / Problem / Market scorecard, weak answers with exact fixes, the top 3 things to *do* before the deadline, and the 5 interview questions you'll likely get

It was written by a founder whose company (Per Diem) went through YC W21, and it includes that accepted application, annotated, as a reference.

## How it works

1. **Kickoff:** what you're building, which batch, and a mode: guided interview, context dump (paste your deck or an old application), review my draft, or just one part.
2. **Interview:** 20+ questions, one at a time, in the order YC weighs them: **Team → Problem → Product → Progress → Market → Equity → Why YC**. Vague answers get a sharper follow-up ("Name one.", "What's the number?", "What did they do?").
3. **Readiness check:** Team, Problem, and Market each get 🟢 / 🟡 / 🔴 before anything is written, with what to fix before the deadline.
4. **Draft:** every field on the live form, in YC's own wording, saved to `yc-application-<company>.md`.
5. **Partner Read:** a skeptical 2-minute read of your application, plus an offer to rehearse the 10-minute interview.

## Example: the 50-character description

| Before | After |
|---|---|
| "Per Diem is a subscription ecommerce platform." | "Subscriptions for local shops, no code needed" (45) |

The "after" says who it's for and doesn't spend characters on the company name.

## Install

```bash
npx yc-application
```

This copies the skill to `~/.claude/skills/yc-application`, so it's available in every project.

```bash
npx yc-application --project   # install into ./.claude/skills (this project only)
npx yc-application --force     # overwrite an existing install (e.g. to update)
```

Prefer a manual install? Copy `SKILL.md` and `references/` into `~/.claude/skills/yc-application/`.

## Use

Start a new Claude Code session and say something like:

- "Help me with my YC application"
- "We're applying to YC W27, interview me"
- "Review my YC answers" (and paste them)
- "Write our 50-character description"
- "Script our YC founder video"

Modes: **Guided interview**, **Context dump** (paste your deck or old application), **Review my draft**, or **Just one part**. Say "pause" any time to save progress.

Pairs well with [`doron-startup-co-founder`](https://www.npmjs.com/package/doron-startup-co-founder): its Startup Plan feeds straight into this skill.

## Files

- `SKILL.md`: how the session runs
- `references/questions.md`: the 30-question interview and the quality bar
- `references/yc-form.md`: the live YC form, verbatim
- `references/writing-guide.md`: how partners read and how to write each answer
- `references/accepted-example.md`: an accepted application (YC W21), annotated
- `references/application-template.md`: the output template

YC changes its form between batches. If yours looks different, paste it in and the skill will follow it.

## Contributing

Issues and PRs welcome, especially when YC changes the form. Update `references/yc-form.md` and open a PR.

Not affiliated with or endorsed by Y Combinator.

## License

MIT
