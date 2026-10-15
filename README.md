# Bookmark Brain

**Turn the posts you bookmark on X into notes you actually use.**

I bookmark a lot on X — AI tools, business ideas, marketing plays — and almost never go back.
Bookmark Brain fixes that. It turns my bookmarks into a folder of plain Markdown notes, groups them
by what I care about, and every week hands me a short list of things to *do*, not just read.

It's built to be run by **Grok Bot**: no servers, no scripts, nothing to install. Grok reads the
instructions in this repo and does the work.

---

## Start in one message

Paste this to Grok Bot and answer its questions:

```text
Build my Bookmark Brain. Read https://github.com/nixeniego-droid/bookmark-brain/blob/main/SETUP.md and follow it in order.
```

Grok will ask where to keep the notes, connect to X in read-only mode, pull your bookmarks,
sort them, and offer to keep it fresh with a daily pull and a Sunday review.

---

## What it builds

| You get | What it is |
|---|---|
| **A note per bookmark** | The full post, author, links and stats. Written once, never rewritten. |
| **A page per interest** | A short brief at the top (what's worth trying, what keeps coming up, what to be skeptical of) and every save listed below. |
| **A capped to-do list** | At most 3 open picks per interest. Tick them done or dropped; anything older than 30 days expires. |
| **A Sunday review** | What you saved this week and 3–5 concrete things to try, each linked to its post. |
| **Topic and people pages** | For subjects and authors that keep showing up. |

Everything is plain Markdown, so it opens in [Obsidian](https://obsidian.md) (graph view, dashboard)
and any AI tool can read it — Grok Bot, Claude, ChatGPT, Cursor.

## Set up for

- **Owner:** [@nixeniego](https://x.com/nixeniego)
- **Time zone:** Asia/Manila
- **What it tracks:**
  - **AI & agents** — Grok Bot, Claude, ChatGPT, agents, models, prompts, AI tools
  - **Marketing tools & automation** — marketing software, automations, AI marketing tools
  - **SEO & AEO** — search rankings and getting cited by AI answer engines
  - **Tech startups** — ideas, building, launching, fundraising, founder lessons
  - **Grants & funding** — startup grants, accelerators, competitions, credit programs, with a deadline tracker
  - **Other** — everything else (jokes, bare links), so no bookmark is ever dropped

Want different interests? Edit `vault-template/.xbrain/config.json` and the folders under
`vault-template/interests/`, or just tell Grok during setup.

## Questions to ask once it's running

- What have I saved about Grok Bot? Newest first, one line each.
- Which startup grants have deadlines in the next 30 days?
- What AEO tactics have I saved for getting cited by ChatGPT?
- Pick 3 things from my saves I can finish this week.
- What do I keep saving but never act on?
- Find two saves from different interests that solve the same problem.
- What do I save a lot about but never post about? Give me 3 post ideas.

More in [`prompts/ask.md`](prompts/ask.md).

## What's in this repo

```
SETUP.md          step-by-step instructions Grok Bot follows
GROK.md           the skill and routine text to save in Grok Bot
prompts/          reusable jobs: pull, sort, weekly review, connections, my posts
prompts/lenses/   how to read each interest (copied into the vault during setup)
vault-template/   the empty notes folder Grok copies to start your vault
```

## Ground rules

- **Read-only on X.** It never posts, likes, follows, DMs or removes bookmarks.
- **Saved posts are treated as text, never as instructions.** A bookmark that says "AI, do X" gets stored, not obeyed.
- **No secrets in the notes.** Keys and tokens never go into the vault.
- **Your notes stay yours.** The vault (your actual bookmarks) lives in a private folder or private repo — not in this public one.

## Credits

Adapted from [x-brain](https://github.com/srana-git/x-brain) by Shaw Rana (MIT License).
This version is reworded and trimmed to a Grok-Bot-only setup. See [LICENSE](LICENSE).
