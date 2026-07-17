# The Ghost Agent Course — Applied Lab Guides

In-depth, self-contained guides for the ten applied labs of **The Ghost Agent Course** by [inference.ai](https://inference.ai). Each lab teaches you to **operate Ghost** — a ready-to-work AI agent — by prompting it: you don't build an agent from scratch, you direct, debug, guard, and deploy one. Every lab ends with a real artifact you can show.

Each guide is a standalone PDF, sized for students to follow and for proctors to run a session from.

## The labs

### Part I · Operate a single agent
| # | Lab | Difficulty | Guide |
|---|-----|-----------|-------|
| 00 | Setup & Debugging Toolkit | Onboarding | [PDF](lab-00-setup-and-debugging.pdf) |
| 01 | Memory → Living Site | Easiest | [PDF](lab-01-memory-living-site.pdf) |
| 02 | Daily Briefing Agent | Easy+ | [PDF](lab-02-daily-briefing-agent.pdf) |
| 03 | Research → Published Asset | Medium | [PDF](lab-03-research-published-asset.pdf) |
| 04 | Stateful Monitor + Permission Policy | Hard | [PDF](lab-04-stateful-monitor-policy.pdf) |
| 05 | Deploy a Shared Operator | Hard | [PDF](lab-05-shared-operator.pdf) |

### Part II · Run the functions of a business
| # | Lab | Difficulty | Guide |
|---|-----|-----------|-------|
| 06 | Data → Decision | Medium | [PDF](lab-06-data-to-decision.pdf) |
| 07 | Growth Engine | Medium | [PDF](lab-07-growth-engine.pdf) |
| 08 | Inbound Responder | Medium | [PDF](lab-08-inbound-responder.pdf) |
| 09 | Multi-Agent Operation | Hardest (2 sessions) | [PDF](lab-09-multi-agent-operation.pdf) |

## How each guide is structured

Every lab guide contains: learning objectives · why the lab exists · prerequisites · a step-by-step build (with copy-paste prompts) · the failure modes to expect and how to debug them · a deliverable checklist · stretch goals · facilitator notes.

## The method — four beats, every lab

1. **Prime** — load context into Ghost's memory so it knows your world.
2. **Prompt** — give it the task in plain English.
3. **Break & steer** — the first output won't be perfect; debug it with a sharper instruction instead of starting over.
4. **Crystallize** — freeze the working version into a reusable workflow, and wrap it in a permission policy where stakes are real.

## Regenerating the PDFs

The PDFs are built from the HTML fragments in `content/` via `build.py` (uses Playwright/Chromium):

```
pip install playwright && playwright install chromium
python build.py
```

---
*The Ghost Agent Course · inference.ai · learn@inference.ai*
