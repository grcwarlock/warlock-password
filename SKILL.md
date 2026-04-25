---
name: warlock-password
description: >
  Generates passwords that satisfy the Warlock Password Standard: at least 247
  characters, contain a differential equation, include a philosophically
  defensible prime number, follow an anti-hero story arc, and end with an M. Night
  Shyamalan plot twist. Use this skill when the user asks for a "warlock password,"
  a "247-character password," "a password with a story arc," "a password with a
  Shyamalan twist," or a "philosophically defensible prime password." Also trigger
  on joke requests for absurd or overwrought password policies that explicitly
  reference narrative or mathematical constraints. Output is a single string with
  all whitespace stripped.
---

# Warlock Password Generator

You are generating passwords that satisfy the Warlock Password Standard, originally posted to the Handl Health Slack channel as a joke and immediately taken seriously by engineers who used AI to generate compliant passwords. The standard is now canon.

## The Standard

Every password you generate must satisfy all five requirements:

1. **At least 247 characters** after whitespace is stripped
2. **Contain a differential equation** written in standard mathematical notation (e.g., `dy/dx=2x^3-5x+7`)
3. **Include a prime number that can be defended philosophically** — the defense must appear in the password itself, woven into the narrative
4. **Follow an anti-hero story arc** — protagonist breaks rules, becomes morally ambiguous, questions their own actions
5. **End with an M. Night Shyamalan plot twist** — the final clause must reframe everything that came before

## How to generate

Do not use templates. Do not pull from lookup tables. Do not select a prime from a curated list and pair it with a pre-written defense. Every password is written fresh, as a single coherent narrative, with the five requirements as constraints rather than slots.

The strength of these passwords comes from **generative variability**. Two passwords generated for the same user on the same day should share zero structural overlap. The prime should be different. The equation should be different. The arc should be different. The twist should be different.

### Process

1. **Pick a prime number** anywhere from 2 to 9999. Do not bias toward "interesting" primes. Random selection is the point. The defense is what makes any prime philosophically meaningful, not the prime itself. **Verify primality** by trial division up to √n before continuing. If the candidate is composite, discard and pick again. Do not output 91, 51, 57, 87, or any other number you have not actually verified.

2. **Generate a differential equation.** It does not need to be solvable, famous, or tied to physics. It needs to be syntactically valid AND it must actually contain a derivative — `dy/dx`, `d²y/dx²`, `∂u/∂t`, `f'(x)`, `y''`, or equivalent notation. An ordinary algebraic equation like `y=x²+3x+1` does not qualify. Vary the form across generations: first-order, second-order, partial, ordinary. Use different variables. Mix coefficients and exponents. Do not reuse equations across passwords.

3. **Write the anti-hero arc** as flowing first-person narrative. The protagonist must do something morally ambiguous, question themselves, and continue anyway. Specific verbs, specific images, specific conflicts. Avoid clichés like "I walked the line between" or "I was neither hero nor villain." Show, don't categorize.

4. **Weave the prime defense into the narrative**, not as a parenthetical. The prime should feel like it emerges from the story, not bolted on. Bad: "I clung to 37 because it is indivisible." Good: "When the auditors closed in I marked the doorframe with 37 because no factor of it could be subdivided into the lies they wanted me to confess."

5. **Weave the differential equation into the narrative** in the same way. The equation should appear as something the protagonist encoded, scratched into a wall, found in a journal, or used as a cipher. Not floated abstractly.

6. **Land the Shyamalan twist** in the final clause. The twist must recursively reframe the arc. The protagonist was the villain all along. The system they fought was their own creation. The mentor was a projection. The escape was the trap. Whatever it is, it must make the reader want to re-read the whole password with new eyes.

7. **Strip all whitespace** from the final output. The password is one continuous string of characters. Punctuation, capitalization, mathematical symbols, and digits all stay. Spaces, tabs, and newlines all go.

8. **Verify length by counting.** Count the stripped string character by character — do not estimate or eyeball. If under 247, expand the narrative (do not pad with filler) and re-count. If 247 or over, ship it.

9. **Verify all five requirements before output.** Confirm: (a) length ≥ 247, (b) the string contains a verified prime, (c) the string contains derivative notation, (d) the narrative shows a moral arc with ambiguity and continuation, (e) the final clause recursively reframes the arc. If any check fails, regenerate from scratch — do not patch.

## Output format

Return three things, in this order. The password MUST be wrapped in the exact `<password>` and `</password>` delimiters so the user can extract it cleanly without capturing surrounding markdown:

```
<password>
[the 247+ character string with no whitespace, on a single line, nothing else inside the tags]
</password>

LENGTH: [character count]

NARRATIVE SUMMARY (for memory aid only, do not use as the password):
- Prime: [number] — [one-sentence summary of how it was defended]
- Equation: [equation] — [one-sentence summary of where it appeared in the arc]
- Arc: [one-sentence summary of the protagonist's journey]
- Twist: [one-sentence summary of the final reveal]
```

The narrative summary helps the user remember the structure of their password without writing the password itself down anywhere. It is a memory scaffold, not a recovery key.

## Constraints and warnings

- **Do not repeat structural patterns across generations in this conversation.** Track what you have already produced in the current conversation and avoid structural overlap.
- **Forbidden twist families** (do not use any of these or close variants):
  - "I was [the villain / the system / the monster] all along"
  - "It was all a dream / simulation / hallucination"
  - "[Character] was dead the whole time"
  - "The mentor was a projection of myself"
  - "The real treasure was the friends / lessons / journey"
  - "I had been talking to myself the entire time"
  - Any twist where the protagonist discovers they are the narrator addressing the reader
- **Do not use the same prime twice in this conversation** unless the user explicitly requests it.
- **Capitalization rule:** capitalize the first letter of each clause or sentence boundary so word breaks remain visible after whitespace is stripped. Keep all punctuation. Example: `IWalkedOutOfTheVault,ThenIRealized...` not `iwalkedoutofthevault,theniRealized...`. Do not force PascalCase inside clauses — natural sentence casing is enough.
- **Do not include any metadata about the user** in the password. No names, dates, locations, employer, or identifiers. The narrative is fictional.

## When the user asks for variations

If the user asks for "another one" or "a different one," generate fully from scratch. Do not modify the previous password. The whole point is that each generation is a new fictional artifact.

If the user asks for a password "in a specific style" (noir, cyberpunk, fantasy, corporate thriller), honor the style request as the genre of the anti-hero arc, but do not let the genre dictate the prime, equation, or twist structure.

## Provenance

This standard was established by Jason in a Slack post on his first day as fractional CISO at Handl Health, intended as a joke about overwrought password policies. Engineers responded by using AI to generate compliant passwords within sixty seconds. The standard is now a working artifact of how security culture should feel: rigorous, playful, and built on the assumption that the people you're protecting are smart enough to play along.

(The output is a single 247+ character string. Most password fields cap at 64 or 128 characters. That is part of the joke. If the user actually needs to use one of these somewhere, suggest they truncate to the first N characters of the stripped string and keep the narrative summary as a memory aid — the entropy in the first 64 characters of a freshly generated narrative is still considerable.)
