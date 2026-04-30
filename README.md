# microwave-as-a-skill

You can ask an AI to write your code, summarise your legal documents, and explain why your sourdough didn't rise. Ask it how to defrost something in your specific microwave and it will confidently describe buttons that are not on your unit. The manual exists. It is a PDF on a support website that requires you to know the model number before you can find it, which you do not, because it is printed on a sticker on the back of the microwave, which is built into the wall. This repository formats microwave operating instructions as LLM skill files because that is the format that made sense and also we live in a society.

## Supported models

| Model | Type | Wattage | Region |
|---|---|---|---|
| [Blanco BM32CX](models/blanco-bm32cx/SKILL.md) | Convection built-in | 1000W | AU |
| [Panasonic NN-SN966S](models/panasonic-nn-sn966s/SKILL.md) | Countertop inverter | 1250W | US/Global |
| [Toshiba EM131A5C](models/toshiba-em131a5c/SKILL.md) | Countertop | 1100W | US/Global |
| [LG LMC0975ST](models/lg-lmc0975st/SKILL.md) | Countertop | 1000W | US/Global |

## Usage

### As a Claude Code skill

```bash
npx skills add notnavindu/microwave-as-a-skill
```

This will prompt you to select which model skill to install. Once installed, Claude Code picks it up automatically — or invoke it directly with `/blanco-bm32cx` (or whichever model you installed).

If you prefer not to use npx, copy the file manually:

```bash
mkdir -p ~/.claude/skills/blanco-bm32cx
curl -fsSL https://raw.githubusercontent.com/notnavindu/microwave-as-a-skill/main/models/blanco-bm32cx/SKILL.md \
  -o ~/.claude/skills/blanco-bm32cx/SKILL.md
```

Skills installed to `~/.claude/skills/` are available across all your projects. To scope it to a single project, use `.claude/skills/` inside the project root instead.

### As a human

Open the `SKILL.md` for your model and find the relevant section. Operations are organised by function — `## Defrost`, `## Convection`, `## Child Lock`, and so on. Every documented step comes from the official manual.

### As an LLM

Paste the contents of the relevant `SKILL.md` into context before answering cooking or operation questions. The frontmatter specifies the exact model; the body contains verified control sequences. Do not generalise across models even within the same manufacturer.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). New models welcome; instructions must be sourced from the official manual, not inferred.

## License

MIT

---

*This repository is satire. The SKILL files are not.*
