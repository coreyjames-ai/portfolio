# Facebook Page provider



Canonical: https://coreyjames.ai/tools/facebook/  
Author: Corey James · Published: 2026-10-28 · Kind: tool group  
Systems: [FAFOHive](https://github.com/coreyjames-ai/fafohive)  

## What was built

A business's Facebook Page is its storefront, and an agent that runs one has to cover the whole life of a post: publish it, answer the comments, handle the messages, measure it and clean up after it. I built this provider as my own MCP server over the Meta Graph API. It keeps its own register of everything it created, so delete tools only ever touch the Page's own posts, media and comments. Writes are read back before they are reported. Incoming comments, messages, mentions and reviews are collected into a local inbox, and Graph usage and permission health are visible to the agent before it hits a limit.

## Posts and publishing

`fb_publish_post` publishes a Page post as text, a link, one or more photos, a video or a reel.

`fb_schedule_post` creates a Facebook-native schedule for a post and its media.

`fb_edit_post` corrects a post's text, changes its visibility or moves a scheduled publication.

`fb_list_posts` lists published and scheduled posts, or shows one post with its engagement.

`fb_delete_own_post` deletes a post the provider published, or cancels its schedule, then checks what media remains.

`fb_tagged` finds posts that tag the Page and the Page's reviews within a date range.

## Media

`fb_upload_media` uploads an unpublished photo for later use in posts, comments or the Page's profile and cover images.

`fb_list_media` lists the Page's photos, videos and reels and the processing state of each.

`fb_delete_own_media` deletes a photo, video or reel the provider created and confirms it is gone.

## Comments and moderation

`fb_comments` reads the comments on one post or object, or finds unanswered comments across recent posts.

`fb_reply_comment` answers a comment or review publicly as the Page, or sends the commenter a private message.

`fb_moderate_comment` moderates one comment.

- `hide` and `unhide` hide or restore a visitor's comment.
- `like` and `unlike` like a comment as the Page or remove that like.
- `delete_own` deletes a comment the Page itself wrote.

## Messenger inbox and events

`fb_inbox` lists Messenger conversations or opens one, including how long the reply window has left.

`fb_inbox_send` acts in an existing Messenger conversation.

- `send` sends a reply with text, an attachment or both.
- `mark_read` marks the conversation read.
- `typing_on` and `typing_off` show or clear the typing indicator.

`fb_events` reads collected comments, messages, mentions and reviews that are waiting for attention.

`fb_event_mark` records how one event was handled: answered, ignored or failed.

`fb_engagement_report` measures how quickly the Page handles incoming engagement, from the local event records.

## Page and analytics

`fb_page_info` reads the Page's public profile and, optionally, its events.

`fb_page_update` updates the Page's description, contact details or profile and cover images, and reads them back.

`fb_insights` returns engagement counts and the available Insights for the Page, a post or a video.

`fb_usage` shows Graph API usage, write settings, permission health and event-ingestion errors.

## Events to other systems

`fb_webhook_subscribe` sends Facebook events to an outside listener, signed and filtered by event type.

`fb_webhook_list` lists those listeners and their delivery failures.

`fb_webhook_remove` turns a listener off and keeps its history.

Ownership is what I designed this around. An agent can run a Page end to end and still cannot delete anything a person posted.

## What was verified

Each line is a claim the canonical page supports, with the figure as the page states it.

- Social platform integration: 24 tools on my own MCP server over the Meta Graph API let an agent publish, schedule, edit and measure Page posts and answer comments and messages.
- Safe automation design: a register of everything the provider created limits deletes to the Page's own content, writes are read back before they are reported, and Graph usage is visible before a limit is hit.

## Related

- System: [FAFOHive](https://github.com/coreyjames-ai/fafohive)

## Citation

Corey James. "Facebook Page provider." coreyjames.ai, 2026. https://coreyjames.ai/tools/facebook/

```bibtex
@misc{coreyjames-facebook,
  author = {Corey James},
  title = {Facebook Page provider},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/tools/facebook/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/tools/facebook}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
