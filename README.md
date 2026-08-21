# input-from-stakeholders

Collects and synthesizes attributed stakeholder input without manufacturing consensus.

It produces:

- **Stakeholder Input Brief and Synthesis:** a working artifact built from supplied facts, labeled inference, and visible missing fields.

It executes the [Input From Stakeholders playbook](https://www.andrewluxem.com/playbooks/input-from-stakeholders). The playbook teaches the framework. This skill runs it and returns a working artifact.

**Static by construction: no dependencies, executable code, telemetry, network calls, remote instructions, auto-update, scheduled work, or background behavior.** It reads only the files in its own skill folder. Nothing happens until a user or agent invokes it.

## Install

Clone and copy the skill into Claude Code:

```bash
git clone https://github.com/andrewluxem/input-from-stakeholders.git
cp -r input-from-stakeholders/skills/input-from-stakeholders ~/.claude/skills/
```

For Codex, copy the same complete folder to the Codex skills directory:

```bash
cp -r input-from-stakeholders/skills/input-from-stakeholders ~/.codex/skills/
```

Or install it as a Claude Code plugin:

```text
/plugin marketplace add andrewluxem/input-from-stakeholders
/plugin install input-from-stakeholders@input-from-stakeholders
```

For clients that install from an archive, use the versioned [input-from-stakeholders v1.0.0 ZIP](https://www.andrewluxem.com/downloads/input-from-stakeholders-v1.0.0.zip).

## Invoke it

```text
Synthesize this stakeholder input into a decision brief
Use the input-from-stakeholders skill.
```

Naming the skill is always valid: `use the input-from-stakeholders skill`.

## Files

```text
.claude-plugin/
  plugin.json
  marketplace.json
skills/input-from-stakeholders/
  assets/stakeholder-input-brief-template.md
  LICENSE.md
  meta.yaml
  references/synthesis-standard.md
  SKILL.md
README.md
LICENSE
```

The complete canonical package is copied under `skills/input-from-stakeholders/`, including every asset, reference, test prompt, source note, changelog entry, and license file present in the source.

## Versioning

Plugin installation is version-pinned. When behavior changes, update the version consistently in `SKILL.md`, `meta.yaml`, `.claude-plugin/plugin.json`, and `.claude-plugin/marketplace.json`, then add a changelog entry. Reinstalling is an explicit update; this repository never auto-updates itself.

## License

MIT. See [LICENSE](LICENSE). The canonical skill folder carries the same authorization in [skills/input-from-stakeholders/LICENSE.md](skills/input-from-stakeholders/LICENSE.md).

---

## More playbooks

This skill packages one playbook from the free library at [github.com/andrewluxem/playbooks](https://github.com/andrewluxem/playbooks). Every playbook is free to read, with no email required.