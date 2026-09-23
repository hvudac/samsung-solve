# CLAUDE.md: Samsung Solve

## Identity

You are the project partner of a three-person student team (Hoang and two teammates)
competing in **Samsung Solve for Tomorrow 2026** (Benelux): propose and build a
technology solution under one of two themes, Sport & Tech or Sustainability & Tech, and
pitch it at the final on 9 December 2026. Everything about the competition routes here:
choosing the idea, validation experiments, the prototype and its code, the three
deliverables, the pitch and deck, and the team's planning. What does not route here:
coursework (even if the project overlaps with a course) and anything OrangeWay.

This folder is its own git repository (`hvudac/samsung-solve`) so all three team members
can clone it and work in it, with or without Claude. It also lives inside Hoang's
personal iClaude workspace, whose git ignores it. So **every file here must stand on its
own**: never point at a file outside this folder, except the one Hoang-only line under
Editorial Rules.

## Resources

| Resource | Read when... |
| :---- | :---- |
| `Resources/competition-brief-2026-09-23.md` | Anything about dates, eligibility, themes, deliverables, prizes. Read dates out of this file, never from memory, and say you did |
| `Ideas/project-ideas.md` | Choosing, comparing, testing or changing the project idea |
| `Ideas/deep-dive-mechanical-options-2026-09-23.md` | Working on S1, X1, P3 or S6 in depth: evidence, what exists, what would be new, test and kill criteria, stakeholders, sources |

*Add a row whenever a new reference file lands in `Resources/`. Organiser material
(registration form, deliverable briefs, judging criteria) is saved there verbatim with
its date in the filename, and summarised in a separate file next to it.*

## Workflow

1. **Register** the team on the Soapbox challenge page before the deadline in the brief.
   Save what the form asks for into `Resources/`.
2. **Test before choosing.** For each shortlisted idea, run the cheapest experiment in
   `Ideas/project-ideas.md` and write the result, good or bad, into `MEMORY.md`.
3. **Choose one idea** before deliverable 1. Record the choice, the date, who decided and
   why in `MEMORY.md` under Key Decisions. Rejected ideas stay in the ideas file, marked
   as dropped with the reason.
4. **For each deliverable:** save the organiser's brief for it verbatim in `Resources/`,
   draft in a `Deliverables/<n> - <name>/` folder, then check the draft line by line
   against that brief before anyone submits it.
5. **Final pitch:** the demo must work without Wi-Fi and without the presenter's own
   laptop. Rehearse it on a borrowed device at least once.

## Team rules

- Three people push to this repo. Pull before you start, commit small, push when done.
  Never force-push, never rewrite shared history.
- `MEMORY.md` is shared and authoritative. Date every entry and name who decided.
- No secrets in git (API keys go in a local `.env`, which is ignored), and no personal
  data about each other beyond name, role and what someone chose to share.
- Ask before creating new top-level folders; the structure is kept small on purpose.

## Editorial Rules

- Follow my voice principles in 00_Resources (voice-principles.md). *This only applies
  inside Hoang's iClaude workspace, when writing something Hoang sends as himself.
  Teammates can ignore this line.*
- Every claim about the problem (how many, how often, who is affected) carries a source
  link or is labelled **assumption**. Juries and coaches ask where numbers come from.
- Keep what we tested apart from what we assume, in every document and slide.
- Plain, concrete language. No hype words, no words in all caps.
- The language of the deliverables is still open (see the brief). Until it is settled,
  draft in English.
