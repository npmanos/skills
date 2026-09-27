# Manos' Skills (`manos-skills`)

A curated collection of personal agent skills bundled as harness plugins for autonomous AI coding assistants. Built and maintained for [Antigravity CLI](https://github.com/google/antigravity) (`agy`) and [Claude Code](https://claude.ai/code).

---

## Overview

This repository provides reusable, test-hardened capabilities and procedural standards for AI agents. Rather than relying on fuzzy model instincts, each skill in this collection is developed using rigorous Test-Driven Development (TDD) for process documentation—tested under adversarial pressure scenarios to resist rationalization and ensure consistent compliance.

## Included Skills

| Skill | Description | Location |
|---|---|---|
| **`conventional-commits`** | Enforces the Conventional Commits specification (`<type>(<scope>): <description>`), accurate semantic types, refactor vs. style distinctions, architectural scoping rules, and strict revert formatting. | [`skills/conventional-commits/SKILL.md`](skills/conventional-commits/SKILL.md) |

---

## Supported Harnesses & Setup

### Antigravity (`antigravity-cli`)

Install directly using the GitHub repository URL:

```bash
agy plugin install https://github.com/npmanos/skills
```

Antigravity automatically discovers skills within active plugins and exposes them through progressive disclosure—only injecting metadata initially and loading full skill documentation on demand.

### Claude Code

Install directly via the `claude` CLI:

```bash
claude plugin install https://github.com/npmanos/skills
```

Or run directly from inside a Claude Code session:

```text
/plugin install https://github.com/npmanos/skills
```

---

## Repository Structure

```
.
├── .claude-plugin/
│   └── plugin.json                          # Claude Code plugin manifest
├── plugin.json                              # Antigravity plugin manifest
├── README.md                                # Repository documentation
└── skills/
    └── conventional-commits/
        └── SKILL.md                         # Conventional Commits skill & decision trees
```
