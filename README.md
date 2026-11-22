# Tout

Configuration Claude Code partagée pour ce dépôt.

## Outils installés

- **last30days** (plugin Claude Code) : déclaré dans `.claude/settings.json` via la marketplace `mvanhorn/last30days-skill`. Il s'active à l'ouverture du projet.
- **MarkItDown** (serveur MCP) : déclaré dans `.mcp.json`, lancé par `uvx markitdown-mcp`. Convertit PDF, DOCX, PPTX, XLSX, images, etc. en Markdown.
- **Agent Reach** (skill + CLI) : le skill est dans `.claude/skills/agent-reach/`. Le programme `agent-reach` doit être présent sur la machine :
  ```bash
  uv tool install https://github.com/Panniantong/Agent-Reach/releases/latest/download/agent-reach.zip
  agent-reach setup
  ```
  Ne pas l'installer depuis PyPI (le paquet `agent-reach` de PyPI est un autre projet).

## Non installé

- **Prompt Motion** (prompt-motion.com) : c'est une bibliothèque en ligne de prompts et de skills de motion design, pas un plugin. On copie au cas par cas le skill voulu depuis le site.
