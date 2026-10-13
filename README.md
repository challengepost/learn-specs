# Learn AR with SPECS: Devpost Learn skill pack

The skill pack for **Learn AR with SPECS** on Devpost Learn. Works in any coding agent that supports skills (see skills.sh): Claude Code, Codex, Cursor, and others.

## Order of steps

1. **Create a SPECS project.** In Lens Studio, choose **SPECS**, then **Base Template**, then **File > Save As**. Lens Studio saves it as its own folder.
2. **Start your coding agent in that project folder** (the one with the `.esproj` and `.mcp.json` files), with Lens Studio open. That's where the Lens Studio tools load.
3. **Install CLAD** for your agent, following Snap's guide. In Claude Code:
   ```
   /plugin marketplace add https://github.com/lens-studio-devs/ls-extensions.git
   /plugin install ls-clad@ls-extensions
   /reload-plugins
   ```
   Guides for Claude Code, Codex and Cursor: https://developers.specs.com/docs/clad
4. **Install the skill pack** in the same folder:
   ```
   npx skills add challengepost/learn-specs --all -y
   ```
5. **Say `plan-lens`.** About 20 to 30 minutes. It writes `devpost/design-brief.md`.
6. **Clear the chat and fire it off:**
   > Read devpost/design-brief.md and build it for SPECS. Follow the brief closely. Get the basic flow working first, then add detail. Write and run LEAF tests for each done criterion, and tell me which pass.

The Quick Start on the resources page walks through steps 1 to 4: https://learn-specs.devpost.com/resources

The brief ends with an **After the build** section: how to judge your Lens in the preview, iterate with design notes, and get ready to submit. Publish the Lens project folder, with `devpost/` inside it, as your public repo.

## Layout

```
skills/plan-lens/SKILL.md          the skill
skills/plan-lens/templates/        the design brief template
skills/plan-lens/references/       AR design rules and preview limits the agent reads
```
