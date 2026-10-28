# X provider



Canonical: https://coreyjames.ai/tools/x/  
Author: Corey James · Published: 2026-10-28 · Kind: tool group  
Systems: [FAFOHive](https://github.com/coreyjames-ai/fafohive)  

## What was built

I needed agents that could research conversations on X and take part in them, and the existing options did not fit. X's official API covers only some of what a campaign needs, research reads are metered, and a social account is easy to damage with careless automation. So I built my own X provider as two MCP servers behind the [FAFOHive](https://coreyjames.ai/systems/fafohive) hub. One holds 21 tools that research, read and report. The other holds 15 tools that act on the account, and it is authorised separately, so an agent can be given research without being given the account. Underneath is a hybrid backend: a commercial X data API for public research, the official X API for account operations and activity webhooks, and a bridge into my existing logged-in browser for the routes the official API does not serve. Each acting tool takes an explicit mode that names which route it uses. Every write is read back from X before it is reported as done, every collected response is stored locally, and reports over stored data cost nothing.

## Research

`x_find_live_threads` finds and ranks fresh threads from given queries or from a configured campaign lane, with authors, provenance and the actual cost of the search.

`x_find_lookalikes` explores the followers or following of chosen seed accounts, filters the profiles and ranks candidates by overlap with the seeds.

`x_profile_accounts` looks up a batch of accounts, with optional samples of their recent activity.

`x_pulse_hashtags` samples recent activity on a set of hashtags: volume, engagement, co-occurring tags and visible spam or sensitive signals.

`x_scan_lane` surveys a campaign lane or a set of queries for threads, accounts, hashtags and activity patterns, and stores what it reads.

`x_trend_phrase` compares how often a phrase was seen across days, and extrapolates only when the data supports it.

`x_trends` compares changes in stored post metrics and in phrase and hashtag sightings.

`x_watch_conversation` refreshes a known conversation's metrics, replies and quotes and reports what changed since the last look.

`x_list_lanes` lists the configured campaign lanes with their queries and blocklists.

## Our account and its inbox

`x_list_our_posts` lists the account's own posts, replies and quotes from stored records or fresh reads, with proof of ownership.

`x_inbox_mentions` collects mentions, replies and quotes of the account's recent posts.

`x_inbox_messages` reads direct messages with one person and stores new incoming messages as events.

`x_events` reads the local inbox of incoming events, with filters and paging, at no cost.

## Reports from stored data

`x_history` returns the stored time series for one post, account, hashtag or phrase.

`x_lane_report` compares the conversations collected in a campaign lane with the account's own activity there.

`x_performance_history` compares stored metric curves of the account's posts by variant, lane and posting hour.

`x_report_our_performance` refreshes a bounded sample of the account's posts and reports rankings and totals, joined with campaign plan data.

`x_engagement_report` reports inbound event counts, handling status, delivery health and recent polling failures.

`x_credit_report` reports metered usage, the remaining allowance, the budget gates and the polling estimates, without calling X.

`x_export_observations` exports collected observations as CSV or JSONL.

`x_queue` shows the local action queue: what is scheduled or was sent, in which mode, with outcomes, errors and costs.

## Acting on the account

`x_post` publishes an original post with optional media, then reads it back to confirm author and text.

`x_reply` replies to a chosen open thread, confirms the author, parent and text, and can follow the author.

`x_quote` quotes a post with commentary and optional media, then confirms the quoted post and media.

`x_delete_post` deletes one of the account's own posts after checking ownership, then confirms it is gone.

`x_like` likes one chosen post.

`x_unlike` removes the account's like from one post.

`x_follow_batch` follows a list of accounts at a measured pace, with an outcome stored for each.

`x_unfollow` unfollows a list of accounts and confirms each follow is gone.

`x_dm_outreach` prepares a checked preview of a direct message to named recipients, and sends only against that preview's receipt.

`x_schedule` stores a future post, reply or quote with its mode, to be sent later.

`x_queue_cancel` cancels a queued action before it is sent.

`x_event_mark` marks an incoming event as answered, ignored or failed, with optional notes.

## Events to other systems

`x_webhook_subscribe` routes normalized social events to an HTTPS listener, signed.

`x_webhook_list` lists those subscriptions and their delivery counts.

`x_webhook_remove` removes a subscription and cancels its pending deliveries.

The split between reading and acting, the explicit route on every write and the read-back after it are what make it safe to hand this account to an agent.

## What was verified

Each line is a claim the canonical page supports, with the figure as the page states it.

- Social research and engagement for AI agents: 36 tools on two MCP servers, 21 that research, read and report on X conversations and 15 that act on the account.
- Least privilege for AI agents: the acting server is authorised separately, so an agent can be given research without being given the account.
- Hybrid API integration: a data API for research, the official API for account operations and webhooks, and a browser bridge for the rest, with every write read back before it is reported.

## Related

- System: [FAFOHive](https://github.com/coreyjames-ai/fafohive)

## Citation

Corey James. "X provider." coreyjames.ai, 2026. https://coreyjames.ai/tools/x/

```bibtex
@misc{coreyjames-x,
  author = {Corey James},
  title = {X provider},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/tools/x/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/tools/x}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
