# Cheat Reply

An agent skill for researching X/Twitter conversations and drafting replies in your voice.

The workflow starts with the actual comments: read the post, study what people are responding to, and contribute one specific observation, question, or joke. It supports learning, drafting, and posting text you have approved.

## Install

Clone the repository into your agent's skills directory. For a local Codex installation using `~/.codex/skills`:

```sh
git clone https://github.com/nniiovoo/cheat-reply.git ~/.codex/skills/cheat-reply
```

For Claude Code:

```sh
git clone https://github.com/nniiovoo/cheat-reply.git ~/.claude/skills/cheat-reply
```

If `cheat-reply` is already installed at the destination, compare or back up your customized copy before replacing it. Other skill-compatible agents can load the root [SKILL.md](SKILL.md); use their supported skill directory.

The package contains instructions and examples. It does not install a browser extension, connect an X account, store credentials, or run a background posting service. Live research needs browsing tools that can read the conversation; you can also paste the post and relevant comments.

## Use

Example requests:

```text
Use $cheat-reply to study the replies to this post and draft one response
in my voice: [post URL]. Draft only.
```

```text
Use $cheat-reply to find active conversations about [your topic].
Study the comments and show me three relevant targets. Do not post.
```

```text
Use $cheat-reply to learn from these pasted comments. Summarize the
patterns worth testing; don't write a reply yet.
```

Research and drafting do not authorize publication. Posting requires approval of the exact reply and target, an authorized posting tool or signed-in browser, and verification after sending.

## Personalize

Describe your audience and voice in the request, or copy the optional templates into your own working project:

- [audience.md](examples/audience.md): audience, voice, and boundaries.
- [reply-learnings.md](examples/reply-learnings.md): current observations and recent cases.

The skill reads those files only when present. It does not require the wider `cheat-on-content` system. Keep real account notes, private conversations, credentials, and performance data outside this repository.

## Files

| File | Purpose |
|---|---|
| [SKILL.md](SKILL.md) | Main workflow and posting boundaries |
| [Reply playbook](references/reply-playbook.md) | Optional strategy and maintenance reference |
| [Examples](examples/) | Generic, optional account-context templates |
| [Agent metadata](agents/openai.yaml) | Skill discovery metadata |

## Contributing

Issues and pull requests are welcome. Include a concrete example of the behavior you want to improve. Anonymize account details and private context; do not submit credentials or copied private conversations. Keep new rules specific to the situation where they help, and distinguish observations from claims about the algorithm.

## Origin and license

This standalone distribution is maintained by [nniiovoo](https://github.com/nniiovoo). It was developed from a local extension to [cheat-on-content](https://github.com/XBuilderLAB/cheat-on-content), with additional reply research and workflow refinements.

Distributed under the [MIT License](LICENSE), retaining the `cheat-on-content contributors` notice for inherited material. Public packaging adds generic context templates and removes account-specific case histories and local-path dependencies.
