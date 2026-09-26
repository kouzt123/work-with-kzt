# work-with-kzt

Install this skill to consult Zhitao's AI counterpart on anything.

Zhitao is a TikTok Creative Strategy Manager with 8 years of overseas growth experience across creative strategy, paid acquisition, creator/KOL marketing, and creative production. This repo packages his perspective and working style into an installable AI counterpart: bring it a question, decision, or real problem and work through it with Zhitao's way of thinking.

## What It Does

- Offers Zhitao's perspective as an AI counterpart for open-ended questions and decisions.
- Pressure-tests product, market, and creative strategy.
- Diagnoses ads, hooks, creator scripts, landing pages, and campaign logic.
- Reviews creator shortlists and briefs without turning into ad-speak.
- Designs growth and creative automation workflows using whatever tools are available in the host environment.
- Keeps confidential employer IP out of scope.

The skill is intentionally modular. `SKILL.md` handles persona and routing; detailed methods live in `references/` and are loaded only when relevant.

## Install for Codex

Personal install:

```bash
mkdir -p ~/.agents/skills
git clone https://github.com/kouzt123/work-with-kzt.git ~/.agents/skills/work-with-kzt
```

Repo-scoped install:

```bash
mkdir -p .agents/skills
git clone https://github.com/kouzt123/work-with-kzt.git .agents/skills/work-with-kzt
```

Use it in Codex:

```text
$work-with-kzt I want to consult Zhitao about this decision: ...
```

## Install for Claude Code

Personal install:

```bash
mkdir -p ~/.claude/skills
git clone https://github.com/kouzt123/work-with-kzt.git ~/.claude/skills/work-with-kzt
```

Repo-scoped install:

```bash
mkdir -p .claude/skills
git clone https://github.com/kouzt123/work-with-kzt.git .claude/skills/work-with-kzt
```

Use it in Claude Code:

```text
/work-with-kzt I want to consult Zhitao about this decision: ...
```

## First Prompts to Try

- "I want Zhitao's take on a decision I am weighing. Help me think it through."
- "Give me a product link and target market; map the creative strategy and first tests."
- "Paste an ad, landing page, or script; diagnose the hook, proof, friction, and next iteration."
- "Send a creator shortlist or brief; vet fit, red flags, and brief quality."

## Module Map

- `creative-strategy.md`: product, market, positioning, angle systems, GTM messaging, test design.
- `creative-production.md`: scripts, briefs, shot lists, production loops, asset iteration.
- `influencer-marketing.md`: creator vetting, brief QC, creator script diagnosis.
- `ad-analysis.md`: ad teardown, hook diagnosis, proof, claims, funnel friction.
- `automation.md`: growth workflows, reporting loops, prompt ops, tool-assisted execution.
- `investing.md`: easter egg, only when asked.
- `humor.md`: easter egg, only when asked.

## Sources

- Codex Agent Skills: https://developers.openai.com/codex/skills
- Claude Code Skills: https://code.claude.com/docs/en/skills

## IP Boundary

This skill is built from generic, portable working judgment. It must not include employer-internal frameworks, confidential data, unreleased product details, internal tools, or nonpublic campaign examples.
