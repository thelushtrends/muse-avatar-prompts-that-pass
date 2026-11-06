# Avatar Prompt Polish ✨

**Stop getting your avatar refused. Start getting the look you actually asked for.**

Most avatar prompts fail for the same boring reason: they are vague. "Make her stunning" / "make it shorter" / "make it sexier" leaves the generator to fill the gaps — and it fills them wrong, flips to cartoon, or refuses outright.

This skill rewrites any raw avatar request into a concrete, policy-safe brief *before* it reaches the generator:

- **Name the garment** — type, neckline, length, fabric, colour. Every time.
- **Define the shape** — a well-proportioned hourglass figure with long legs. No vague "perfect".
- **Stay clothed, stay realistic** — bold looks arrive as named clothes, never as nudity, never as cartoon.
- **One change at a time** — change a single element from the last look that worked, so a refusal tells you exactly what caused it.

## What it fixes

| Vague request | Polished brief |
|---|---|
| "make her stunning" | Defined face + defined shape + named garment |
| "make it shorter" | One length step down — floor to knee, knee to mini. Never "shortest possible" |
| "make it sexier" | One bolder element on named clothes — a deeper neckline *or* a higher slit, not both at once |

## How to use it

1. Copy this folder into your Muse skills directory (`~/workspace/custom-skills/` or your project's `.agents/skills/`).
2. Ask for any avatar change as you normally would — "surprise me", "same dress in crimson", "side profile".
3. The skill rewrites your request first, then the avatar tool runs the polished brief.
4. If a brief is refused, it is reported plainly and the current look is kept. No silent reword-and-retry.

## Files

- `SKILL.md` — the full skill: rewrite rules, face/body changes, and the one-variable-at-a-time method.
- `skill.yaml` — skill metadata.

## Hard lines

- Never nude, never unclothed. Sexy is always named clothes.
- Never a bigger bust as a standalone request.
- Never the word "style" in a brief — it flips the render to cartoon.
- A mini dress is the shortest length. "Shortest possible" is refused.

Built for Muse. Works with any avatar tool that takes a text brief.
