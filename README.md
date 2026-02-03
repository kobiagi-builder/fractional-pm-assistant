# Fractional PM Agent

> Your AI-powered partner for managing multiple clients, maintaining obsessive documentation, and accessing expert PM frameworks on demand.

<p align="center">
  <img src="https://img.shields.io/badge/Claude-Code-blueviolet?style=for-the-badge" alt="Claude Code">
  <img src="https://img.shields.io/badge/27-Expert%20Capabilities-green?style=for-the-badge" alt="27 Capabilities">
  <img src="https://img.shields.io/badge/9-Operational%20Modes-orange?style=for-the-badge" alt="9 Modes">
</p>

---

## What Is This?

The Fractional PM Agent is an AI assistant specifically designed for **fractional product managers** and **consultants** who juggle multiple clients. It solves three critical problems:

| Problem | Solution |
|---------|----------|
| **Context switching** between clients | Automatic context loading - say "Let's work on [Client]" and everything loads |
| **Documentation slipping** through the cracks | Enforced documentation after every interaction |
| **Reinventing frameworks** for every task | 27 expert capabilities with proven PM methodologies built-in |

This isn't a chatbot or a prompt template. It's a **structured agent system** with rules that enforce behavior, skills for quick operations, and specialized sub-agents for deep work.

---

## Quick Start Guide

### Step 1: Clone or download from Git

https://github.com/kobiagi-builder/fractional-pm-agent

If you're comfortable with the terminal:

```bash
git clone https://github.com/kobiagi-builder/fractional-pm-agent
cd fractional-pm-agent
```

---

### Step 2: Save It Somewhere You'll Remember

Move the folder to an easy-to-find location:

| Your Computer | Suggested Location |
|---------------|-------------------|
| **Mac** | `/Users/[your-name]/Documents/fractional-pm-agent` |
| **Windows** | `C:\Users\[your-name]\Documents\fractional-pm-agent` |

The exact location doesn't matter - just remember where you put it!

---

### Step 3: Open It in Claude Code

<details>
<summary><strong>If using VSCode (Recommended) - Click to expand</strong></summary>

1. **Open VSCode**

2. **Open the agent folder:**
   - Go to **File → Open Folder**
   - Navigate to where you saved the `fractional-pm-agent` folder
   - Select it and click **Open**

3. **Trust the folder:**
   - VSCode will ask "Do you trust the authors?"
   - Click **Yes, I trust the authors**

4. **Start Claude Code:**
   - Look for the Claude icon in the left sidebar and click it, OR
   - Press `Cmd+Shift+P` (Mac) or `Ctrl+Shift+P` (Windows)
   - Type "Claude" and select "Open Claude Code"

5. **You're ready!** Start chatting in the Claude panel.

</details>

<details>
<summary><strong>If using Terminal - Click to expand</strong></summary>

1. **Open Terminal:**
   - **Mac:** Press `Cmd+Space`, type "Terminal", press Enter
   - **Windows:** Press `Win+R`, type "cmd", press Enter

2. **Navigate to your folder:**
   ```bash
   cd /path/to/fractional-pm-agent
   ```
   (Replace `/path/to/` with your actual folder location)

3. **Start Claude Code:**
   ```bash
   claude
   ```

4. **You're ready!** Claude Code starts with the agent loaded.

</details>

<details>
<summary><strong>If using Claude Desktop App - Click to expand</strong></summary>

1. **Open the Claude app**

2. **Tell Claude where the files are:**
   > "I want to use the Fractional PM Agent. The files are in [your folder path]"

3. **Claude will activate the agent** and you're ready to go!

</details>

---

### Step 4: Introduce Yourself (Onboarding)

The first time you use the agent, help it understand who you are. Start with:

> *"Hi! I'm new here. I'm a [your role] working with [types of clients/companies]. I want to use this agent to help me [your main goal]."*

**Example:**
> *"Hi! I'm new here. I'm a fractional product manager working with early-stage B2B SaaS startups. I want to use this agent to help me manage multiple clients and stay organized."*

The agent will ask follow-up questions to build your profile. Be honest - this is like talking to a coach who genuinely wants to help.

**Where your profile lives:** `growth/profile.md` - you can always open this file to see or edit what the agent knows about you.

---

### Step 5: Add Your First Customer

Ready to track a client? say something like:

> *"I want to add a new customer: [Company Name]"*

**What happens next:**
1. The agent creates a folder: `customers/[company-name]/`
2. It asks you questions about the company, team, product, and challenges
3. It sets up the documentation structure automatically

**From now on**, whenever you say "Let's work on [Company Name]", the agent instantly loads all that context.

---

### Step 6: Start Using It!

Here are things you can try right now:

#### For Customer Work

| Say This | What Happens |
|----------|--------------|
| `"Let's work on Acme Corp"` | Loads all Acme context, shows priorities |
| `"I just had a call with Sarah about the roadmap..."` | Documents the event automatically |
| `"What's the status with Acme?"` | Summarizes recent events and open items |

#### For Expert Frameworks

| Say This | Framework Used |
|----------|----------------|
| `"Help me create a product strategy using Playing to Win"` | Lafley/Martin strategy framework |
| `"Write an executive summary in Amazon 6-pager format"` | Amazon's memo structure |
| `"Prioritize this backlog using RICE"` | RICE scoring framework |
| `"Help me position this product for launch"` | April Dunford positioning method |

#### For Personal Growth

| Say This | What Happens |
|----------|--------------|
| `"Assess my skills"` | Growth Advisor evaluates you honestly |
| `"Plan my Q1 professional development"` | Creates OKRs with actionable steps |
| `"I got feedback that I talk too much in meetings"` | Processes feedback into growth plan |

---

### The Magic: It Remembers Everything

After each session, the agent **automatically** updates your documentation.

When you come back - whether tomorrow or three months later - it remembers:
- What you discussed with each customer
- Decisions made and why
- Action items and their status
- Your personal growth journey

You don't have to do anything. The documentation happens automatically.

---

## How It Works (Architecture)

The agent uses a **three-tier system**:

```
┌─────────────────────────────────────────────────────────────────────┐
│                             RULES                                    │
│         Always-active behaviors that trigger automatically           │
│                                                                      │
│   • customer-context-loading  →  MUST load context before work      │
│   • obsessive-documentation   →  MUST update docs after sessions    │
├─────────────────────────────────────────────────────────────────────┤
│                            SKILLS                                    │
│           Lightweight operations that run inline (<1 min)            │
│                                                                      │
│   • load-customer-context  →  Reads & synthesizes customer files    │
│   • update-customer-docs   →  Updates docs after interactions       │
│   • build-agent            →  Creates new rules/skills/capabilities │
├─────────────────────────────────────────────────────────────────────┤
│                         CAPABILITIES                                 │
│              Expert sub-agents for deep work (1+ min)                │
│                                                                      │
│              27 specialists across 9 operational modes               │
└─────────────────────────────────────────────────────────────────────┘
```

### The 9 Operational Modes

| Mode | When to Use | Key Capabilities |
|------|-------------|------------------|
| **BUILDER** | Creating MVPs, scoping features | `zero-to-launch-specialist`, `flow-designer`, `ux-ui-designer` |
| **COMMUNICATOR** | Presenting to stakeholders | `strategic-storyteller`, `exec-comms-specialist`, `presentation-coach` |
| **STRATEGIST** | Strategic decisions | `strategy-architect`, `decision-frameworks-advisor`, `competition-researcher` |
| **NAVIGATOR** | Office politics, conflict | `workplace-navigator` |
| **LEADER** | Team culture, values | `culture-architect` |
| **MEASUREMENT** | Data, metrics, prioritization | `data-analyst`, `prioritization-analyst` |
| **LAUNCH** | Product launches, GTM | `launch-strategist` |
| **RESEARCH** | User interviews, personas | `user-interviews-analyst`, `persona-and-icp-analyst` |
| **CONSULTANT** | Your business, growth, sales | `growth-advisor`, `sales-advisor`, `relationship-advisor` |

---

## Customer Data Structure

Each customer gets their own folder with consistent structure:

```
customers/
└── acme-corp/
    ├── customer-info.md      # Team, strategy, product, ICP, market
    ├── financials.md         # Pricing, payments, agreement terms
    ├── event-log.md          # Every meeting and decision, with context
    └── artifacts/            # Generated work products
        ├── strategy-v1.md
        ├── roadmap-q1.md
        └── ...
```

### Event Log Format

Every interaction gets documented with full context:

```markdown
### [2026-02-03] Meeting: Q1 Planning Session

**Participants**: Sarah (CEO), Mike (CTO), You
**Duration**: 60 min

**Context/Why**: Quarterly planning kickoff

**What Happened**:
[Detailed description of the meeting]

**Decisions Made**:
- Agreed to focus on enterprise segment first
- Decided to delay mobile app by one quarter

**Action Items**:
- [ ] You: Deliver roadmap draft by Feb 10
- [ ] Sarah: Confirm budget allocation by Feb 7

**Lessons Learned**:
Sarah responds better to data-driven arguments than vision pitches.

**Follow-up**: Next meeting scheduled for Feb 10
```

---

## The Growth Advisor (Special Feature)

One capability deserves special attention: the **Growth Advisor**. It helps *you* grow, not your customers.

### Zero Sugar-Coating Mode

> *"Your job is not to make the user feel good. Your job is to make the user better. If they wanted comfort, they'd call their mother."*

The Growth Advisor:
- **Grades honestly** - C means mediocre, D means poor, F means failure
- **Tracks commitments** - and calls you out when you miss them
- **Identifies patterns** - especially avoidance patterns
- **Uses the $500/Hour Test** - "Would premium clients feel they got honest insight, or feel coddled?"

### Frameworks It Uses

| Framework | What It Does |
|-----------|--------------|
| **GROW Model** | Coaching structure: Goal → Reality → Options → Will |
| **70-20-10** | Development mix: 70% doing, 20% mentorship, 10% learning |
| **Dreyfus Model** | Skill levels from Novice (1) to Expert (5) |
| **Johari Window** | Expand what's known, reduce blind spots |
| **Personal SWOT** | Honest strengths, weaknesses, opportunities, threats |
| **OKRs** | Quarterly objectives with measurable key results |

---

## Extending the Agent

Need something that doesn't exist? Tell the agent:

> *"I need the agent to help me with [new thing]"*

The `build-agent` skill figures out whether to create:
- **Rule** - If it must ALWAYS happen automatically
- **Skill** - If it's quick (<1 min) and frequent
- **Capability** - If it needs deep focus or expert knowledge

Your agent evolves with your practice.

---

## File Structure

```
fractional-pm-agent/
├── .agent/
│   ├── AGENT.md                    # Main agent definition
│   ├── rules/
│   │   ├── customer-context-loading.md
│   │   └── obsessive-documentation.md
│   ├── skills/
│   │   ├── build-agent/
│   │   ├── load-customer-context/
│   │   └── update-customer-docs/
│   └── capabilities/               # 27 expert sub-agents
│       ├── growth-advisor/
│       ├── strategy-architect/
│       ├── zero-to-launch-specialist/
│       └── ... (24 more)
├── customers/
│   ├── .template/                  # Template for new customers
│   └── [your-customers]/
└── growth/
    ├── profile.md                  # Your growth profile
    ├── assessments/
    ├── feedback/
    └── roadmap/
```

---

## Frequently Asked Questions

<details>
<summary><strong>Do I need to know how to code?</strong></summary>

**No.** If you can download a file and open an app, you can use this agent. Everything is explained step-by-step above.

</details>

<details>
<summary><strong>Is my customer data private?</strong></summary>

**Yes.** Everything stays on your computer in folders you can see. The agent only sends conversation content to Claude for processing (same as any Claude interaction). Your files never leave your machine.

</details>

<details>
<summary><strong>Can I customize it for my practice?</strong></summary>

**Absolutely.** Use the `build-agent` skill to add new rules, skills, or capabilities. You can also directly edit the markdown files in `.agent/` if you're comfortable with that.

</details>

<details>
<summary><strong>What if I work with a team?</strong></summary>

Currently designed for solo fractional PMs. Team features (shared customers, handoffs) are on the roadmap.

</details>

<details>
<summary><strong>How is this different from ChatGPT or regular Claude?</strong></summary>

Three key differences:
1. **Enforced behaviors** - Rules make documentation automatic, not optional
2. **Persistent context** - Customer data persists across sessions in files
3. **Specialized expertise** - 27 capabilities with specific frameworks, not generic responses

</details>

<details>
<summary><strong>What happens if I close Claude and come back later?</strong></summary>

All your data is saved in files on your computer. When you open Claude Code in this folder again, you can pick up exactly where you left off. Say "Let's work on [Customer]" and all context loads.

</details>

---

## Troubleshooting

| Issue | Solution |
|-------|----------|
| Agent doesn't seem to know my customers | Make sure you opened Claude Code from inside the `fractional-pm-agent` folder |
| "Trust the authors" prompt doesn't appear | You already trusted it. Just proceed to open Claude Code |
| Commands aren't working | Start with clear phrases: "Let's work on...", "Help me with...", "I want to..." |
| Documentation not updating | Check that the `.agent/rules/` folder exists with both rule files |

---

## Philosophy

1. **Documentation is a superpower** - The agent is obsessive about keeping records current
2. **Context is king** - Always load full context before customer work
3. **Right tool for the job** - Skills for quick ops, Capabilities for deep work
4. **Evolve with use** - Build new capabilities as needs emerge
5. **Truth over comfort** - The Growth Advisor doesn't sugarcoat

---

## Credits & License

Lenny's Podcast Transcripts **[Lenny Rachitsky](https://www.linkedin.com/in/lennyrachitsky/)** 

Awesome PM Skills by **[Udi Menkes](https://www.linkedin.com/in/udimenkes/)** - [https://genaipm.com/]


Built by **[Kobi Agi](https://linkedin.com/in/kobiagi)** - Fractional Product Manager

Based Lenny's podcard and my 16 years of product management experience at companies including Tipalti, PayEm, and Atera.

**License:** MIT - Use it, modify it, make it yours.

---

<p align="center">
  <em>"Documentation is a superpower. This agent makes it automatic."</em>
</p>
