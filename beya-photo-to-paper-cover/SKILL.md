---
name: beya-photo-to-paper-cover
description: Create Beya-style photo-derived paper-cover illustrations from uploaded photos or image references, with required handwritten signature styling, one of five selectable premium styles, and selectable output mode. Use when the user asks to generate either a split original-photo plus illustration image or an illustration-only image in a quiet paper-textured style, minimalist poster, deconstructed collage, wax-pencil sketch, travel postcard print, watercolor/gouache picture-book page, natural observation page, or poetic poster, especially when the workflow should ask for a signature name, a 1-5 style choice, and split-vs-illustration-only output mode before generating.
---

# Beya Photo to Paper Cover

## Overview

Use this skill to turn a source photo into either a strict 1:1 split composition or a standalone premium Beya paper-cover illustration. The goal is not a traced copy, painted-over photo, or detailed scenic rendering, but a distilled visual memory of the photo.

The core demo structure is authoritative: the photo remains photographic when a split output is requested, and the illustrated part should look like a sparse independent-publication paper plate. It should be small, abstracted, blocky, and handmade, with large blank paper space. Do not produce a realistic watercolor copy of the whole photo.

This is a public template. Always obtain three inputs before generation: the signature name, the selected style number from 1-5, and the output mode.

## Required Inputs

Before generating an image, obtain:

1. Signature name: ask "Enter the name you want to use for the signature."
2. Style number: `1`, `2`, `3`, `4`, or `5`.
3. Output mode:
   - `1` Split image: original photo on top, generated illustration below.
   - `2` Illustration only: generate only the Beya paper-cover illustration, without the original photo half.

If any input is missing, ask only for the missing input briefly before generating. Do not ask whether the user is Beya. If the style number is missing, show the five choices:

```text
1. Quiet Geometry Poster
2. Still Object Collage
3. Wax Pencil Keepsake
4. Coastal Postmark Print
5. Pastoral Washbook
```

Use the required Beya signature format as a visual mark, not as typed text:

- Render `{SIGNATURE_NAME}` as a clear small brand signature mark, not ordinary font text.
- If the name is `beya`, render a loose lowercase cursive `beya` matching the latest signature reference: muted olive-gray ink on white paper, medium-thin brush-pen strokes with slight pressure variation, a very tall rising first stroke on the `b`, relaxed connected lowercase letters, a large descending loop on the `y`, an elegant long rightward tail after the final `a`, and a small irregular dot at the far right aligned with the tail.
- If the name is not `beya`, design a custom abstract handwritten signature for that exact name: same quiet premium brush-pen mood, low-saturation ink, connected or semi-connected strokes, elegant long tail or finishing flourish when the letters allow, and tiny handwritten `2026` nearby.
- The signature must be horizontally elongated: the rightward tail after `a` should extend at least 60-100% of the width of the written word `beya`, and the final dot must sit clearly away from the letters, not immediately after `a`.
- The signature must not look like a standard cursive font or the short text `beya.`.
- Do not draw a literal tilde character, underline symbol, bullet label, or `BY` prefix.
- Make the `beya` signature smaller than previous outputs: a subtle brand mark, about 2-4% of the illustration area width. For other names, keep the signature similarly subtle and secondary, adjusting width only enough for legibility.
- Place the signature consistently in the lower-right corner of the illustration area, with comfortable paper margin.
- Make the final dot slightly irregular and casual, like a quick imperfect ink tap, not a perfect geometric circle.
- Keep `2026` tiny, handwritten, and secondary near or below the signature unless the user asks to omit the year.

## Style Presets

Read `references/style-presets.md` before generating. Apply exactly one selected preset. The five styles must produce visibly different results in composition, marks, color, texture, and typography mood while preserving the same core source-photo relationship.

Do not mention or reproduce the mobile app UI, screenshots, buttons, badges, or watermarks from the demos. Use the demos only as style references.

## Workflow

1. Preserve the uploaded photo in the photo half:
   - Keep it realistic and photographic.
   - Preserve natural lighting, complete composition, clean texture, and the original subject relationships.
   - Do not stylize the photo half into illustration.
   - For output mode `1`, place the original photo on top and the generated illustration below.
   - For output mode `2`, do not include the original photo in the final image; use it only as source reference.
2. Analyze the photo for the illustration half:
   - Identify the most recognizable subject.
   - Preserve essential silhouette, proportion, pose, gesture, important objects, spatial relationship, and emotional tone.
   - Remove nonessential details, visual clutter, secondary objects, busy textures, and literal background complexity.
   - Collapse the scene into a few paper-cut/acrylic-print shapes instead of rendering the entire photo.
   - Keep only the number of elements needed for instant recognition, usually 3-7 visual components.
3. Apply the selected preset:
   - Use its composition scale, material, marks, palette strategy, and typography placement.
   - Keep the output premium, restrained, and highly designed.
   - Make color choices feel editorial and expensive, not cute, random, or over-saturated.
   - For photo-derived scenes, prefer a small editorial vignette on paper over a full-frame illustration.
4. Required Beya signature:
   - Add a clear small handwritten brand signature in the illustration half.
   - Use the user's signature name, rendered as a flowing handwritten signature in the Beya format.
   - For `beya`, render it like the latest reference image: loose lowercase cursive, muted olive-gray brush-pen ink, tall first stroke, connected letters, large `y` loop, long right tail, and final dot.
   - For any other name, create a custom abstract handwritten signature using the supplied name, with the same small lower-right placement, subdued ink, and handmade brush-pen feel.
   - Make the tail long enough that the signature reads as a logo-like mark rather than `beya.` typed in cursive.
   - Place the final dot far to the right of the letters, aligned with the tail endpoint.
   - Make the final dot loose and imperfect, not a neat circular period.
   - Do not use ordinary typed text for the signature.
   - Do not add `BY`, a literal `~`, or a separate dot line; the dot belongs visually at the far right of the signature tail.
   - Place the whole signature in the lower-right corner of the illustration half.
   - Keep `2026` tiny, handwritten, and secondary near or under the signature.
   - Keep the signature natural, sparse, and secondary to the illustration.
   - Do not add other titles, locations, short phrases, or object names unless the user explicitly asks for them.

## Prompt Construction

When using image generation, build the prompt from `references/prompt-template.md` and the selected preset in `references/style-presets.md`.

Include these non-negotiable constraints in the generation prompt:

- Output mode `1`: the full image is split into exactly two equal horizontal halves; the top half is the original uploaded photo as a real photo, and the bottom half is the generated paper-textured Beya illustration.
- Output mode `2`: generate only the paper-textured Beya illustration inspired by the uploaded photo; do not include the original photo half or any split layout.
- The illustration must not be a direct copy, filter, vector trace, or line-art conversion.
- The illustration must not become a realistic scenic painting or a detailed redraw of the source photo.
- The illustration should follow the demo grammar: small central or low vignette, rough paper texture, flat imperfect color blocks, sparse linework, and generous negative space.
- The illustration includes the required Beya-style handwritten signature and tiny `2026`.
- No UI overlays, phone interface elements, app labels, watermarks, or demo screenshot chrome appear in the final image.

## Quality Checks

Before finalizing, check that:

- For mode `1`, the split is visually 1:1, top and bottom, and the photo half still reads as the original real photo.
- For mode `2`, the final is a standalone illustration and does not include the source photo.
- The illustration half clearly matches the selected preset and is not a generic version of another preset.
- The illustration can be recognized from the photo with very few details.
- The illustration is visibly more abstract, smaller, and more paper-plate-like than a realistic painting.
- There are no busy backgrounds, dense decoration, large typography, or over-rendered details.
- The signature uses the supplied name in the Beya handwritten format, with a clearly elongated tail, distant imperfect dot, lower-right placement, and `2026` as tiny handwritten secondary year text.
- The mood is quiet, refined, poetic, durable, premium, and not childish.

## Reference

Read `references/prompt-template.md` and `references/style-presets.md` when writing a final reusable prompt, translating the template, or generating images in this style.
