# Pull — bring new bookmarks into the vault

Run daily (or whenever). Read the vault's `AGENTS.md` first.

1. Read the owner's X bookmarks, newest first, with the X plugin (read only).
   - Use a page size of **50**. Asking for 100 returns 99 posts and drops the next-page token.
   - Ask for the full text of long posts, plus links, media and metrics.
   - If the owner uses bookmark folders on X, note each post's folder — it helps sorting.
2. Stop at the first post that already has a note in `raw/` (match on `id:`). On the very first
   pull, read as far back as X allows (or as far as the owner agreed to pay for).
3. For each new post, write one note using the format in `SETUP.md` Step 5:
   - copy the post text exactly; for a thread by the same author, add the following posts below it
   - mark images and videos as `[image]` / `[video]`
   - if it links to an article, include the link and the article title
   - write `summary` fresh for this post: what it gives the owner, not a copy of its first line
4. Don't open DMs or read anything beyond the bookmarks and the posts they point to.
5. Report: how many new saves, and the oldest and newest dates among them.

Then run `sort.md`.
