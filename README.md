# short-social-copy

A reusable AI skill that turns a **finished video script into a strong video title and short companion copy**.

## Input → output

**Input:** a video script  
**Output:** a video title, TikTok/Instagram captions, YouTube Shorts descriptions, X companion posts, or a requested combination

This is not a scriptwriting skill. It does not start from a loose topic, article, story idea, or transcript.

## The problem

AI-generated social copy often sounds polished but lifeless. It tends to:

- repeat the video's hook
- summarize the full script
- use canned marketing pivots
- add fake-casual phrases to disguise a polished thesis
- produce several near-identical options instead of one strong recommendation

The result may be technically correct while still sounding like copy nobody would naturally post.

## The approach

The skill reads the full script and separates two jobs:

- **Title:** package the video's central tension clearly and accurately
- **Companion copy:** remove what the viewer already hears and add a complementary angle

For companion copy, it looks for:

- the strangest implication
- the hidden conflict
- the detail that changes how the story feels
- a natural reaction
- an honest unanswered question

It then writes the shortest platform-appropriate version that preserves that angle without adding unsupported claims.

## A failure caught during testing

Both of these drafts were rejected as too written:

> Everyone's obsessed with chips.  
> But that may not be what slows AI down.

> the wild part isn't that Nvidia needs $500B  
> it's that Wall Street might be the one paying for it

The first reads like a polished headline. The second performs casualness but still uses a rehearsed `not X, but Y` contrast.

The reusable lesson is not “use more casual phrases.” It is:

- remove thesis-like contrast structures
- remove performed conversational lead-ins
- do not confuse lowercase text with natural voice
- do not label any draft a positive example until the creator explicitly approves it

## Feedback becomes reusable rules

| Feedback | Reusable correction |
| --- | --- |
| “sounds written” | Reduce symmetry, exposition, thesis-like contrast, and polished sentence structure |
| “sounds like AI” | Remove canned pivots, performed casualness, vague stakes, and generic emphasis |
| “too much like the video” | Shift from recap to implication, reaction, or unresolved tension |
| “too long” | Keep the single line with the most curiosity and factual integrity |
| “too generic” | Anchor the copy in the script's distinctive fact or contradiction |

New feedback should improve the rule set without overfitting it to one post.

## Video titles

Titles follow a different rule from companion copy:

- package the script's central tension, decision, conflict, or surprising fact
- make the subject clear instead of relying on vague curiosity
- prefer concrete nouns and active language
- avoid clickbait, generic stakes, unsupported conclusions, and title formulas
- give one recommendation first; alternatives must represent genuinely different framings

A title does not need to complement the video. Its job is to package the video accurately.

## Platform defaults

| Platform | Default behavior |
| --- | --- |
| TikTok / Instagram | One or two short lines with a reaction, implication, or curiosity gap |
| YouTube Shorts | Make the subject discoverable without writing a miniature summary |
| X | Write a standalone companion thought that still rewards watching |

## Use

Supply the complete video script and specify the platform when relevant.

```text
Use @short-social-copy to turn this video script into a video title and X companion post.
[PASTE SCRIPT]
```

The skill gives one recommended version first. It adds alternatives only when they explore genuinely different angles or the user requests them.

## Repository structure

```text
.
├── SKILL.md            # Input contract, workflow, and writing rules
├── agents/openai.yaml  # ChatGPT/Codex metadata
├── assets/icon.svg     # Skill icon
└── LICENSE             # MIT
```

## Validation status

This is an early working version built through real RON script-to-copy testing and direct creator feedback. It is structurally validated as a ChatGPT/Codex skill.

It is not presented as a proven universal writing formula. The next stage is repeated testing across real RON scripts and platforms, recording rejected drafts and adding only lessons that transfer across multiple posts.

## Design principles

1. Start from the full video script.
2. Package the central tension clearly in the title.
3. Complement the script rather than recap it in companion copy.
4. Do not perform casualness.
5. Preserve tension without manufacturing hype.
6. Prefer one strong recommendation over minor variations.
7. Never trade factual accuracy for a stronger hook.
8. Treat creator approval—not the model's explanation—as the final quality signal.

## License

MIT
