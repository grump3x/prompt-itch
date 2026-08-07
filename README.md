# prompt-itch

A Claude Code plugin marketplace for writing discipline: cut the AI tells, cut the words.

## Install

```
/plugin marketplace add grump3x/prompt-itch
/plugin install laconic@prompt-itch
```

Then pick an output style in `/config` → **Output style**: `laconic` or
`laconic-ru`. The choice takes effect after `/clear` or in a new session.

## Plugins

| Plugin | Ships | Upstream | License |
|--------|-------|----------|---------|
| `laconic` | Output styles `laconic` and `laconic-ru` | [GabrielBarberini/laconic](https://github.com/GabrielBarberini/laconic) | MIT, Gabriel Barberini |

Built on upstream MIT work, redistributed under the original license, which
ships alongside the files it covers.

## Layout

```
.claude-plugin/marketplace.json
plugins/laconic/
  .claude-plugin/plugin.json
  output-styles/laconic.md          # brevity rules
  output-styles/laconic-ru.md       # brevity rules + language policy
  LICENSE README.md
```
