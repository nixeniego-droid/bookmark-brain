# Sort — file each new save under the right interest

Run after every pull. Read the vault's `AGENTS.md` first.
For a big first sort, go in batches of about 100 and save after each batch.

1. Read every `interests/<slug>/PROMPT.md` so you know what belongs where.
2. For each note in `raw/` with no `interest:` (or `interest: unsorted`):
   - choose the **one** best-fitting interest → `interest: <slug>`; add `also: <slug>` for a clear runner-up
     (a matching X bookmark folder name wins)
   - set `topics:` to 1–3 slugs from `.xbrain/config.json` — never make one up
   - fill `summary:` (one plain sentence), `kind:`, `value:` (1–3), and `action:` only when value is 3
   - leave the note's body and `status:` untouched — notes never move, only their frontmatter changes
   - nothing fits? `interest: other`
   - add a line for it at the top of `## All saves` in `interests/<slug>/<slug>.md`
3. If 5+ `other` notes share a theme, suggest a new interest to the owner. Don't create it without a yes.
4. For each interest that got new saves, rewrite its compiled block following its `PROMPT.md`.
5. Update `index.md` and append to `log.md`.
6. Report how many went to each interest and how many to `other`.
