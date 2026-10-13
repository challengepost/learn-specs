# Learn AR with SPECS: Devpost Learn skill pack

The skill pack for **Learn AR with SPECS** on Devpost Learn. Works in any coding agent that supports skills (see skills.sh): Claude Code, Codex, Cursor, and others.

## Install

From the folder you've set aside for your project:

```
npx skills add challengepost/learn-specs --all -y
```

Set up Lens Studio, the Lens Studio MCP and CLAD first. The Quick Start is on the hackathon's resources page: https://learn-specs.devpost.com/resources

## The skill

| Skill | What happens | Output |
|---|---|---|
| `plan-lens` | A short interview about your idea, checked against AR design best practices and what Lens Studio's preview can do | `devpost/design-brief.md` |

Start your agent in your project folder and say **plan-lens**. It takes about 20 to 30 minutes.

When your brief is approved, create your Lens Studio project if you haven't yet: choose **SPECS**, then **Base Template**, and use **File > Save As** to save it in the same folder as your `devpost/` folder. Then clear the chat (or start a new one) and point CLAD at the brief:

> Read devpost/design-brief.md and build it for SPECS. Follow the brief closely. Get the basic flow working first, then add detail. Write and run LEAF tests for each done criterion, and tell me which pass.

The brief ends with an **After the build** section: how to judge your Lens in the preview, iterate with design notes, and get ready to submit. Keep the `devpost/` folder in your public repo.

## Layout

```
skills/plan-lens/SKILL.md          the skill
skills/plan-lens/templates/        the design brief template
skills/plan-lens/references/       AR design rules and preview limits the agent reads
```
