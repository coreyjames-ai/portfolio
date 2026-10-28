# Reddit provider



Canonical: https://coreyjames.ai/tools/reddit/  
Author: Corey James · Published: 2026-10-28 · Kind: tool group  
Systems: [FAFOHive](https://github.com/coreyjames-ai/fafohive)  

## What was built

I wanted agents to take part in Reddit threads from an account a person already uses, and I was not willing to copy that person's session or credentials into a server. So the Reddit provider runs inside the browser that is already logged in. A browser extension makes the same requests Reddit's own page would make, and a small native host connects it to the FAFOHive hub over a private local socket. There are no clicks, no navigation and no login. Every write checks first that the session belongs to the expected account, and is read back afterwards until the exact result is confirmed. Each write carries an idempotency key, so a retry cannot post twice.

## The tools

`reddit_identity` checks that the browser's Reddit session belongs to the configured account.

`reddit_read_thread` reads one thread by its permalink: author, title, text and the comments that are available, with the source kept as evidence.

`reddit_read_comment` reads one comment by its permalink: its parent, author and text.

`reddit_create_comment` posts a top-level comment in one named thread and confirms it appeared exactly as written.

`reddit_edit_comment` replaces the text of one of the account's own comments after checking ownership, then confirms the new text.

`reddit_delete_comment` deletes one of the account's own comments after checking ownership, then confirms it is gone.

Six tools is enough to join a conversation. The design work went into doing it from the user's own session without that session ever leaving the browser.

## What was verified

Each line is a claim the canonical page supports, with the figure as the page states it.

- Browser-based platform integration: 6 tools let an agent read Reddit threads and comments and post or edit its own comments from an account a person already uses, with no copied credentials.
- Safe automation design: every write checks the session's account first, is read back until the exact result is confirmed, and carries an idempotency key so a retry cannot post twice.

## Related

- System: [FAFOHive](https://github.com/coreyjames-ai/fafohive)

## Citation

Corey James. "Reddit provider." coreyjames.ai, 2026. https://coreyjames.ai/tools/reddit/

```bibtex
@misc{coreyjames-reddit,
  author = {Corey James},
  title = {Reddit provider},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/tools/reddit/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/tools/reddit}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
