# Install Trading Skills Across AI Agents

The skill folders under `skills/` are the shared source. Each folder contains a
`SKILL.md` and may also include scripts, references, and assets. Agents that
implement the open Agent Skills format can read the same source; only the
installation location or command changes.

This guide covers Claude Code, OpenAI Codex, GitHub Copilot, Cursor, and Gemini
CLI. It documents how to install skills and does not claim that every workflow
has been exercised in each product. A skill can also depend on Python, a data
provider API key, an MCP server, or client tools such as a browser. Check that
skill's `SKILL.md` and the [skills index](../skills-index.yaml) before use.

## 1. Get the source

```bash
git clone https://github.com/JayLunia/trading-agent-skills.git
cd trading-agent-skills
```

You can install one skill or several. Replace `finviz-screener` below with a
directory name under `skills/`. Avoid copying the whole collection unless you
want every skill available to your agent.

## 2. Choose your agent

### OpenAI Codex

Install a personal skill into `~/.agents/skills/`, or a project skill into
`.agents/skills/` in your project:

```bash
mkdir -p ~/.agents/skills
cp -R skills/finviz-screener ~/.agents/skills/
```

For a project-local copy, run the same commands from your project root and
replace `~/.agents/skills` with `.agents/skills`. Start a new Codex session or
reload skills if needed. See the [Codex skills guide](https://developers.openai.com/codex/skills/).

### GitHub Copilot

For a project skill, copy it into `.github/skills/` in the repository where you
use Copilot:

```bash
mkdir -p /path/to/your-project/.github/skills
cp -R skills/finviz-screener /path/to/your-project/.github/skills/
```

For a personal skill, use `~/.copilot/skills/` instead. GitHub also documents
`.agents/skills/` as a project location on supported Copilot surfaces. Run
`/skills reload` in Copilot CLI if the skill list needs refreshing. See
[GitHub's skill setup guide](https://docs.github.com/en/copilot/how-tos/copilot-on-github/customize-copilot/customize-cloud-agent/add-skills).

### Cursor

Cursor supports project skills in `.agents/skills/` and `.cursor/skills/`. Its
compatibility locations also include Claude and Codex skill folders. To use a
project-local copy:

```bash
mkdir -p /path/to/your-project/.agents/skills
cp -R skills/finviz-screener /path/to/your-project/.agents/skills/
```

Or copy into `~/.cursor/skills/` for local user-level use. Cursor notes that
local user skills do not automatically sync to Cloud Agents or remote workers;
put the skill in the project repository for those environments. See
[Cursor Agent Skills](https://cursor.com/docs/skills).

### Gemini CLI

Gemini CLI can install a skill from this Git repository directly. Choose
`--scope user` for your account or `--scope workspace` for the current project:

```bash
gemini skills install https://github.com/JayLunia/trading-agent-skills.git \
  --path skills/finviz-screener --scope user
```

To install a workspace skill, run the command from your project and change the
scope to `workspace`. Review the requested skill before accepting the install.
See [Gemini CLI Agent Skills](https://geminicli.com/docs/cli/skills/).

### Claude Code

Copy the folder into `~/.claude/skills/` for personal use or `.claude/skills/`
inside your project:

```bash
mkdir -p ~/.claude/skills
cp -R skills/finviz-screener ~/.claude/skills/
```

Claude Code also loads project skills from `.claude/skills/`. See the
[Claude Code Skills guide](https://code.claude.com/docs/en/skills).

### Claude Web App

The `.skill` archives in `skill-packages/` are ZIP-formatted uploads for
Claude's web app. Download the skill you want and upload it in Claude's Skills
settings. The archive format is not a universal agent installer; use the
directory instructions above for coding agents.

## 3. Check runtime requirements

Installing `SKILL.md` gives an agent the workflow instructions. It does not
install API credentials, MCP servers, Python dependencies, browser access, or
broker integrations. Before running a skill:

1. Read its `SKILL.md`, especially its integrations and setup notes.
2. Check `skills-index.yaml` for required and optional integrations.
3. Configure the corresponding API key or tool in your chosen agent, if needed.
4. Start with a no-API workflow if you are exploring the repository. The
   [README](../README.md#no-api-key-starter-path) lists the current starter set.
5. Review all generated analysis yourself. These skills do not place orders or
   replace financial, tax, or legal advice.

Some features in the upstream project are specifically implemented for Claude
Code or rely on Claude-oriented tools. Those need an equivalent tool and a
separate check in another agent; copying a skill folder alone does not port
those integrations.

## Compatibility scope

| Capability | Status |
|---|---|
| Shared `SKILL.md` instructions and bundled text references | Portable where the agent supports Agent Skills |
| Install locations and commands in this guide | Documented from each vendor's current setup guide |
| Python helper scripts | Depend on that skill's Python version, packages, filesystem, and shell access |
| API and MCP integrations | Require matching credentials, server configuration, and tool names |
| Claude Web `.skill` upload | Claude-specific packaging and upload flow |
| Every skill's behavior across every agent | Not yet validated; verify the workflows you plan to use |

This project is an independent fork of
[tradermonty/claude-trading-skills](https://github.com/tradermonty/claude-trading-skills).
The upstream MIT license and attribution are retained.
