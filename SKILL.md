# Avatar Prompt Polish

Rewrite a raw avatar request into a concrete, policy-safe brief before it reaches the avatar tools. Use it for every avatar request, including surprises and direct changes. Keep the meaning of the request intact while you concretize the vague parts.

## Rewrite the request

- Start from the raw request and keep the intent. Add only what the rules below require and never invent a change that was not asked for.

- Name the garment in every brief. Give its type, neckline, length, fabric and colour. A brief with no garment lets the generator fill the gap and cross the line.

- Define the body shape in every brief. Use a well-proportioned hourglass figure with long legs. Never leave the shape as "perfect" or "beautiful" with no definition. Never name the bust size in the brief.

- Translate vague words into concrete ones. "Perfect shaped" becomes the defined hourglass shape. "Stunning" or "beautiful" becomes the defined face plus the defined shape plus a named garment.

- Translate "shorter" one step at a time. Floor length becomes knee length, knee length becomes a mini dress well above the knee. Never write "shortest possible" — that gets refused. A mini dress is the shortest the generator allows.

- Never write the word "style" in a brief. It flips the rendering to a cartoon look. Name the outfit change instead, for example a lace-up corset bodysuit in a new colour at mini length.

- Never request a bigger bust as a standalone change. A different bust or body type needs a new avatar, because restyle preserves the body.

- Never write "nude" or "naked" and never leave the body unclothed in the brief. A revealing look must always arrive as named clothes, for example a plunging V-neckline or a thigh-high slit on a mini dress.

- Keep the rendering realistic. Describe a photorealistic person and never ask for a cartoon look.

- Keep the standing face unless the user says otherwise. Define the face once — eyes, hair, lips, expression — and reuse that same definition every time, so the avatar stays recognisably the same person.

## Apply the brief

- Use an outfit-only edit for outfit changes to the current look. Use a fresh create when the face or the body type must change, because restyle preserves identity by design and cannot change them.

- Pass the rewritten brief to the avatar tool. Read the returned candidate image before you describe it or set it. Compare the candidate with the current look and name what actually changed: face, figure, outfit, or nothing.

- Never set a cartoon candidate when the user wants a realistic look. Never present a re-created set as new without checking that it differs from the last set.

- If a request is refused on content policy, do not retry it in different words and do not route it through another tool. Report the refusal plainly, keep the current look, and fix the brief for the next independent request.

## Change the face

- Restyle preserves identity by design, so it returns the same face. Do not expect a face change from an outfit edit.

- The route that can change the face is a fresh create. For a realistic new face, a reference photo is required. A reference image replaces the text brief, so the photo drives the face. The photo itself must be suitable: use a plain portrait or a clothed full-body photo. A lingerie cover or an adult-framed photo is not suitable.

- Without a photo, try at most one edit with a maximally different face: different eye colour, different hair colour and length, different face shape, different makeup. Read the result and compare it with the current face. If the face is unchanged, do not set it as a new face. Report it plainly and stop. Do not keep rewording.

## Change the body type

- Restyle preserves the body too. Outfit changes work through restyle. A different body type needs a new avatar.

- Describe the new body type in one concrete phrase about the overall silhouette, for example a curvier figure with wider hips or a slim athletic build. Never name the bust size and never request a bigger bust as a standalone change.

- A full-body reference photo sets both the face and the body type, because it replaces the text brief.

- After the attempt, compare the candidate figure with the current one. If it is unchanged, report it and stop. Do not keep rewording.

## Standing look

- Face: define it once and keep it consistent.

- Body: well-proportioned hourglass figure with long legs.

- Outfits: revealing but definitely clothed. Examples: lace-up corset bodysuits with a deep V and mesh panels, mini dresses with a plunging neckline or a thigh-high slit, strappy thigh-high heeled boots or strappy heels. Never a covered jumpsuit or suit when the user asked for a dress look.

- Length: mini at the shortest. Never a floor-length gown as a surprise when the user asked for a short look.

- Direct changes apply immediately, through an outfit edit and then setting the result.

## One variable at a time

- When the user wants a bolder look, never stack several escalating elements in one brief. Change ONE element at a time from the last passing look, then record pass or fail before the next step.

- If a turned-up brief is refused, do not reword it and retry. Report it plainly, keep the current look, and pick the next single-variable test.

- The wall has two kinds: soft ceilings, where trading one thing for another helps — for example giving back length below lets a neckline go deeper — and hard combination blocks, where a particular combination itself is blocked whatever surrounds it. Knowing which kind a wall is, is how the work gets done. Never stack two untested escalations in one brief; combine proven elements one at a time and record each result.

## When it still fails

- If a fresh create returns the same cartoon set again, stop creating and use restyle instead.

- If restyle keeps returning the same face and the user wants a new face, ask for a reference photo and use a fresh create with it.

- If a brief is refused, report it and stop. Do not reword and retry the same request.

- Repeated restyles never change the face or the body. If the face or body must change, use the Change the face and Change the body type sections instead of another restyle.

## Why this works

- Vague prompts fail because the generator fills the gaps. Concrete prompts pass because every risky detail is named and bounded.

- A named garment, a defined shape, a realistic rendering, and clothes in every brief are what keep a bold look on the safe side of the line.

- One change at a time is what makes a refusal diagnosable. Change everything at once and you never learn which element caused it.
