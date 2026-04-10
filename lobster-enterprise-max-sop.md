# Lobster Enterprise Max SOP v1.0

## Purpose

Zero-Computer agent funnel automation using Model Council + Comet.

## Naming Convention

All files: `lobster_[project_code]_[YYYYMMDD]_[type].ext`

Type suffixes:
- `_sop.md` -> standard operating procedure
- `_action_list.json` -> executable plan
- `_research.md` -> Council raw output
- `_report.md` -> Comet execution report
- `_prompt.md` -> backup prompt

## Core Flow (3 steps, repeatable forever)

### Step 1: Model Council
Paste the Council Prompt (see `council-prompts.md`) with your project code.
Council outputs: Markdown report + JSON Action List + Comet Prompt.

### Step 2: Save to My Files
Save JSON as `lobster_[code]_[date]_action_list.json`.
Save report as `lobster_[code]_[date]_research.md`.

### Step 3: Comet Shortcut
Type `/execute-lobster-funnel [project_code]`.
Comet reads JSON, executes step-by-step, outputs report.

## Roles

| Role | Tool | Responsibility |
|------|------|----------------|
| Strategy Brain | Model Council | Reasoning, risk, architecture, Action List |
| Execution Body | Comet | Read JSON, cross-tab ops, report |
| Trigger | Comet Shortcuts | Repeatable one-click workflows |
| Memory | Spaces + Memory | Accumulate project context |

## Permission Checklist (Enterprise Admin)

- Comet Assistant: only allow necessary domains
- Block Comet from financial systems and sensitive DBs
- Review Audit Logs after each execution
- Rotate API keys monthly

## Common Scenarios

1. Lead funnel automation (HighLevel + Vercel + ECPay)
2. Competitive intelligence daily update
3. Content production + distribution pipeline
4. Auto report generation and delivery
5. OpenClaw agent deployment orchestration

## Changelog

- 2026-04-11 v1.0 Initial release
