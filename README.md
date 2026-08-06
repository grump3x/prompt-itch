# prompt-itch

A Claude Code plugin marketplace for writing discipline: cut the AI tells, cut the words.

## Install

```
/plugin marketplace add grump3x/prompt-itch
/plugin install stop-slop@prompt-itch
/plugin install laconic@prompt-itch
```

## Plugins

| Plugin | What it does | Upstream | License |
|--------|--------------|----------|---------|
| `stop-slop` | Removes AI writing patterns from prose: banned phrases, structural cliches, scoring rubric. | [hardikpandya/stop-slop](https://github.com/hardikpandya/stop-slop) | MIT, Hardik Pandya |
| `laconic` | Brief prose. Short common words. Trust context. Omit what the reader can infer. | [GabrielBarberini/laconic](https://github.com/GabrielBarberini/laconic) | MIT, Gabriel Barberini |

Both plugins are vendored copies of upstream work, redistributed under their original
MIT licenses, which ship alongside each plugin. From `laconic` only the Claude Code
parts are included; its Codex variants, VS Code extension, and benchmarks are left upstream.

## Layout

```
.claude-plugin/marketplace.json
plugins/
  stop-slop/
    .claude-plugin/plugin.json
    skills/stop-slop/SKILL.md
    skills/stop-slop/references/{phrases,structures,examples}.md
    LICENSE README.md CHANGELOG.md
  laconic/
    .claude-plugin/plugin.json
    skills/laconic/SKILL.md
    LICENSE README.md
```
