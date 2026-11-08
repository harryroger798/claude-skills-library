<div align="center">

# Claude Skills Library

### 2,507 production-ready Claude skills — free, MIT / Apache-2.0, one clone away.

[![Skills](https://img.shields.io/badge/skills-2%2C507-4E5380?style=for-the-badge)](https://github.com/harryroger798/claude-skills-library)
[![License](https://img.shields.io/badge/license-MIT%20%2F%20Apache--2.0-12153A?style=for-the-badge)](#-license)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen?style=for-the-badge)](#-contributing)
[![Stars](https://img.shields.io/github/stars/harryroger798/claude-skills-library?style=for-the-badge&color=4E5380)](https://github.com/harryroger798/claude-skills-library/stargazers)
[![Curated by](https://img.shields.io/badge/curated%20by-geowallah.com-4E5380?style=for-the-badge)](https://geowallah.com)

**Curated and maintained by [geowallah.com](https://geowallah.com)**

[Quick start](#-quick-start) · [For AI agents](#-for-ai-agents) · [What's inside](#-whats-inside) · [Structure](#-structure) · [Contributing](#-contributing) · [License](#-license)

</div>

---

## Why this repo

The paid "2,000+ Claude skills" bundles are just free, permissively-licensed skills repackaged. This repo is the real thing: **2,507 skills, deduplicated, organized, machine-readable, and free** — pulled from the best open-source collections and kept under their original MIT / Apache-2.0 licenses.

- **2,507 skills** in one clone
- **Machine-readable** — `manifest.json` indexes every skill (name, description, path, raw URL)
- **Agent-first** — any AI can fetch one skill by raw URL or read the whole manifest
- **No lock-in** — plain `SKILL.md` folders, the open Agent Skills standard
- **Licenses kept** — every source repo credited in `CREDITS.txt`

## Quick start

```bash
# clone everything
git clone https://github.com/harryroger798/claude-skills-library.git

# use one skill (personal)
cp -r claude-skills-library/skills/<folder> ~/.claude/skills/

# use one skill (per project)
cp -r claude-skills-library/skills/<folder> .claude/skills/
```

**Claude.ai (web):** zip a skill folder and upload it under **Customize → Skills**.
**Claude Code:** drop the folder into `~/.claude/skills/` or `.claude/skills/` — Claude loads it automatically when a task matches its `description`.

## For AI agents

This repo is built to be read by agents.

| Resource | URL |
|---|---|
| Manifest (all skills) | `https://raw.githubusercontent.com/harryroger798/claude-skills-library/main/manifest.json` |
| One skill (raw) | `https://raw.githubusercontent.com/harryroger798/claude-skills-library/main/skills/<folder>/SKILL.md` |
| Repo | `https://github.com/harryroger798/claude-skills-library` |

`manifest.json` shape:

```json
{
  "name": "Claude Skills Library",
  "count": 2507,
  "skills": [
    { "name": "...", "folder": "...", "description": "...", "path": "skills/<folder>/SKILL.md", "raw": "https://raw.githubusercontent.com/..." }
  ]
}
```

## What's inside

| Source | Skills |
|---|---|
| mohitagw15856/pm-claude-skills | 1,330 |
| alirezarezvani/claude-skills | 443 |
| wshobson/agents | 185 |
| K-Dense-AI/scientific-agent-skills | 176 |
| tradermonty/claude-trading-skills | 74 |
| paperclipai/paperclip | 68 |
| Jeffallan/claude-skills | 64 |
| nanocoai/nanoclaw | 62 |
| coreyhaines31/marketingskills | 41 |
| JimLiu/baoyu-skills | 22 |
| alchaincyf/nuwa-skill | 16 |
| anthropics/skills (Apache-2.0) | 15 |
| OthmanAdi/planning-with-files | 6 |
| zLanqing/codex-claude-academic-skills | 5 |
| **Total (deduplicated)** | **2,507** |

## Structure

```
claude-skills-library/
├── skills/
│   └── <folder>/
│       ├── SKILL.md          # required: YAML frontmatter (name, description) + instructions
│       ├── scripts/          # optional: helpers the skill can run
│       ├── references/       # optional: docs loaded only when needed
│       └── assets/           # optional: templates, examples
├── manifest.json             # machine-readable index of every skill
├── CREDITS.txt               # every source repo + license + copyright notice
├── _licenses/                # original LICENSE files from each source
├── LICENSE
└── README.md
```

## What is a skill?

A skill is a folder with a `SKILL.md` file: YAML frontmatter (`name`, `description`) plus plain-Markdown instructions, optionally bundled with scripts and references. It works with **Claude Code, Claude.ai, and the Claude API** — and follows the open Agent Skills standard, so other agents (Cursor, Codex, Gemini CLI, etc.) can use it too.

**Progressive disclosure:** Claude only reads each skill's name and description until a task matches it, then loads the body — so a large library stays fast.

## Safety

A skill can run scripts in your environment. Read a skill's `SKILL.md` (and any `scripts/`) before installing, and only use skills you trust.

## Contributing

1. Fork the repo.
2. Add or improve a skill under `skills/<folder>/` with a valid `SKILL.md`.
3. Keep the original license/notice for any content you reuse.
4. Open a pull request.

PRs that add genuinely new, licensed skills are welcome.

## License

Each skill retains its **original license** (MIT / Apache-2.0). See **`CREDITS.txt`** for every source repo and copyright notice, and **`_licenses/`** for the original license files. Redistribution is permitted under those licenses **provided the notices are kept** — do not remove them.

## Credits

- **Curated and maintained by [geowallah.com](https://geowallah.com)**
- Built on the open-source work of every repo listed in [`CREDITS.txt`](CREDITS.txt).

## Star history

[![Star History Chart](https://api.star-history.com/svg?repos=harryroger798/claude-skills-library&type=Date)](https://star-history.com/#harryroger798/claude-skills-library&Date)

---

<div align="center">

**If this saved you a $39 bundle, drop a star.**

Made with care by [geowallah.com](https://geowallah.com)

</div>
