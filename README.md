# Learn Specs — skills

Skill pack for the **Learn AR With SPECS** hackathon on Devpost Learn, packaged as agent skills. Works in any harness that reads `SKILL.md` (Claude Code, Codex, Cursor, …).

> Work in progress — `1-start` is a placeholder until the curriculum is built.

## Install

```
npx skills add challengepost/learn-specs --all -y
```

Prerequisites: **node** and **git** installed, and an empty folder set aside for your project.

Invoke each skill by name in your agent, starting with `1-start`.

## Layout

```
skills/<name>/SKILL.md          the skill
skills/<name>/templates/        document templates the skill fills in
skills/<name>/references/       deeper material the skill reads on demand
```
