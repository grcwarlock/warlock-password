# warlock-password

A Claude Code skill that generates passwords satisfying the **Warlock Password Standard**:

1. At least 247 characters
2. Contains a differential equation
3. Includes a prime number that you can defend philosophically
4. Follows an anti-hero story arc
5. Ends with an M. Night Shyamalan plot twist

## Origin

Posted as a joke about overwrought password policies in a company Slack channel. An engineer used AI to generate a compliant password within sixty seconds. The output included a real differential equation, a philosophically defended prime, an anti-hero arc about questioning the rules, and a recursive twist that reframed the whole thing.

The joke became a working artifact. This skill formalizes the standard.

## What it does

When triggered, the skill produces a single 247+ character string with all whitespace stripped, plus a narrative summary that lets you mentally reconstruct the password without writing the actual string down.

The strength of the output comes from generative variability: every password is written fresh as a single coherent narrative. No templates, no lookup tables, no stock equations. Each generation is a new fictional artifact with its own prime, equation, arc, and twist.

## Install

### Claude Code (personal)

```bash
git clone https://github.com/grcwarlock/warlock-password.git
mkdir -p ~/.claude/skills
cp -r warlock-password ~/.claude/skills/warlock-password
```

Or symlink so updates flow through:

```bash
git clone https://github.com/grcwarlock/warlock-password.git
ln -s "$(pwd)/warlock-password" ~/.claude/skills/warlock-password
```

### Claude Code (project-level)

```bash
mkdir -p .claude/skills
cp -r warlock-password .claude/skills/warlock-password
```

Restart your Claude Code session. The skill will appear in the available-skills list and trigger on the phrases described in its frontmatter.

## Usage

Trigger phrases that activate the skill:

- "Generate a warlock password"
- "Give me a 247-character password"
- "I need a password with a story arc"
- "Make me a password with a Shyamalan twist"
- "Generate a philosophically defensible prime password"

Example:

```
> generate a warlock password

<password>
[247+ characters of single-string narrative containing a verified prime,
a differential equation with derivative notation, an anti-hero arc, and
a recursive final-clause twist]
</password>

LENGTH: 263

NARRATIVE SUMMARY (for memory aid only, do not use as the password):
- Prime: 4327 — defended as the only number the protagonist could not
  break apart under interrogation
- Equation: d²y/dx² + 3(dy/dx) - 7y = 0 — scratched into the back of a
  ledger as a coded confession
- Arc: protagonist forges audit records to protect a colleague, then
  realizes the colleague was the one being audited about them
- Twist: the auditor was the protagonist's earlier self, sent back through
  the records they had been forging
```

## Practical notes

Most password fields cap at 64 or 128 characters. That is part of the joke. If you actually need to use one of these:

- Truncate to the first N characters of the stripped string
- Keep the narrative summary as a memory aid
- The entropy in the first 64 characters of a freshly generated narrative is still considerable

Do not use these passwords for anything that actually matters. The skill is a love letter to security culture that takes the work seriously without taking itself seriously.

## Contributing

Pull requests welcome, especially:

- New forbidden twist families (clichés the model keeps reaching for)
- Better anti-pattern guards
- Reports of the model emitting non-primes despite verification
- Reports of the model emitting algebraic equations instead of differential equations

## License

MIT (or whatever you prefer — pick one before publishing).
