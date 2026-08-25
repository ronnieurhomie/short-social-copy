# short-social-copy

A reusable AI skill for writing short social copy that **complements a video instead of summarizing it**.

Built for:

- TikTok and Instagram captions
- YouTube Shorts descriptions
- X companion posts
- other short social copy

It is deliberately **not** a video-script writer.

## The problem

AI-generated social copy often sounds polished but lifeless:

- it repeats the video's hook
- summarizes the whole story
- uses canned lines like "Here's why this matters"
- turns a casual observation into marketing or LinkedIn copy

That creates copy that is technically correct but does not sound like something a person would naturally post.

## The approach

The skill extracts the video's central tension, removes what the viewer already hears, and chooses one complementary angle:

- the strangest implication
- the hidden conflict
- the detail that changes how the story feels
- a natural reaction
- an honest unanswered question

The output defaults to one recommended version, without unnecessary alternatives, hashtags, emojis, or calls to action.

## Real RON example

For a video about Nvidia seeking enormous outside financing:

**Too written**

> Everyone's obsessed with chips.  
> But that may not be what slows AI down.

**Preferred**

> the wild part isn't that Nvidia needs $500B  
> it's that Wall Street might be the one paying for it

The second version does not recap the financing mechanism. It isolates the surprising relationship and leaves the explanation to the video.

## Feedback becomes reusable rules

The skill translates recurring creator feedback into transferable editing rules:

| Feedback | Reusable correction |
| --- | --- |
| "sounds written" | Reduce symmetry, polish, exposition, and complete-sentence formality |
| "sounds like AI" | Remove canned pivots, vague stakes, and generic emphasis |
| "too much like the video" | Shift from recap to implication, reaction, or unresolved tension |
| "too long" | Keep the single line with the most curiosity and factual integrity |
| "too generic" | Anchor the copy in the story's distinctive fact or contradiction |

These are treated as patterns, not universal laws. New feedback should improve the system without overfitting it to one post.

## Platform defaults

| Platform | Default behavior |
| --- | --- |
| TikTok / Instagram | One or two short lines with a reaction, implication, or curiosity gap |
| YouTube Shorts | Discoverable subject, without turning the description into a miniature summary |
| X | A standalone companion thought that still rewards watching |

## Use

Invoke the skill with an existing video script, transcript, or story and specify the platform when relevant.

Example:

```text
Use @short-social-copy to write an X companion post for this video.
```

The skill returns one recommended version first. Alternatives are only added when they explore meaningfully different angles or are explicitly requested.

## Repository structure

```text
.
├── SKILL.md            # Core workflow and writing rules
├── agents/openai.yaml  # ChatGPT/Codex metadata
├── assets/icon.svg     # Skill icon
└── LICENSE             # MIT
```

## Validation status

This is an early working version developed from real RON short-form posts and direct creator feedback. It has been structurally validated as a ChatGPT/Codex skill.

It is not presented as a proven universal writing formula. The next stage is repeated use across real TikTok, Instagram, YouTube Shorts, and X posts—logging failures, updating only reusable rules, and comparing outputs over time.

## Design principles

1. Complement the video; do not recap it.
2. Sound observed, not composed.
3. Let the fact create interest; do not announce that it is interesting.
4. Preserve tension without manufacturing hype.
5. Prefer one strong recommendation over a menu of minor variations.
6. Never trade factual accuracy for a stronger hook.

## License

MIT
