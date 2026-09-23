# Samsung Solve for Tomorrow 2026: team workspace

Shared workspace for our team's entry in
[Samsung Solve for Tomorrow 2026](https://www.samsung.com/nl/explore/brand/solve-for-tomorrow/)
(Benelux). Everything is plain Markdown, so it works in any editor, in Obsidian, or with
Claude.

## Start here

1. `Resources/competition-brief-2026-09-23.md`: the rules, themes and every date.
2. `Ideas/project-ideas.md`: six project ideas, each with the cheapest test that would
   tell us if it is worth building, and a recommendation.
3. `MEMORY.md`: where we are, what we decided and why, and what is still open. Add your
   name and strengths under Contacts.

## Working together

```bash
git clone https://github.com/hvudac/samsung-solve.git
cd samsung-solve
git pull            # before you start
git add -A && git commit -m "what changed" && git push   # when you are done
```

Never force-push. If a push is rejected, `git pull --rebase` and push again.

## Using it with Claude

Open this folder as the working folder in Claude (Cowork or Claude Code). `CLAUDE.md`
tells Claude how to behave here: read dates from the brief, keep tested facts apart from
assumptions, log decisions in `MEMORY.md`.
