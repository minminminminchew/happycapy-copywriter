# happycapy-copywriter

A Claude Code skill for writing HappyCapy marketing copy. Built for the HappyCapy marketing team.

## What it does

This skill turns Claude into a dedicated HappyCapy copywriter. It knows the brand voice, product positioning, and target audiences. Give it a writing task and it walks you through platform, format, tone, and context before generating on-brand copy.

Supports 12 platforms, multiple formats per platform, and three language modes (English, Chinese, bilingual mix).

## Supported platforms and formats

| Platform | Formats |
|----------|---------|
| Twitter / X | Single tweet, thread, reply/quote tweet, bio |
| Xiaohongshu (RED) | Image-text post, short video caption, comment reply |
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

The skill follows a 7-step workflow:

1. **Pick the platform** - Where will this copy live?
2. **Pick the format** - What type of content? (thread vs. single tweet, post vs. article, etc.)
3. **Pick tone and language** - Suggests defaults per platform, you can override
4. **Gather context** - What feature, update, or theme to write about
5. **Research** - Searches for high-performing examples of the same platform + format combo, shares insights before writing
6. **Generate, score, and self-improve** - Recursive loop: generate draft, score against criteria, diagnose failures, rewrite, re-score. Repeats until all criteria pass. Then stress-tests through an adversarial persona attack.
7. **Present and refine** - Iterate on tone, length, focus, language mix. Every revision goes through the same scoring loop.

## Key features

**Recursive self-improvement loop.** The skill doesn't just generate and ship. It scores every draft against 8 criteria (6 universal + 2 platform-specific), diagnoses what's weak, rewrites, and re-scores. Nothing gets presented until all criteria pass their minimum thresholds. After scoring, it stress-tests the copy through an adversarial persona attack (e.g., "The Skeptical Developer", "The Cynical Redditor") to find weaknesses a checklist might miss.

**Scoring criteria.** Every piece of copy is scored 1-10 on: Hook Power, Human Voice, Brand Alignment, Clarity, CTA Effectiveness, Emotional Resonance, plus 2 platform-specific criteria. Each has a defined minimum threshold and automatic score caps for specific violations (e.g., using banned AI words caps Human Voice at 5/10).

**Anti-AI writing rules.** The skill actively avoids AI writing tells: excessive dashes, "seamlessly/effortlessly/leverage" vocabulary, repetitive sentence structures, and generic patterns like "Whether you're X or Y." Copy should read like a human wrote it.

**Research before writing.** Before generating any copy, the skill searches for top-performing examples on the target platform. It studies hooks, structure, tone, and engagement patterns, then applies those insights.

**Bilingual native.** HappyCapy's brand naturally mixes English and Chinese. The skill handles code-switching between both languages without awkward forced translations. Technical terms (Claude Code, Skills, Agent, AI) stay in English.

**Opinionated.** The skill pushes back on off-brand requests and suggests angles you might not have considered. It won't just say yes to everything.

## Skill structure

```
happycapy-copywriter/
├── SKILL.md                        # Core workflow and brand voice rules
└── references/
    ├── brand-foundation.md         # Product facts, positioning, audiences, anti-patterns
    ├── platform-guides.md          # Format rules and structure patterns for 12 platforms
    ├── scoring-criteria.md         # Scoring rubric, thresholds, and adversarial personas
    └── examples.md                 # Real brand copy examples with voice analysis
```

## Installation

Copy the skill folder to your Claude Code skills directory:

```bash
cp -r happycapy-copywriter ~/.claude/skills/
```

## Usage

Trigger the skill by asking Claude to write copy for HappyCapy. Examples:

- "write copy"
- "Write a Product Hunt launch post"
- "Draft a Xiaohongshu post about the Skills feature"
- "Write ad copy for Google Ads"
- "Help me write a tweet about the new update"

## Brand voice in a nutshell

Confident but not arrogant. Simple but not shallow. Exciting but grounded.

The copy should feel like it was written by someone who genuinely built and uses the product. Not a marketing department. Not an AI.

## About HappyCapy

HappyCapy is an agent-native computer powered by Claude Code that runs in your browser. Built by the [Trickle](https://trickle.so) team.

For more: [happycapy.ai](https://happycapy.ai)
