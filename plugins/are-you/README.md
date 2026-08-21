# are-you

Brief prose, no AI tells — and four corrections the user types at a turn that went wrong: the wrong
thing built, filler instead of an answer, the agent's own work handed over, a claim made without
checking. One skill per failure, each naming it and carrying the repair. Self-contained: no other
plugin, no hooks, no env vars.

## Reference

### Output style

Pick `laconic` in `/config` → **Output style**. Applies after `/clear`.
For every project: `"outputStyle": "laconic"` in `~/.claude/settings.json`.

### User-invoked

| Skill | Entry point | Typed when |
|---|---|---|
| `dolbaeb` | `/are-you:dolbaeb` | the output is not worth reviewing — the wrong thing got built |
| `mudozvon` | `/are-you:mudozvon` | the answer was water, and it ended in "want me to…?" |
| `ohuel` | `/are-you:ohuel` | a step it could have run itself was handed to the user |
| `pizdabol` | `/are-you:pizdabol` | a claim about the outside world was stated unchecked |

None of them fires on its own: `disable-model-invocation` keeps all four in the human's hands, because
the judgement that a turn was bad is the human's. The repair lives in the skill; this page names the
trigger and stops.

## Install

```
/plugin marketplace add grump3x/prompt-itch
/plugin install are-you@prompt-itch
```
