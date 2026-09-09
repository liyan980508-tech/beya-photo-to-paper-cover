# Beya Photo to Paper Cover Skill

A Codex skill for turning uploaded photos into quiet Beya-style paper-cover illustrations.

## What It Does

This skill asks for three inputs before generating:

1. Signature name
2. Style number from `1` to `5`
3. Output mode:
   - `1`: split image, original photo on top and illustration below
   - `2`: illustration only

## Styles

1. Quiet Geometry Poster
2. Still Object Collage
3. Wax Pencil Keepsake
4. Coastal Postmark Print
5. Pastoral Washbook

## Install

Copy the `beya-photo-to-paper-cover` folder into your Codex skills directory:

```bash
~/.codex/skills/beya-photo-to-paper-cover
```

Then invoke it in Codex with:

```text
Use $beya-photo-to-paper-cover
```

## Included

- `beya-photo-to-paper-cover/`: the Codex skill
- `palette/`: Beya paper-cover palette reference files

## Notes

The skill is designed to avoid realistic redraws. Its core visual grammar is a small, abstract, paper-textured vignette with large negative space, restrained color, dry acrylic blocks, and handmade marks.
