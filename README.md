# Martins Bash

AI researcher and benchmark engineer with a background in finance & data analysis. I evaluate how models reason under real-world conditions, stress test where failures fall into repeating patterns rather than random errors, and test the limits of what prompt architecture can actually enforce. The tooling I build extends that research: error classifiers that catch failure patterns before output is final, self-correcting agents that carry corrections across context resets, and systems that keep model behavior consistent under adversarial conditions and more...

Based in Toronto. Active work lives in [`claude-skills`](https://github.com/martinsbash/claude-skills), a library of reliability-focused skills for Claude that started as infrastructure for my own research workflow. I also co-run [Afro Creative Group](https://afrocreativegroup.lovable.app), a web and creative agency.

---

## What I'm working on

**[`claude-skills`](https://github.com/martinsbash/claude-skills)**. A small library of composable skills for Claude Code and Claude agents. Each skill is a self-contained Markdown file that activates on specific triggers. The library currently covers five areas: recursive self-correction, production-grade prompt engineering, context compression for long sessions, session continuity across conversations, and deep research with per-claim source verification. The flagship skill, `self-evolving-agent`, is on its third major iteration (v1.2). Each version closed a specific gap that the previous one didn't solve. I write about what changed and why in each skill's SKILL.md.

**[`b2b-lead-gen-system`](https://github.com/martinsbash/b2b-lead-gen-system)**. A business discovery pipeline. Given search criteria, it finds matching businesses and pulls the structured detail I actually need to work with them: contact info, web presence, ownership signals, offering gaps, anything worth knowing before outreach or underwriting. My primary use case right now is SMBs without working websites, but the engine is general. Built from daily operational use, not from a clean-sheet design. The current repo shows the general shape of the approach, and I'm actively rebuilding it into a proper end-to-end tool that produces agency-grade output rather than a sequence of intermediate scripts.

**[`trading-pattern-ai`](https://github.com/martinsbash/trading-pattern-ai)**. A pattern-recognition tool I'm building for my own trading workflow. Five chart patterns, defined by liquidity engineering rather than shape, with a planned backtest framework and alerting. In active development and honestly early.

**[`personal-productivity-system`](https://github.com/martinsbash/personal-productivity-system)**. An operating system for my own life: a Markdown-driven task manager, daily priority surfacing, and a night-before planning ritual. Open-sourced because the framework is reusable, not because my exact setup is.

---

## How I think about AI systems

The claude-skills work has taught me that most AI failures aren't random. They're systematic. Claude tends to make the same categories of mistakes repeatedly: hallucinating specific details, missing edge cases, giving generic advice when specifics were needed, walking a single reasoning path when three were available. The interesting engineering question is not "how do I prevent any one mistake" but "how do I install mechanisms that catch entire categories of mistake even when the agent's attention lapses."

That framing shows up in `self-evolving-agent` v1.2 as a commit gate: every correction rule ships with a paired regression test that runs before output is finalized, regardless of whether the agent remembered to check the rule in its head. It shows up in `prompt-engineering` as the behavioral-vs-output contract distinction: the same prompt has to govern both how Claude reasons and what the final output looks like. It shows up in `session-continuity` as a multi-query retrieval protocol because a single search almost never captures a full working state.

I don't claim to have this figured out. I do claim to be iterating in public, with honest changelogs about what each version didn't solve.

---

## Background

I came into tech from finance, and both sides still inform the work. The finance background is where I learned to think about risk, precision, and compounding, which translates more directly to AI reliability than I expected going in. Worked on projects with Outlier as an Oracle-tier benchmark engineer and reviewer, evaluating AI training data and model outputs for quality, reasoning, and failure modes. That research is where the patterns in `claude-skills` came from: reviews surface the same categories of failure repeatedly, and the skills exist because I needed a way to catch them systematically

---

## Tech and tools I work in

Python for backends and scripting. JavaScript and React for client projects. Claude API and Claude Code for agent work. Apify for scraping. Lovable for rapid site prototyping. Pine Script and TradingView for the trading work. Everything I ship goes through my own `claude-skills` as part of the workflow.

---

## Currently learning

- Anthropic's own course catalog on Skilljar (Claude API, prompt engineering, tool use, Claude Code workflows, and agent design), working through them one at a time
- How to make LLM systems reliable in production: catching agent mistakes before they ship, testing for regressions, and knowing when the model is guessing vs. actually knowing something
- Multi-agent design: agents that coordinate, hand off work, and check each other's output
- Web and software development broadly, with an emphasis on shipping client work end-to-end
- Quantitative finance as a rigorous framework for the pattern-recognition work in `trading-pattern-ai` (replacing the looser Smart Money Concepts chart-reading approach)

---

## Certifications

|  |  |
|---|---|
| **AI / Prompt Engineering**<br>• Claude 101 (Anthropic, 2026)<br>• OutlierEDU Prompt Engineering (Outlier, 2026)<br>• Advanced Prompt Engineering: Model Stumps (Outlier, 2026) | **AI Research & Benchmarking**<br>• OutlierEDU Expert to Data Architect (Outlier, 2026)<br>• OutlierEDU Reviewing 101 (Outlier, 2026) |
| **Finance & Capital Markets**<br>• ETF Proficiency Course (Learnedly, 2025)<br>• Financial History (Learnedly, 2025)<br>• Anti-Money Laundering 2025 (Learnedly, 2025) | **Blockchain & Fintech**<br>• Tokenization of Real-World Assets (Udemy, 2025)<br>• Blockchain and Fintech: Basics, Applications and Limitations (edX, 2025) |
| **Project & Program Management**<br>• CompTIA Project+ (CompTIA, 2021)<br>• Certification for Program and Project Managers, Entry Level (FAC-P/PM, EntryLevel, 2022)<br>• Microsoft Project Certification (Microsoft, 2021) | **PM Tools & Office**<br>• Microsoft Office Specialist: Microsoft Office 2016 (Certiport, 2023)<br>• Microsoft Project 2019 Essential Training (LinkedIn Learning, 2023)<br>• Visio 2021 Essential Training (LinkedIn Learning, 2023) |
| **Creative & Design**<br>• Adobe After Effects CC (Adobe, 2022) | **Professional Skills**<br>• Jobberman Soft-skills Training (Jobberman, 2021)<br>• EC-Council Customer Relationship Management (EC-Council, 2021) |

---

## Reach me

- [martinsbash@gmail.com](mailto:martinsbash@gmail.com)
- [Medium](https://medium.com/@martinsbash)
- [Afro Creative Group](https://afrocreativegroup.lovable.app)

I'm open to collaborations on AI agent work, fellowships, freelance engagements, and conversations with people working on similar problems.

---
