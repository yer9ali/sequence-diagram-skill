# sequence-diagram

A [Claude Code](https://claude.com/claude-code) skill for building sequence
diagrams of microservice interactions and API call flows, from source code,
a described scenario, or both. Outputs Mermaid or PlantUML.

## Install

In Claude Code:

```
/plugin marketplace add yer9ali/sequence-diagram-skill
/plugin install sequence-diagram@sequence-diagram-skill
```

Or manually: copy [`skills/sequence-diagram/SKILL.md`](skills/sequence-diagram/SKILL.md)
into your skills directory (`~/.claude/skills/sequence-diagram/` on Claude Code;
`~/.agents/skills/sequence-diagram/` also works on Codex, Copilot CLI, and
Gemini CLI).

## Usage

Just ask: "build a sequence diagram for OrderService's checkout flow" — the
skill picks the right participants (process boundaries, not function calls),
traces sync/async calls, and renders Mermaid or PlantUML.

See [SKILL.md](skills/sequence-diagram/SKILL.md) for the full process and quick reference.

## License

[MIT](LICENSE)
