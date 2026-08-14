# Laconic

Brief prose, no AI tells.

## Output styles

Two variants, pick one in `/config` under **Output style**. Both keep Claude
Code's built-in engineering instructions.

| Style | What it adds |
|-------|--------------|
| `laconic` | Brevity rules only. Language untouched. |
| `laconic-ru` | Same rules, plus: reason in English, answer the user in Russian, keep the repository English-only. |

Only one output style is active at a time. Neither sets `force-for-plugin`, so
the choice stays yours. `/config` saves it to the project's
`.claude/settings.local.json`; to apply it everywhere, put `"outputStyle": "laconic"`
in `~/.claude/settings.json` instead. The change takes effect after `/clear` or
a new session.

A style sets how every answer sounds. This plugin ships nothing else.

## Upstream and licenses

Vendored from [GabrielBarberini/laconic](https://github.com/GabrielBarberini/laconic),
redistributed under its original MIT license as [LICENSE](LICENSE), Gabriel
Barberini. The rules come from its `SKILL.md`, reworded in ASD-STE100 Simplified
Technical English; the `laconic-ru` variant appends a language section. Upstream
also ships Codex variants, a VS Code extension, and benchmarks, all left there.
