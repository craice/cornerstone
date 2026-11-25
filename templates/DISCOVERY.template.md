# [Project Name] — Discovery

> Structured exploration of the project idea

---

## Discovery Guardrails

> **Instructions for the AI assistant conducting Discovery.**
>
> These rules apply throughout the entire Discovery conversation:
>
> 1. **Don't accept vague answers.** If the human says something generic ("it should be good" / "modern design" / "normal users"), ask them to be specific. What does "good" mean to them? What does "modern" look like? Who exactly is a "normal user"?
> 2. **Challenge assumptions.** If the human assumes something without justification ("we'll use React" / "it needs a database"), ask *why*. There might be a simpler path.
> 3. **Offer options when they don't know.** If the human says "I don't know", don't move on — suggest 2-3 concrete options and explain tradeoffs so they can choose.
> 4. **Confirm understanding before advancing.** Before moving to the next dimension, summarize what you heard and ask "Is this accurate?" Misunderstandings caught early cost nothing; misunderstandings caught during execution cost everything.
> 5. **Flag contradictions.** If something said in Scope contradicts something from Purpose, say so immediately. Don't wait.

---

## How to Use This Document

This template guides the Discovery conversation between you and an AI assistant. You don't need to fill it in alone — start a conversation with an AI, share your idea, and work through the 6 dimensions together. Use this as a checklist to make sure nothing is missed.

### Kick-off Prompt

```
I want to create [your idea in 1-2 sentences].

Help me define this project using the Cornerstone Discovery process.
Interview me across these 6 dimensions: Purpose, Audience, Scope,
Constraints, Quality, and Identity. Ask questions one group at a time.
Challenge my assumptions when needed.
```

---

## 1. Purpose — *Why does this exist?*

*Write freely. The AI should guide you through these questions in conversation, not as a form to fill.*

**What problem are you trying to solve? Describe it in your own words.**

[Write here — be honest, be specific. If you're not sure, say that too.]

**Who has this problem today, and how are they dealing with it?**

[Write here]

**What happens if this project never gets built?**

[Write here — this reveals how important it really is]

**What's driving you to build this?** (personal need / commercial opportunity / learning / open source / other)

[Write here]

**The one-sentence version:** [Try to capture the whole idea in a single sentence]

**Summary:** [After discussion, capture the purpose in 2-3 sentences]

---

## 2. Audience — *Who is it for?*

**Describe your primary user. Who are they? What's their day like? What frustrates them?**

[Write here — a real person, not a persona template]

| Question | Answer |
|----------|--------|
| Secondary user (if any)? | |
| What do they use today? | |
| Technical level? | |
| What would make them choose this? | |

**Summary:** [After discussion, capture the audience in 2-3 sentences]

---

## 3. Scope — *What's in and what's out?*

### In Scope (Must-Haves)

- [ ] ...
- [ ] ...
- [ ] ...

### Out of Scope (Explicitly Not Included)

- ...
- ...

### Future Scope (Maybe Later)

- ...
- ...

**What's the smallest version that would be valuable?** Describe the MVP — the version with the fewest features that still solves the core problem.

[Write here]

| Question | Answer |
|----------|--------|
| What features seem important but can wait? | |
| Is there anything you've assumed is included that might not need to be? | |

---

## 4. Constraints — *What limits exist?*

### Technical

| Question | Answer |
|----------|--------|
| Are there required languages or frameworks? | |
| Required platforms (web, mobile, desktop)? | |
| Hosting requirements or preferences? | |
| Dependencies or integrations? | |
| Any technologies to avoid? | |

### Time & Resources

| Question | Answer |
|----------|--------|
| Is there a deadline? | |
| How many hours per week can you dedicate? | |
| Solo or team? | |
| Budget (if any)? | |
| Existing assets to reuse? (code, design, content) | |

### Knowledge

| Question | Answer |
|----------|--------|
| What do you already know well? | |
| What would you need to learn? | |
| Are you comfortable with that learning curve? | |

---

## 5. Quality — *What standards matter?*

| Question | Answer |
|----------|--------|
| Performance expectations? (fast, acceptable, doesn't matter) | |
| Accessibility requirements? (WCAG level, specific needs) | |
| Browser/device support? | |
| Visual quality bar? (rough, clean, polished, pixel-perfect) | |
| Testing expectations? (none, basic, comprehensive) | |
| Documentation expectations? | |

---

## 6. Identity — *What makes this unique?*

*Write freely. Identity is about feel, not data — let it flow naturally.*

**What's the personality of this project? If it were a person, how would it talk?**

[Write here — formal? playful? minimal? warm? technical?]

**What should this absolutely NOT look or feel like?**

[Write here — anti-references are as useful as references]

**Are there projects, products, or designs that inspire you?** Share links, screenshots, or descriptions.

[Write here]

**Are there brand elements to follow?** (existing colors, fonts, logo, tone)

[Write here — or "starting from scratch"]

**If this project were a building, what kind would it be?**

[Write here — this is a thinking exercise, not a test. A cozy cabin? A glass skyscraper? A library?]

---

## Discovery Checklist

Before moving to Specification, verify:

- [ ] **Purpose** is clear — you can explain why this exists in one sentence
- [ ] **Audience** is defined — you know who it's for and who it's not for
- [ ] **Scope** has boundaries — you know what's in, what's out, and what's for later
- [ ] **Constraints** are documented — technical, time, and resource limits are known
- [ ] **Quality** standards are set — you know how good is good enough
- [ ] **Identity** has direction — you have a sense of personality and style
- [ ] **No major open questions** — or they're explicitly noted for later resolution

---

## Transition to Specification

When Discovery is complete, use this prompt:

```
Based on our Discovery conversation, create a complete SPECIFICATION.md
using the Cornerstone Specification template. Capture every decision we made.
Be comprehensive — this document should be the single source of truth
for the entire project.
```

---

*This file follows the Cornerstone process. For more information, see CORNERSTONE.md*
