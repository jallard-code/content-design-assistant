# Content Design Assistant — Claude Skill

A Claude Code skill for anyone creating content at Thumbtack. Paste in copy, get back a scored review, issue-by-issue feedback, and a rewrite — all against Thumbtack's voice and style guidelines. Use it standalone in Claude Code or as the brains behind the Figma plugin.

---

## What it does

- Reviews content against Thumbtack voice, tone, grammar, and component rules
- Scores the original and rewrite independently on a 1–5 scale
- Names each issue specifically and references the rule it breaks
- Rewrites only what's broken — preserves what's working
- Handles UI copy, email, error messages, buttons, and more
- Asks for audience (customer vs. pro) before generating new content from scratch

---

## Install

### Step 1 — Get the file

Clone or download this repo:

```
git clone https://github.com/jallard-code/content-design-assistant.git
```

### Step 2 — Place the skill file

Copy `content-design-assistant.md` into your personal Claude skills directory so it's available across all your projects:

```
cd content-design-assistant
mkdir -p ~/.claude/skills/content-design-assistant
cp content-design-assistant.md ~/.claude/skills/content-design-assistant/SKILL.md
```

That's it. No restart needed.

### Step 3 — Use it

Open Claude Code in any project and type:

```
/content-design-assistant
```

Or just start a conversation — Claude will load the skill automatically when you're doing a content review.

---

## How to use it

**Review existing content**

Paste in your copy and ask for a review. You can include labels like `[Header]`, `[Body text]`, or `[CTA button]` to tell it what component each piece belongs to — that makes the feedback more accurate.

```
Review this:

[Header] Get more done with Thumbtack
[Body text] Thumbtack has been helping customers find pros since 2008. Our platform utilizes advanced matching technology to connect you with the right professional for your project.
[CTA button] Get Started
```

**Generate new content**

Ask it to write something and it will ask whether it's for a customer or a pro before starting.

```
Write a confirmation message for when a customer books a pro.
```

**Ask follow-up questions**

After a review, you can ask it to explain a specific issue, try a different angle, or adjust the tone. It responds conversationally without re-running the full review format.

---

## Scoring rubric

| Score | Meaning |
|---|---|
| 5 | Ships immediately — every word is necessary, reads like a real Thumbtack person wrote it |
| 4 | Minor issues only — good to ship with small tweaks |
| 3 | 1–2 major issues — needs a real edit before shipping |
| 2 | 3+ major issues — significant rework needed |
| 1 | Critical issue present — do not ship |

---

## Questions

Reach out to Jody Allard on Slack.
