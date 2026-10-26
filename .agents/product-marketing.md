# Product Marketing Context

**Document version:** v1
**Last updated:** 2026-10-26

> This context describes the independent `JayLunia/trading-agent-skills` fork,
> not the original project's author or business. Product details are grounded in
> the repository. Audience needs, switching dynamics, and channel priorities are
> working assumptions; no customer interviews or marketing tests were provided.

## Product Overview
**One-liner:** A free, open-source collection of structured trading and investing workflows that can be installed in several AI agents.
**What it does:** Packages market research, screening, portfolio review, trade planning, risk checks, journaling, and strategy research into modular `SKILL.md` folders with supporting scripts and references. Helps an investor structure analysis and review; it does not decide or execute trades.
**Product category:** Open-source AI agent skills; trading and investing workflow toolkit.
**Product type:** Open-source software and downloadable agent-skill packages.
**Business model:** Free, MIT-licensed upstream content retained by this fork. Some workflows optionally require paid third-party market-data services. No paid product or revenue model is established for this fork.

## Target Audience
**Target companies:** Not applicable; individual users are the working assumption.
**Decision-makers:** Self-directed individual investors and traders choosing their analysis workflow and AI agent.
**Primary use case:** Add repeatable market-analysis, risk-review, and journaling workflows to an agent without treating it as a trading authority.
**Jobs to be done:**
- Structure a quick market or portfolio review.
- Screen and compare trade candidates with explicit criteria.
- Record decisions and review outcomes consistently.
**Use cases:** Investors combining long-term holdings with a disciplined swing-trading satellite; traders who want a no-paid-data-API starting path; technically comfortable users who can configure local scripts or integrations.

## Personas
| Persona | Cares about | Challenge | Value we promise |
|---------|-------------|-----------|------------------|
| Time-constrained self-directed investor (assumption) | A useful routine, understandable risk, low setup burden | Repeats market checks and portfolio decisions inconsistently | Structured workflows and a documented no-API starting path |
| Agent-curious trader (assumption) | Using an existing AI agent without rebuilding every workflow | Skills are fragmented by agent and integrations vary | Shared skill folders plus agent-specific installation instructions; runtime compatibility is disclosed per capability |

## Problems & Pain Points
**Core problem:** Investors who want a repeatable review process may rely on ad hoc prompts, scattered tools, or memory.
**Why alternatives fall short:** These are hypotheses, not validated customer findings.
- General-purpose agents do not arrive with this repository's specific workflow manifests and trading checklists.
- Copying one-off prompts between tools makes it harder to version a process or see required inputs.
**What it costs them:** Potentially wasted setup time and inconsistent review; no quantified cost is known.
**Emotional tension:** Concern about missing a risk factor, while not wanting to delegate financial judgment to an AI.

## Competitive Landscape
**Direct:** No direct competitor has been validated for this fork. Comparable open-source trading skills or agent-workflow repositories should be researched before making comparative claims.
**Secondary:** General-purpose AI agents and investment research platforms can support analysis, but their workflow scope and human-decision boundaries differ by product.
**Indirect:** Personal spreadsheets, saved prompts, and manual checklists can provide structure without installing a skill collection.

## Differentiation
**Key differentiators:**
- 74 skills are listed in the inherited upstream catalog, with workflows, skillsets, an index, and helper scripts.
- This fork documents install paths for Claude Code, Codex, GitHub Copilot, Cursor, and Gemini CLI.
- A no-paid-data-API starter path and explicit human review boundary are documented upstream.
**How we do it differently:** Keep one shared `SKILL.md` source and document agent-specific locations while distinguishing instruction portability from runtime integrations.
**Why that's better:** Users can reuse compatible instructions across agents and see when API keys, MCP servers, Python, or client-specific features are required.
**Why customers choose us:** Not yet evidenced by customer or usage research. Working hypothesis: users value a broad, inspectable workflow library and are comfortable configuring their own agent.

## Objections
| Objection | Response |
|-----------|----------|
| Will every skill work the same in my agent? | No universal runtime claim: the folders use the shared format, but MCP, API, browser, and Claude-specific features may need adaptation. See the compatibility guide. |
| Will this tell me what to buy or make money? | No. It structures analysis and review; it is not a signal service or promise of profitability. |
| Do I need paid data? | Not for the documented no-API starter path. Other skills list their integration requirements. |

**Anti-persona:** Anyone looking for guaranteed returns, an autonomous broker bot, personalized financial advice, or an agent that makes consequential decisions without human review.

## Switching Dynamics
**Push:** Repetitive, scattered analysis and prompts (assumption).
**Pull:** Modular workflows, documented inputs, and several agent installation paths.
**Habit:** Existing watchlists, spreadsheets, prompts, and established routines.
**Anxiety:** Setup effort, data accuracy, agent-specific behavior, and risk of over-trusting generated analysis.

## Customer Language
**How they describe the problem:** No verbatim customer research has been collected.
**How they describe us:** No user descriptions or testimonials have been collected.
**Words to use:** structured, review, screen, risk-aware, human-reviewed, open-source, agent skill.
**Words to avoid:** guaranteed, profitable, alpha, autonomous trading, universally compatible, financial advice.
**Glossary:**
| Term | Meaning |
|------|---------|
| Skill | A folder of `SKILL.md` instructions and optional supporting resources |
| Workflow | An ordered process that combines skills for a user goal |
| Integration | A third-party API, MCP server, or agent capability a workflow may require |

## Brand Voice
| Attribute | Means | Doesn't mean | Example line |
|-----------|-------|--------------|--------------|
| Practical | Explain the workflow and next step plainly | Oversell outcomes | "New users should start with one of these operational workflows." |
| Risk-aware | State limitations before users infer certainty | Alarmist or vague warnings | "This is not a signal service or a promise of profitability." |
| Transparent | Separate shared format support from tested runtime support | Claim compatibility without evidence | "Agent-format compatibility does not guarantee that every skill's integrations or scripts work unchanged in every agent." |

**Tone by context:**
- Support: Concrete setup steps and exact requirements.
- Launch: Show the problem and a runnable workflow; avoid performance claims.
- Errors: State the missing input, key, package, or tool and the next check.
- Sales: Not applicable; this fork has no verified paid offer.
- Social: Share a useful workflow or sample, label fictional examples, and invite specific feedback.
**Terms we own:** None established.
**Never use (and why):** "guaranteed returns," "AI trading bot," or "works everywhere" because they imply outcomes or compatibility not supported by evidence.

## Proof Points
**Metrics:** The inherited catalog lists 74 skills. This describes source content, not installs, users, or performance.
**Customers:** None documented.
**Testimonials:** None documented.
**Value themes:**
| Theme | Proof |
|-------|-------|
| Modular workflow library | `skills/`, `workflows/`, `skillsets/`, `skills-index.yaml` in the upstream repository |
| Risk-first, human-reviewed use | Upstream README and workflow documentation |
| Multi-agent setup | This fork's `docs/agent-compatibility.md`; installation is documented, not validated end-to-end for every workflow |

## Goals
**Business goal:** Build useful discovery and contribution around a clearly attributed multi-agent fork; no commercial goal is established.
**Conversion action:** Visit the repository, install one appropriate skill, or contribute a compatibility report.
**Current metrics:** GitHub stars, clones, installs, contributors, and retention are not yet recorded as a baseline.

## Learnings
| Date | Learning | Evidence | Applies to | Status |
|------|----------|----------|------------|--------|
| | | | | |

## Changelog
*Newest first. One line per revision: what changed and why.*
- v1 (2026-10-26) — Established the Trading Agent Skills name and multi-agent positioning; marked audience assumptions and unmeasured proof points for future validation.
