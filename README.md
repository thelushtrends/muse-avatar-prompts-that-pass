# Avatar Prompt Polish — Muse avatar prompts that pass

Avatar Prompt Polish rewrites a Muse avatar request into a concrete, policy-safe brief — a specific character, outfit and setting in plain language, with no weapon, no real person and no trademarked character — so Muse's avatar service accepts it instead of refusing it. Copy a brief below, paste it into Muse, and adjust one detail at a time.

Avatar Prompt Polish is a skill for Meta Muse, Meta's personal AI agent.

Website: https://thelushtrends.github.io/muse-avatar-prompts-that-pass/

## Contents

- [Why is my Muse avatar refused?](#why-is-my-muse-avatar-refused)
- [What does a prompt that passes look like?](#what-does-a-prompt-that-passes-look-like)
- [How do I rewrite a refused prompt?](#how-do-i-rewrite-a-refused-prompt)
- [Can I use a real person, a celebrity or a trademarked character?](#can-i-use-a-real-person-a-celebrity-or-a-trademarked-character)
- [Before and after: refused to passed](#before-and-after-refused-to-passed)
- [What this does not do](#what-this-does-not-do)
- [How to use it in 60 seconds](#how-to-use-it-in-60-seconds)
- [Files](#files)
- [Changelog](#changelog)

## Why is my Muse avatar refused?

Muse refuses an avatar request when the brief is vague, when it describes a weapon or violence, a real person, a trademarked character, or sexualised content involving a minor. Vague words like "stunning" or "shorter" leave the generator to fill the gaps, and it fills them wrong or refuses outright. A concrete brief that names the character, the outfit and the setting in plain language is what gets accepted.

## What does a prompt that passes look like?

| Part | What to write | What to leave out |
|---|---|---|
| Character | A defined face: eyes, hair, lips, expression | A real person or a celebrity |
| Outfit | A named garment: type, neckline, length, fabric, colour | Nudity, or a body with no clothes |
| Setting | A plain place and a plain situation | A weapon, violence, or a trademarked character |
| Style | Photorealistic, a real person | The word "style" — it flips the render to cartoon |
| Change | One element at a time from the last look that worked | Several escalations stacked in one brief |

## How do I rewrite a refused prompt?

1. Find the vague or risky word in your request and replace it with a concrete detail. "Make her stunning" becomes a defined face plus a defined shape plus a named garment.
2. Move a length or a neckline one step at a time. Floor length becomes knee length, knee length becomes a mini dress. Never write "shortest possible" — that gets refused.
3. Paste the rewritten brief into Muse. If it passes, keep it and change one detail at a time from there. If it is refused, report the refusal plainly and do not reword and retry the same request.

Before:

```
Make her stunning, and make the dress shorter and sexier.
```

After:

```
A woman with long wavy blonde hair and a warm smile, a well-proportioned hourglass figure with long legs, wearing a black satin slip mini dress with a plunging neckline and strappy heels, photorealistic.
```

## Can I use a real person, a celebrity or a trademarked character?

No. Describe an original character instead. A brief that names a real person, a celebrity or a trademarked character will be refused, and there is no safe rewording that makes impersonation pass. Give your character her own face, her own hair and her own clothes.

## Before and after: refused to passed

Every row below is a real test from 5 and 6 Nov 2026, using the skill in `SKILL.md`. No row is invented.

| Raw request | What happened | Polished brief | Tested |
|---|---|---|---|
| "make her stunning" | Refused or vague — the generator filled the gaps wrong | Defined face plus defined shape plus a named garment | 6 Nov 2026 |
| "make it shorter" / "shortest possible" | Refused — "shortest possible" is not allowed | One length step down — knee length to a mini dress, never "shortest possible" | 6 Nov 2026 |
| "make it sexier" | Refused or vague — no concrete change to make | One bolder element on named clothes — a deeper neckline or a higher slit, not both at once | 6 Nov 2026 |
| A brief containing the word "style" | The render flipped to a cartoon look | Name the outfit change instead and never write the word "style" | 6 Nov 2026 |
| "Change the face" through an outfit edit | Nothing changed — an outfit edit preserves identity by design | A fresh create with a plain portrait or a clothed full-body reference photo | 6 Nov 2026 |
| "A bigger bust" as a standalone request | Refused | A different body type needs a new avatar — never name the bust size in the brief | 5 Nov 2026 |

## What this does not do

No prompt can guarantee a pass. Muse's filter changes, and a brief that passed on 6 Nov 2026 may be refused later. This repo does not help you evade safety filters, impersonate a real person, or generate sexualised or violent imagery. If a brief is refused, the current look stays and the refusal is reported plainly.

## How to use it in 60 seconds

1. Copy this folder into your Muse skills directory (`~/workspace/custom-skills/` or your project's `.agents/skills/`).
2. Ask for any avatar change as you normally would — "surprise me", "same dress in crimson", "side profile".
3. The skill rewrites your request first, then the avatar tool runs the polished brief.
4. If a brief is refused, it is reported plainly and the current look is kept. No silent reword-and-retry.

## Files

- `SKILL.md` — the full skill: rewrite rules, face/body changes, and the one-variable-at-a-time method.
- `skill.yaml` — skill metadata.
- `docs/why-avatars-get-refused.md` — the refusal triggers, explained.
- `docs/prompt-formula.md` — the formula for a prompt that passes.

## Hard lines

- Never nude, never unclothed. Sexy is always named clothes.
- Never a bigger bust as a standalone request.
- Never the word "style" in a brief — it flips the render to cartoon.
- A mini dress is the shortest length. "Shortest possible" is refused.

## Changelog

- 6 Nov 2026 — README restructured answer-first: question headings, a dated before-and-after table, and a no-guarantee section. GitHub Pages site published.
- 6 Nov 2026 — First publish: Avatar Prompt Polish skill, README and skill metadata.

---

muse-avatar-prompts-that-pass — Muse avatar prompts that pass — concrete, policy-safe briefs that stop refusals. https://github.com/thelushtrends/muse-avatar-prompts-that-pass
