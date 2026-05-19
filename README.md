# Martins Bash

AI trainer and researcher with a background in finance & data analysis. I evaluate how models reason under real-world conditions, stress test where failures fall into repeating patterns rather than random errors, and test the limits of what prompt architecture can actually enforce. The tooling I build extends that research: error classifiers that catch failure patterns before output is final, self-correcting agents that remember errors, systems that keep model behavior consistent under adversarial conditions, and more...

Active work lives in [`claude-skills`](https://github.com/martinsbash/claude-skills), a library of reliability-focused skills for Claude that started as infrastructure for my own research workflow. I also co-run Afro Creative Group, a web and creative agency.

---

## What I'm working on

**[`claude-skills`](https://github.com/martinsbash/claude-skills)**. A small library of composable skills for Claude Code and Claude agents. Each skill is a self-contained Markdown file that activates on specific triggers. The library currently covers six areas: recursive self-correction, production-grade prompt engineering, context compression for long sessions, session continuity across conversations, deep research with per-claim source verification, and a super-intelligent reasoning protocol for technical questions. I update these skills once every month. Each new version closes a specific gap that the previous one didn't solve. I write about what changed and why in each skill's SKILL.md.

**[`b2b-lead-gen-system`](https://github.com/martinsbash/b2b-lead-gen-system)**. A business discovery pipeline. Given search criteria, it finds matching businesses, scrapes the web, and pulls structured details and information I actually need to work with them: contact info, web presence, offering gaps, and anything worth knowing before outreach or underwriting. My primary use case right now is SMBs without working websites. The current repo only shows the general shape of the approach, but I'm actively building it into a proper end-to-end tool that produces agency-grade output rather than a sequence of intermediate scripts.

**[`trading-pattern-ai`](https://github.com/martinsbash/trading-pattern-ai)**. A pattern-recognition tool I'm building for my own trading workflow. Five chart patterns defined by liquidity engineering: structural setups, not visual ones. Monitors higher timeframes and fires an alert when the patterns alone signal that a high-probability configuration is taking shape. Still in early development, and currently running deep backtesting.

---

## Website development

Through Afro Creative Group, I design and build websites for small businesses. The focus is service businesses that don't have a working web presence, or have one that's outdated and costing them customers.

**What I build:**

- Landing pages and brand sites for local service businesses
- Multi-page sites with booking forms, lead capture, and advanced SEO
- E-commerce and online store setups
- Custom web apps and client portals
- Agency and portfolio sites
- Brand identity packages

**Stack on client projects:** React, JavaScript, Lovable for rapid prototyping.

The `b2b-lead-gen-system` repo powers the outreach side: it automatically finds and qualifies businesses that need this work, so the pipeline runs without spending 3 hours on manual research before every call.

**Client & Demo sites:**

| Site | Industry |
|------|----------|
| [Jaiye With Timi](https://jaiyewithtimi.lovable.app) | Content creator, weddings and events |
| [Carolyn's Beauty](https://carolynsbeauty.lovable.app) | Hair salon and beauty supply |
| [Lightspeed Energy](https://lightspeedenergy.lovable.app) | Energy sector |
| [Maya Retreat](https://mayaretreat.lovable.app/) | Wellness retreat |
| [Elegant Wedding Ed](https://elegantweddinged.lovable.app/) | Wedding and events |
| [Total Health & Sports](https://totalhealthsp.lovable.app/) | Health and fitness |
| [Brooklin Physio](https://brooklinphysio.lovable.app) | Physiotherapy |
| [Numiva Accounting](https://numivaacounting.lovable.app) | Accounting, Durham Region |
| [Crystal Event Decor](https://crystaleventdecor.lovable.app/) | Event decoration |

---

## How I think about AI systems

The claude-skills work has taught me that most AI failures aren't random. They're systematic. Claude tends to make the same categories of mistakes repeatedly: hallucinating specific details, missing edge cases, giving generic advice when specifics were needed, walking a single reasoning path when three were available. The interesting engineering question is not "how do I prevent any one mistake" but "how do I install mechanisms that catch entire categories of mistake even when the agent's attention lapses."

That framing shows up in `self-evolving-agent` v1.2 as a commit gate: every correction generates a test that blocks output if it fails; the check runs mechanically, not from memory. `prompt-engineering` makes the same point from a different angle: every prompt is two contracts at once, one for how Claude reasons and one for what the output must look like. In `oracle-research`, it becomes a source-ledger rule: every claim traces to a primary source before output ships, so gaps stay visible rather than papered over. And `superintelligence` runs the reasoning across seven parallel registers, because one fluent line of thinking isn't enough on a hard question.

I don't claim to have this figured out. I do claim to be iterating in public, with honest changelogs about what each version didn't solve. Full list in [`claude-skills`](https://github.com/martinsbash/claude-skills).

---

## Background

I came into tech from finance, and the two have been intertwined ever since. The finance background is where I learned to think about risk, precision, pattern recognition and compounding, which translates more directly to AI reliability than I expected going in. Worked on projects with Outlier as an Oracle-tier prompt engineer and reviewer, evaluating AI training data and model outputs for quality, reasoning, and failure modes. That research is where I started seeing the gaps in current AI models firsthand, so I started diving deep into how to close them, building and researching skills that make my own version of Claude significantly more reliable for the work I do

---

## Tech and tools I work in

Python for backends and scripting. JavaScript and React for client projects. Claude API and Claude Code for agent work. Apify for scraping. Lovable for rapid site prototyping. Pine Script and TradingView for the trading work. Almost everything I ship goes through my own `claude-skills` as part of the workflow.

---

## Currently learning

- Anthropic's own course catalog on Skilljar (Claude API, prompt engineering, tool use, Claude Code workflows, and agent design), working through them one at a time
- How to make LLM systems reliable in production: catching agent mistakes before they ship, testing for regressions, and knowing when the model is guessing vs. actually knowing something
- Multi-agent design: agents that coordinate, hand off work, and check each other's output
- Web and software development
- Quantitative finance as a rigorous framework for the pattern-recognition work in `trading-pattern-ai`

---

## Certifications

|  |  |
|---|---|
| **AI / Prompt Engineering**<br>• Claude 101 (Anthropic, 2026)<br>• OutlierEDU Prompt Engineering (Outlier, 2026)<br>• Advanced Prompt Engineering: Model Stumps (Outlier, 2026) | **AI Research and Benchmarking**<br>• OutlierEDU Expert to Data Architect (Outlier, 2026)<br>• OutlierEDU Reviewing 101 (Outlier, 2026) |
| **Finance and Capital Markets**<br>• ETF Proficiency Course (Learnedly, 2025)<br>• Financial History (Learnedly, 2025)<br>• Anti-Money Laundering 2025 (Learnedly, 2025) | **Blockchain and Fintech**<br>• Tokenization of Real-World Assets (Udemy, 2025)<br>• Blockchain and Fintech: Basics, Applications and Limitations (edX, 2025) |
| **Project and Program Management**<br>• CompTIA Project+ (CompTIA, 2021)<br>• Certification for Program and Project Managers, Entry Level (FAC-P/PM, EntryLevel, 2022)<br>• Microsoft Project Certification (Microsoft, 2021) | **PM Tools and Office**<br>• Microsoft Office Specialist: Microsoft Office 2016 (Certiport, 2023)<br>• Microsoft Project 2019 Essential Training (LinkedIn Learning, 2023)<br>• Visio 2021 Essential Training (LinkedIn Learning, 2023) |
| **Creative and Design**<br>• Adobe After Effects CC (Adobe, 2022) | **Professional Skills**<br>• Jobberman Soft-skills Training (Jobberman, 2021)<br>• EC-Council Customer Relationship Management (EC-Council, 2021) |

---

## Reach me

- [martinsbash@gmail.com](mailto:martinsbash@gmail.com)
- [Medium](https://medium.com/@martinsbash)
- [Afro Creative Group](https://afrocreativegroup.lovable.app)

I'm open to collaborations on AI agent work, fellowships, AI training, freelance engagements, and conversations with people working on similar problems.
