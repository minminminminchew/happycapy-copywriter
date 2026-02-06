# happycapy-copywriter

A Claude Code skill for writing HappyCapy marketing copy. Built for the HappyCapy marketing team.

## What it does

This skill turns Claude into a dedicated HappyCapy copywriter. It knows the brand voice, product positioning, and target audiences. Give it a writing task and it walks you through platform, format, tone, and context before generating on-brand copy.

Supports 12 platforms, multiple formats per platform, and three language modes (English, Chinese, bilingual mix).

## Supported platforms and formats

| Platform | Formats |
|----------|---------|
| Twitter / X | Single tweet, thread, reply/quote tweet, bio |
| 小红书 | 图文笔记, short video caption, comment reply |
| LinkedIn | Post, article, comment, company page intro |
| Product Hunt | Launch post, discussion post, comment, tagline |
| Reddit | Post, comment, AMA answer |
| Website | Hero section, feature section, about page, FAQ, CTA block |
| Blog | Full article, intro + outline, summary/abstract |
| Email | Announcement, welcome email, weekly digest, drip sequence |
| Ad | Search ad, display ad, social ad, retargeting ad |
| App Store | Title + subtitle, description, "what's new" |
| Changelog | Announcement, release notes |
| Slogan | Tagline brainstorm |

## How it works

The skill follows an 8-step workflow:

1. **Pick the platform** - Where will this copy live?
2. **Pick the format** - What type of content? (thread vs. single tweet, post vs. article, etc.)
3. **Pick tone and language** - Suggests defaults per platform, you can override
4. **Gather context** - What feature, update, or theme to write about
5. **Research** - Searches for high-performing examples of the same platform + format combo, shares insights before writing
6. **Generate** - Writes copy with multiple variations for short/medium-form
7. **Quality check** - AI smell test, platform-native check, brand check
8. **Refine** - Iterate on tone, length, focus, language mix

## Key features

**Anti-AI writing rules.** The skill actively avoids AI writing tells: excessive dashes, "seamlessly/effortlessly/leverage" vocabulary, repetitive sentence structures, and generic patterns like "Whether you're X or Y." Copy should read like a human wrote it.

**Research before writing.** Before generating any copy, the skill searches for top-performing examples on the target platform. It studies hooks, structure, tone, and engagement patterns, then applies those insights.

**Bilingual native.** HappyCapy's brand naturally mixes English and Chinese. The skill handles 中英 code-switching without awkward forced translations. Technical terms (Claude Code, Skills, Agent, AI) stay in English.

**Opinionated.** The skill pushes back on off-brand requests and suggests angles you might not have considered. It won't just say yes to everything.

## Skill structure

```
happycapy-copywriter/
├── SKILL.md                        # Core workflow and brand voice rules
└── references/
    ├── brand-foundation.md         # Product facts, positioning, audiences, anti-patterns
    ├── platform-guides.md          # Format rules and structure patterns for 12 platforms
    └── examples.md                 # Real brand copy examples with voice analysis
```

## Installation

Copy the skill folder to your Claude Code skills directory:

```bash
cp -r happycapy-copywriter ~/.claude/skills/
```

## Usage

Trigger the skill by asking Claude to write copy for HappyCapy. Examples:

- "写文案" / "write copy"
- "帮我写一条推文"
- "Write a Product Hunt launch post"
- "Draft a 小红书 post about the Skills feature"
- "Write ad copy for Google Ads"

## Brand voice in a nutshell

Confident but not arrogant. Simple but not shallow. Exciting but grounded.

The copy should feel like it was written by someone who genuinely built and uses the product. Not a marketing department. Not an AI.

## About HappyCapy

HappyCapy is an agent-native computer powered by Claude Code that runs in your browser. Built by the [Trickle](https://trickle.so) team.

For more: [happycapy.ai](https://happycapy.ai)
