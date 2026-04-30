# Contributing

Contributions follow the same process as any open source project, applied to the domain of home appliances.

## Adding a new model

1. Create a directory: `models/<manufacturer-modelnum>/` (lowercase, hyphenated)
2. Add a `SKILL.md` following the template and conventions below
3. Add the model to the table in `README.md`
4. Open a pull request

## SKILL.md requirements

### Frontmatter

```yaml
---
name: <manufacturer-modelnum lowercase hyphenated>
description: >
  Operate a <full model name>. Invoke this skill when the user needs to
  perform cooking, reheating, defrosting, or other functions on this
  specific model. Do not generalise to other <manufacturer> models.
manufacturer: <name>
model: <model number>
type: <countertop | built-in | over-the-range>
wattage: <output wattage>W
capacity: <litres>L
interface: <brief description, e.g. "rotary dial + single confirm button">
source: <URL to official manual PDF or manual page>
---
```

### Body

One orientation paragraph describing the interface — how the controls work conceptually, what state the machine starts in, any model-specific quirks worth knowing upfront.

Then one `##` section per major function. Use the following structure within each section:

```markdown
### <Operation name>

**Invoke:** <what button/sequence to press to enter this mode>
**Parameters:** <what the user sets — time, weight, power level, temperature>
**Execute:** <what starts the operation>
**Returns:** <what happens when done — beeps, display state, etc.>
**Edge cases:** <anything that will catch the user out>
```

Include only sections the model actually supports. Suggested sections: Quick Start, Reheating, Defrost, Power Levels, Grill, Convection, Combination Cooking, Multi-Stage Cooking, Auto Menus, Child Lock, Clock, Error States.

### Source requirements

Instructions must come from the official manual — not inferred from LLM knowledge of the model or generalised from similar units. Cite the manual source URL in the frontmatter.

**PRs based on theoretical knowledge of a model the contributor has not physically operated will be rejected in review.**

If a step cannot be verified against the actual unit or official documentation, omit it rather than approximate.

### Verification

Test each documented operation against the actual unit where possible. Sensor cook edge cases and multi-stage sequences are the sections most likely to contain errors.

### Style

No jokes inside SKILL files. The README is where the framing lives; the SKILL files are operational documentation. Maintain the deadpan. Use the vocabulary consistently:

- Button presses → "invoke" or "press"
- Entering a mode → "invoke [MODE]"
- Turning the dial → "turn dial to select"
- Starting → "execute" or "press START"
- The machine finishing → "returns" or "operation completes"
- Unexpected beeping → "error state"
- Mid-cook intervention → "interrupt"
