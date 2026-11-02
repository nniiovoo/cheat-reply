---
name: cheat-reply
description: Research X/Twitter posts and their replies, find relevant conversations, and draft concise replies in the user's voice. Use for reply targets, comment research, reply drafting, or reply growth strategy. Study actual comments before writing; posting requires approval of the exact text and target.
license: MIT
metadata:
  version: "0.1.0"
  maintainer: nniiovoo
---

# Cheat Reply

Learn what works in a conversation before joining it. Find relevant posts, study their replies, and write one specific contribution in the user's voice.

This skill is for replies. Use a separate workflow for original posts, engagement predictions, or post-performance calibration.

## Choose the mode

- **Learn:** study posts and comments; record useful observations without drafting or posting.
- **Draft:** research the conversation and propose a reply. This is the default.
- **Post an approved reply:** publish only the exact text to the exact target the user has approved, then verify the result. A learning or drafting request does not authorize posting.

Use the user's topic, target, audience, and constraints when supplied. Otherwise infer what is clear from the request and ask only for missing information that affects the work. Do not assume a crypto audience or an aggressive voice.

## Load only useful context

If present in the user's working project:

1. Read the current rules and latest five cases in `reply-learnings.md`.
2. Read only the voice and audience sections of `audience.md` when needed.

These files are optional. Without them, use the user's stated voice and audience; do not invent a persona or performance history. Blank starting points are in [examples](examples/). Keep the user's real notes in their project, outside this installed skill.

Read [the playbook](references/reply-playbook.md) for strategy, repeated underperformance, or skill maintenance. Ordinary single-reply work does not need the full playbook.

## Find worthwhile conversations

For discovery, weigh:

- **Audience fit:** would the people reading this care about the user's work or interests?
- **Timing:** a fresh post from an established account can have few views because it is still early. For an older post, look for demonstrated ongoing activity.
- **Visible competition:** a relevant conversation with room to contribute can be more useful than a crowded viral thread.
- **Context:** read the complete post, expand hidden text, and inspect relevant media before committing to an angle.

Use specific topics, accounts, or phrases rather than a broad search that mixes unrelated audiences. Crypto and AI examples include `Claude Code`, `DeepSeek funding`, `Hyperliquid`, or `Bitcoin energy`; adapt the search to the user's niche. If X search filters fail, simplify the query.

The original workflow used roughly 100K post views or 1K likes as research heuristics for established posts, and tried to arrive within the first 20–30 replies. Treat those as starting points to test, not platform rules or guarantees. The user's supplied target takes precedence over a discovery heuristic.

## Learn before writing

For the target, inspect relevant or top replies and note what receives attention:

- Is the useful contribution a punchline, concrete question, counterexample, explanation, or personal experience?
- Does it agree, challenge, extend, or clarify the original post?
- What makes it specific to this conversation?

When the target's replies are too fresh or sparse, study one active post on the same topic. Reuse a pattern across a closely related batch only when the context still fits. Learn the mechanism; do not copy another person's wording.

Use available browsing or approved computer-use tools. If comments are inaccessible, ask the user to paste the post and a few relevant replies. State what you could inspect; do not invent comment evidence, engagement counts, or a winning pattern.

## Draft one strong reply

Start with one candidate. Offer alternatives when the angle genuinely branches or the user asks.

- Make one point, using a concrete detail from the post.
- Match the user's voice and the conversation. Short and dry can work; thoughtful technical discussions may need an explanation or a precise question.
- For builder posts, keynotes, or essays, add something that shows you read the material. Generic praise and a forced joke add little.
- Use the author's wording only when it supports a natural extension or reversal.
- Keep slang, emoji, and links purposeful. Avoid repetitive emoji, padded caveats, stock aphorisms, forced contrasts, and a formulaic three-part conclusion.
- A serious market reply can connect a signal to a mechanism and a time window, when that is relevant and supported.
- Never fabricate the user's experience, qualifications, results, conversations, or insider access. Ask for a real detail when it is essential.

Keep drafts concise. Before posting, check the current composer's limit; do not assume every account or format has the same limit. Without composer access, do not claim that you verified the platform's current limit.

Show the target link/account when available, a short reason it is worth joining, what you observed in the comments, and the proposed reply. For pasted material without a link, identify the supplied post; a missing URL does not prevent drafting. Keep research notes outside the copyable reply. Separate observations from your interpretation.

## Record useful learning

When learning is requested or a reusable observation emerges, add a compact entry to the user's project notes:

```markdown
| Date | Topic/target | Observed reply pattern | Evidence/limitation | Lesson |
|---|---|---|---|---|
```

Save a short paraphrase and a source link where useful. Do not archive private messages or long copied comments. Periodically merge repeated cases into the current rules. Keep observations distinct from proven causes of engagement; this workflow does not predict results.

If the user also maintains blind main-post predictions, keep their pending metrics out of reply research. Reply work does not enter that scoring or prediction loop.

## Publish only approved text

Use an available, authorized posting tool or a browser already signed into the intended account.

1. Confirm the signed-in account, exact target, and approved text.
2. Open the reply composer and check its target and focus before typing.
3. Inspect the complete text in the composer before sending.
4. Send once, then verify the posted reply or a reliable sent confirmation.

If navigation, focus, text, or account is wrong, stop and correct it before sending. If a send may have succeeded, check for the posted reply before retrying to avoid duplicates. If the interface remains unreliable, provide the target link and approved text for manual posting.

Do not post unsupported allegations, fake insider claims, or undisclosed promotions. Do not turn research into unsolicited mass replies or manufactured engagement.
