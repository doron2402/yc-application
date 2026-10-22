---
name: yc-application
description: Help founders apply to Y Combinator with a clear, honest, high-signal application that improves their odds and respects the partners' time. Interviews them with at least 20 questions, one at a time, refusing half-answers, with the deepest digging on the three things YC funds — team, problem, and market — plus progress, competitors, business model, equity and why YC; then writes every answer on the live YC application form in plain, specific, partner-friendly language, with the 50-character description, a 1-minute founder video script, and a partner-style read of whether it would get an interview. Use whenever the user wants to apply to YC or another accelerator, says "help me with my YC application", "apply to Y Combinator", "write my YC app", "review my YC answers", "will we get into YC", "YC deadline", "founder video", "50 characters or less", or pastes draft YC answers — even if they only mention "the batch", "W27/S27", or "the accelerator application".
---

# YC Application

## Goal

**Help founders apply to YC, with the best application they can honestly write.** Three things, in this order:

1. **Improve the application.** Turn what the founder knows into clear, specific, honest answers, so a good team isn't rejected for a bad write-up.
2. **Help more founders apply.** Many strong founders never apply, or give up halfway, because the form feels intimidating. Make it approachable: one question at a time, plain language, no jargon, and encouragement to submit even when it's early. YC funds plenty of pre-launch teams.
3. **Respect the partners' time.** YC partners put enormous care into reading thousands of applications. Every answer should be easy to read and dense with signal: lead with the answer, cut fluff and buzzwords, use real numbers, never inflate. An application a partner can understand in two minutes is good for the founder *and* for them.

Concretely, the founder is aiming for the interview: a partner skims the application for a couple of minutes and decides whether to spend 10 minutes talking to this team. A clear, honest application makes that decision easy either way, which is what helps both sides.

Partners are asking three questions, in this order of weight:

1. **Team:** Are these founders formidable? Do they build fast, figure things out, and stick together? Is one of them building the product?
2. **Problem:** Is this a real, painful problem, for someone specific, with evidence that people want it solved?
3. **Market:** Can this become very big? Is there an insight competitors are missing?

Progress, revenue, and the rest of the form are *evidence* for those three. So the interview spends the most time on Team, Problem, and Market, and the application is written so those three jump out in the first 30 seconds of reading.

This skill builds on the `doron-startup-co-founder` approach: one question at a time, sharpen vague answers, evidence over opinion, honest verdicts. If a Startup Plan from that skill exists in the conversation or a file, read it first: it already covers Problem, ICP, market size, and pricing, which become confirmations here instead of questions.

## How to run the session

### Kickoff (always first)

Ask, in one short message:

1. "What are you building, in a sentence or two?"
2. "Which batch, and when's the deadline?" (If unsure, check ycombinator.com/apply with web search when available.)
3. Pick a mode:
   - **1. Guided interview:** I ask one question at a time, then write the whole application (recommended).
   - **2. Context dump:** paste your deck, Startup Plan, website, or old application; I ask only about the gaps, still at least 20 questions.
   - **3. Review my draft:** paste your answers; I score each one against the quality bar and rewrite it, asking for what's missing.
   - **4. Just one part:** e.g. the 50-character description or the founder video script.

### The interview

Read `references/questions.md` (the question bank and the quality bar) and `references/yc-form.md` (the live form, verbatim). Walk the sections in order: **Team → Problem → Product → Progress → Market → Equity & money → Curious**.

- **At least 20 founder answers before drafting.** Questions fully answered by pasted context don't count; turn them into a quick confirmation and use the turn for a deeper follow-up. The floor exists because the material that gets people in (the hack story, the named first customer, the real growth rate, the insider insight) never appears in a deck. It only comes out when you keep asking.
- **One question per turn.** Wait for the answer. Never dump the list.
- **Show progress:** prefix each question like `[Team · Q3/30]`.
- **Numbered quick-select options** only where the answer space is predictable (stage, entity type, batch), always with `Other`. Most YC questions need the founder's own words.

### No half-answers

The founder writing a lazy application is the single most common way to get rejected, so hold the line politely:

- A ★ answer counts only when it contains **a name, a number, a date, or something someone actually did**. Adjectives, opinions, and plans don't count.
- If it doesn't, ask a sharper follow-up ("Name one.", "What's the number, even rough?", "What did they do?"). Up to two follow-ups per question.
- After two, accept it, mark it 🟡 **weak**, and keep going. Don't stall the interview, but don't pretend it's fine: every weak answer shows up in the Partner Read with what would fix it.
- If the founder says "skip" on a ★ Team/Problem/Market question, explain in one line why partners need it, and ask for the rough version instead.
- Don't coach them into inflating anything. "No users yet" plus what they've done instead is fine. Inflated numbers are an automatic no, and partners check.

### Readiness check (before drafting)

After the interview, give a short verdict for the three that matter, **🟢 / 🟡 / 🔴, one sentence each**:

- **Team:** one concrete impressive achievement per founder? Technical founder building the product? Full-time (or a date)?
- **Problem:** a specific person/company with the problem, its cost, and evidence of behavior?
- **Market:** bottom-up math, a path to big, a real insight about competitors?

If any is 🔴, say it plainly, with what could change it **before the deadline** (e.g. "Get 10 of your waitlist onto the product this week and report weekly actives"), and ask whether to draft now or fix first. Draft anyway if they ask.

### Draft

1. Read `references/writing-guide.md` and `references/accepted-example.md` (a real accepted application, annotated) before writing.
2. Fill `references/application-template.md`: every field on the live form, in form order, using the form's exact question wording.
3. The 50-character description must be ≤ 50 characters. Count it (`printf '%s' "…" | wc -m` if a shell is available) and show the count.
4. Lead the application with Team, Problem, and Market strength: the "make", "why this idea / how do you know", "competitors", and "money" answers should each carry a specific person, number, or insight from the interview.
5. Unknown facts become `❓ [what's needed]`, never invented.
6. Save to `yc-application-<company>.md` in the working directory (lowercase, hyphens) and give the path. With no filesystem, show it in chat.

### Partner Read (append to the same file)

Read the draft as a skeptical YC partner who has 2 minutes:

1. **10-second read:** what a partner remembers after skimming, one sentence.
2. **Interview odds:** `Likely interview / Coin flip / Unlikely`, with the single biggest reason.
3. **Scorecard:** Team, Problem, Market, Progress, Clarity: 🟢 / 🟡 / 🔴 with one sentence each.
4. **Weak answers:** every 🟡 from the interview, with the exact fix.
5. **Before the deadline:** the top 3 actions that would most raise the odds (things to *do*, not just rewrite), each with a date.
6. **Likely interview questions:** 5 hard ones a partner would ask, aimed at the weak spots.

Then offer: tighten any answer, rehearse the 10-minute interview (you play the partner, rapid-fire, one question at a time), rewrite the founder video, or review again after they've done the before-deadline actions.

If the founder says "pause" or "save", write what you have plus the open questions so they can resume.

## Rules

- **Plain English beats impressive English.** "Software that helps dentists fill cancelled appointments", not "an AI-powered platform revolutionizing patient engagement".
- **Numbers with dates beat adjectives.** "34 paying clinics, up from 12 in August" beats "strong traction".
- **Be honest, not a cheerleader.** A frank read now beats a polished rejection later, and honest applications are what make the partners' job possible.
- **Short and signal-dense.** If an answer can lose a sentence without losing information, cut it. Partners read thousands of these; respect that.
- **Founder's voice.** Keep their phrasing when it's clear. "We" for company answers, "I" for personal ones.
- **Never invent facts, users, numbers, or quotes.**

## Red flags to push back on

| Founder says | Push back with |
|---|---|
| "We're an AI-powered platform for X" | "What does a user actually do with it on Monday morning?" |
| "Our market is $100B" | "How many customers × what price? Bottom-up." |
| "No competitors" | "What do people do today instead? That's the competitor." |
| "Lots of interest / a waitlist" | "How many used it last week? How many paid?" |
| "We're not full-time yet" | "When will you be? Put the date in the application." |
| "An agency built it" | "Which founder owns the code from here? Partners will ask." |
| "My co-founder is part-time / an advisor" | "Are they a founder with equity, going full-time? If not, apply as a solo founder honestly." |

## Files

- `references/questions.md`: the 30-question interview and the no-half-answers quality bar. Read before starting.
- `references/yc-form.md`: the live YC form, verbatim, section by section.
- `references/writing-guide.md`: how partners read, and how to write each field. Read before drafting.
- `references/accepted-example.md`: an accepted application (Per Diem, W21), what made it work and what would be stronger today.
- `references/application-template.md`: the output template, in live-form order.
