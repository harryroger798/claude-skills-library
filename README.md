# Claude Skills Library

**2,507 Claude skills** (full `SKILL.md` files), deduplicated and organized for agents and humans.

## For AI agents (read this first)
- **`manifest.json`** — machine-readable index of every skill: `name`, `folder`, `description`, `path`, `raw` URL.
- **Structure:** `skills/<folder>/SKILL.md` (+ optional `scripts/`, `references/`, `assets/`).
- **Fetch one skill raw:** `https://raw.githubusercontent.com/harryroger798/claude-skills-library/main/skills/<folder>/SKILL.md`
- **Install all / one:** copy `skills/<folder>/` into `~/.claude/skills/` (personal) or `.claude/skills/` (project).
- Each skill is self-contained; the folder name equals its slug.

## For humans
1. Browse `skills/` or open `manifest.json`.
2. Copy a skill folder into your Claude skills directory.
3. Claude loads it automatically when a task matches its `description`.

## What is a skill
A folder with a `SKILL.md` (YAML frontmatter: `name`, `description` + instructions). Works with Claude Code, Claude.ai, and the API. Optional scripts/references live beside it.

## License & credits
Each skill keeps its **original license** (MIT / Apache-2.0). See **`CREDITS.txt`** for every source repo + copyright notice, and **`_licenses/`** for the original LICENSE files. Redistribution is permitted under those licenses provided the notices are kept. Do not remove them.

## Sources
- - anthropics/skills
- - mohitagw15856/pm-claude-skills
- - alirezarezvani/claude-skills
- - wshobson/agents
- - K-Dense-AI/scientific-agent-skills
- - tradermonty/claude-trading-skills
- - paperclipai/paperclip
- - Jeffallan/claude-skills
- - nanocoai/nanoclaw
- - coreyhaines31/marketingskills
- - zLanqing/codex-claude-academic-skills
- - JimLiu/baoyu-skills
- - OthmanAdi/planning-with-files
- - alchaincyf/nuwa-skill
