# Organic Launch Kit

This kit is for sharing the `JayLunia/trading-agent-skills` fork. It positions
the work as an independently maintained, attributed adaptation of
[TraderMonty's Claude Trading Skills](https://github.com/tradermonty/claude-trading-skills).
Do not imply authorship of the upstream trading workflows or claim that this
fork has been tested end-to-end across every agent.

## Positioning

**Short description:** Open-source trading and investing workflows for Claude,
Codex, GitHub Copilot, Cursor, and Gemini CLI.

**Search phrases to use naturally:** agent skills for trading, AI agent trading
workflows, market analysis skills, portfolio review workflow, trading journal
AI skill, Codex trading skills, Gemini CLI skills.

**Proof available today:** the upstream catalog lists 74 skills; this fork adds
agent-specific install instructions, GitHub topics, and clear compatibility
limits. The skill library and its MIT license remain credited to the upstream
project.

**Core message:** use an AI agent to make a review process more structured,
while keeping the investor responsible for decisions. Do not promise returns,
signals, autonomous execution, or universal runtime compatibility.

## Launch post drafts

### Short post

I made an independently maintained, multi-agent fork of TraderMonty's open
source Claude Trading Skills. It documents how to install the shared trading
and investing workflows in Codex, Copilot, Cursor, and Gemini CLI, while
calling out where APIs, MCP servers, or Claude-specific tools still matter.

It is for structured research and review—not trade signals or automated
orders. The original skills and MIT license are credited.

Repo: https://github.com/JayLunia/trading-agent-skills

### Longer post

AI trading demos often jump straight to “what should I buy?” I wanted a more
careful starting point: repeatable market reviews, screening criteria, risk
checks, trade journals, and post-trade learning that leave decisions with the
investor.

I’ve forked and credited TraderMonty's MIT-licensed Claude Trading Skills and
added a multi-agent installation guide for Codex, GitHub Copilot, Cursor, and
Gemini CLI. The repository lists 74 skills upstream. The folders share the
`SKILL.md` format, but integrations still vary by agent; the guide spells out
that boundary.

This is an open-source research and process toolkit, not financial advice,
trade recommendations, or an automated trading bot. Feedback on a specific
skill/agent combination is useful.

Repo: https://github.com/JayLunia/trading-agent-skills

## Four-week content sequence

| Week | Useful demo | Evidence to include | Call to action |
|------|-------------|--------------------|----------------|
| 1 | Run the no-paid-data-API market review workflow | The exact required skills, inputs, and an illustrative output labeled fictional | Try the README starter path |
| 2 | Show how position sizing turns a risk limit into a calculation | Formula, assumptions, and a small reproducible example | Review or improve the calculation workflow |
| 3 | Demonstrate a closed-trade journal and postmortem loop | A fictional trade record and the lessons the workflow does and does not infer | Share a gap or edge case |
| 4 | Compare where one `SKILL.md` can be installed across agents | The same folder and vendor-specific path, plus one real integration limitation | Report a tested agent/skill combination |

Publish one practical walkthrough at a time. Link to the repository and the
relevant skill; identify fictional examples; credit the upstream author. On
community forums, answer an existing question or share a directly relevant
workflow and follow that community's self-promotion rules.

## Track progress

Record a starting date and weekly GitHub stars, unique visitors, clones,
issues, pull requests, and reported agent/skill combinations. Add UTM tags to
links for channels where they are allowed. Treat stars and clicks as discovery
signals, not proof that users installed a skill or improved trading results.

No channel baseline, audience research, conversion data, or campaign results
are currently available. Add learnings to `.agents/product-marketing.md` only
after a result is supported by a completed test or repeated evidence.
