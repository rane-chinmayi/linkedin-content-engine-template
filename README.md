# LinkedIn Content Engine — Template

A plug-and-play AI content pipeline for LinkedIn, built 
with Claude Code specialist sub-agents.

> "AI handles structure. Humans handle truth."

---

## What This Is

A system of 4 specialist Claude Code sub-agents that work 
together to plan, write, and optimize your LinkedIn content 
every week — in your voice, not AI's.

Built by [Chinmayi Rane](https://www.linkedin.com/in/chinmayi-rane/) 
— adapted from her personal LinkedIn Content Engine that 
reduced weekly content creation from 3+ hours to 30 minutes.

---

## The 4 Agents

| Agent | Color | Job |
|-------|-------|-----|
| 🧠 Content Strategist | Purple | Generates 6 post ideas every Sunday (2 per day) |
| ✍️ Post Writer | Blue | Writes full posts in your voice. Runs Human Test. |
| 🎯 Hook Critic | Red | Rates your opening line 1-10, gives 3 alternatives |
| 💬 Comment Strategist | Yellow | Drafts daily comments for you to review and post |

---

## Project Structure

```
linkedin-content-engine-template/
├── CLAUDE.md                    # YOUR memory file — fill this in first
├── assets/                      # Add your photos here (for carousels)
├── weeks/                       # Your weekly post archive
└── .claude/
    └── agents/
        ├── content-strategist.md
        ├── post-writer.md
        ├── hook-critic.md
        └── comment-strategist.md
```

---

## How to Use This Template

### Step 1 — Clone and open in Claude Code

```bash
git clone https://github.com/rane-chinmayi/linkedin-content-engine-template
cd linkedin-content-engine-template
```

Open the folder in Claude Code desktop.

### Step 2 — Fill in CLAUDE.md
This is the most important step. Open `CLAUDE.md` and 
replace every `[PLACEHOLDER]` with your real information:
- Your name and role
- Your 4 content pillars
- Your audience description
- Your writing voice and tone
- Your posting schedule and themes

The more specific you are, the better every agent performs.

### Step 3 — Add your best performing posts
In `CLAUDE.md` add a section called `## My Best Posts` 
and paste in 2-3 of your highest performing LinkedIn posts. 
The agents will reverse-engineer your voice from these.

### Step 4 — Run your first week
In Claude Code, type:

```
Read CLAUDE.md. Then ask the 🧠 Content Strategist 
to plan my week.
```

---

## Weekly Workflow

### Sunday — Content Planning (15 mins)

```
Step 1: "Read CLAUDE.md. Ask the 🧠 Content Strategist to plan my week."
Step 2: Review 6 ideas → pick 1 per day
Step 3: Add your real personal details to each brief
Step 4: "Ask the ✍️ Post Writer to write all three posts: [briefs]"
Step 5: "Ask the 🎯 Hook Critic to review the three hooks: [hooks]"
Step 6: Swap in winning hooks → posts ready
Step 7: Save to weeks/week-[date].md
```

### Monday / Wednesday / Friday — Posting (2 mins)

```
Copy paste your post → add your photo → publish
```

### Daily — Comment Strategy (10 mins)

```
Step 1: Paste 3-5 post excerpts you saw while scrolling
Step 2: "Ask the 💬 Comment Strategist to draft comments for: [excerpts]"
Step 3: Pick safe or bold version for each
Step 4: Post yourself on LinkedIn within 60 mins of creator posting
```

---

## The Human Test

Every post must pass this before publishing:
- Could only YOU have written this?
- Does it sound like you talking to a friend?
- Is there at least one detail that feels real and lived-in?

If NO to any — rewrite. Don't publish.

This is baked into every agent. It's your protection 
against AI-sounding content.

---

## How CLAUDE.md Works

Every agent reads this file before doing anything. It's 
your shared memory — voice fingerprint, audience, content 
pillars, proven patterns, and the Human Test.

Think of it as your creative brief that every team member 
reads before starting work.

---

## Customization Tips

**To change an agent's behavior:**
Open the relevant `.claude/agents/` file and edit the 
rules or persona directly. Changes take effect immediately.

**To add a new content pillar:**
Update the `## Your Content Pillars` section in CLAUDE.md. 
All agents pick it up on next run.

**To improve post quality over time:**
After each week, add your best post to the `## My Best Posts` 
section in CLAUDE.md. The agents get better as they learn 
more of your proven patterns.

**To add target creators for commenting:**
Add a `## Target Creators` section to CLAUDE.md with 
names and LinkedIn handles of creators your audience 
follows.

---

## Tech Stack

- Claude Code desktop (required)
- No other dependencies for text posts
- Python 3.12 + Pillow + ReportLab (optional, for carousel generation)

---

## Original Project

This template is based on Chinmayi Rane's personal 
LinkedIn Content Engine. The original private repo 
includes a carousel PDF generator and personal voice 
fingerprint.

[Connect on LinkedIn](https://www.linkedin.com/in/chinmayi-rane/)

---

## Topics
`claude-code` `ai-agents` `linkedin` `content-automation` 
`personal-branding` `sub-agents` `productivity`
