# Copy Scoring Criteria

Score every piece of generated copy against these criteria. Each criterion is scored 1-10. The copy does not ship until ALL criteria hit their minimum threshold.

## Universal Criteria (Apply to ALL copy)

These 6 criteria apply regardless of platform or format.

### 1. Hook Power (min: 8/10)
Does the first sentence stop the scroll? Would a busy, distracted person pause and keep reading?
- 10: Impossible to ignore. Creates immediate curiosity or recognition.
- 8: Strong pull. Most readers would keep going.
- 5: Generic opener. Could be any brand, any product.
- 3: Boring. Starts with "We are excited to..." or similar filler.

### 2. Human Voice (min: 9/10)
Does this sound like a real person wrote it, or does it smell like AI?
- 10: Completely natural. You'd never guess AI was involved.
- 8: Mostly natural with maybe one slightly formulaic phrase.
- 5: Noticeably AI. Dashes everywhere, "seamlessly" type words, repetitive structure.
- 3: Obviously AI. Could be any LLM output on any topic.

Specific checks:
- Dash count: more than 1 per 200 words = automatic cap at 6/10
- Any word from the banned list (seamlessly, effortlessly, streamline, empower, leverage, unlock, delve, robust, harness) = automatic cap at 5/10
- "Whether you're X or Y", "From X to Y", "It's not just X, it's Y" patterns = automatic cap at 6/10
- Three or more consecutive sentences with the same structure = automatic cap at 7/10

### 3. Brand Alignment (min: 8/10)
Does this feel like HappyCapy? Could you put the HappyCapy name on it and it fits?
- 10: Unmistakably HappyCapy. Uses brand patterns naturally, nails the confident-but-grounded tone.
- 8: On-brand. Consistent with voice guidelines.
- 5: Generic tech copy. Could be any SaaS product.
- 3: Off-brand. Too corporate, too hypey, or contradicts positioning.

Specific checks:
- Contains hype words without substance (revolutionary, game-changing, cutting-edge) = automatic cap at 5/10
- Over-promises (replace all your tools, never code again) = automatic cap at 4/10
- Corporate stiffness (We are pleased to announce...) = automatic cap at 4/10

### 4. Clarity (min: 8/10)
Would someone who has never heard of HappyCapy understand what it does after reading this?
- 10: Crystal clear. A non-technical person gets it instantly.
- 8: Clear with minimal effort. Might need one re-read for technical details.
- 5: Confusing. Jargon-heavy or assumes too much prior knowledge.
- 3: Incomprehensible to outsiders.

### 5. CTA Effectiveness (min: 7/10)
Does the reader know what to do next? Is the call-to-action natural and compelling?
- 10: Irresistible. The reader feels pulled toward action.
- 8: Clear and motivated. Reader knows the next step.
- 5: Present but weak. Generic "learn more" or buried.
- 3: Missing or awkward. Forced sales pitch.

### 6. Emotional Resonance (min: 7/10)
Does this make the reader FEEL something? Curiosity, excitement, recognition, relief?
- 10: Strong emotional pull. Reader thinks "I need this" or "I want to try this."
- 8: Engages interest. Reader is intrigued.
- 5: Flat. Informative but no feeling.
- 3: Repels. Feels like spam or empty hype.

## Platform-Specific Criteria

Apply these IN ADDITION to the universal criteria, based on the target platform.

### Social Media (Twitter, Xiaohongshu, LinkedIn, Reddit)

**7. Scroll-Stop Power (min: 8/10)**
In a fast-moving feed, would this make someone pause?
- 10: Thumb-stopper. The first line alone creates a curiosity gap or pattern interrupt.
- 8: Strong hook. Stands out from typical feed content.
- 5: Blends in. Nothing distinctive about the opening.

**8. Engagement Trigger (min: 7/10)**
Would this prompt replies, shares, saves, or discussion?
- 10: Inherently shareable or debatable. People want to respond.
- 8: Invites engagement naturally. Good question or provocative angle.
- 5: One-way broadcast. Nothing to respond to.

### Product Hunt / Reddit

**7. Authenticity (min: 9/10)**
Does this sound like a real maker talking, not a marketing department?
- 10: You'd swear a founder wrote this at 2am. Personal, specific, honest.
- 8: Genuine and transparent. Community would trust this person.
- 5: Marketing-speak leaking through. Community would be skeptical.
- 3: Corporate press release. Would get downvoted.

**8. Community Value (min: 8/10)**
Does this give the community something useful beyond self-promotion?
- 10: Teaches something, shares a genuine insight, or starts a meaningful discussion.
- 8: Offers value alongside the product mention.
- 5: Pure self-promotion dressed up as a discussion.

### Landing Page / Website

**7. Scanability (min: 8/10)**
Can someone get the core message in 5 seconds of scanning?
- 10: Hierarchy is perfect. Bold text, short sections, clear visual flow.
- 8: Easy to scan. Key points jump out.
- 5: Wall of text. Requires committed reading.

**8. Objection Handling (min: 7/10)**
Does the copy preemptively address likely concerns?
- 10: Anticipates and resolves the top 3 objections naturally within the flow.
- 8: Handles the biggest concern without feeling defensive.
- 5: Ignores obvious questions the reader would have.

### Ad Copy

**7. Benefit Specificity (min: 8/10)**
Is the benefit concrete and specific, not abstract?
- 10: "Write code, generate images, process documents in your browser." (Specific actions.)
- 5: "Boost your productivity." (Vague.)
- 3: "The future of computing." (Meaningless.)

**8. Click Motivation (min: 8/10)**
Would someone actually click this ad?
- 10: Creates urgency or curiosity that demands a click.
- 8: Clear value proposition. Clicking feels like a good investment of time.
- 5: No reason to click over any other ad.

### Email / Newsletter

**7. Subject Line Power (min: 8/10)**
Would this get opened in a crowded inbox?
- 10: Impossible to skip. Creates personal curiosity or urgency.
- 8: Stands out from typical marketing emails. Would get opened.
- 5: Generic. Blends with other promotional emails.

**8. Skim Value (min: 8/10)**
Can the reader get the key message by skimming bold text and headers?
- 10: Bold text alone tells the full story.
- 8: Quick skim reveals the core message and CTA.
- 5: Must read every word to understand.

## Adversarial Pressure Personas

After scoring, attack the copy from one of these perspectives (choose the most relevant):

**The Distracted Scroller**: "I'm on my phone, half-watching TV, scrolling through 200 posts. Would I stop for this? Why? What would make me keep scrolling?"

**The Skeptical Developer**: "I've seen 50 AI tools this week. Why should I care about this one? What's actually different? Prove it."

**The Non-Technical User**: "I don't know what Claude Code is. I don't know what 'agent-native' means. Does this copy make me feel included or excluded?"

**The Competitor's CMO**: "I work at a rival product. Can I rip this positioning apart? Where are the weak points? What claim can I undermine?"

**The Cynical Redditor**: "This is just another startup promoting themselves. Change my mind. What's genuine here?"

Pick the persona most dangerous to this specific piece of copy. If the copy survives the attack, it ships. If the persona finds a real weakness, diagnose and rewrite.
