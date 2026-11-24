# Generations log

A public record of real tracks made with this skill: the exact inputs (style block, Exclude list, lyrics, settings) and what came out (take links, what worked, what didn't, what to change next). The point is to learn which prompt moves actually change the output, not just collect prompts.

## Layout

```text
generations/
  <creator>/
    gen-NNN-<track-slug>/
      README.md   inputs, settings, take log, lessons
```

One folder per generation. A generation is one prompt brief and the takes made from it. When you change the brief, start the next generation and link back to the one it came from.

## What each generation records

1. **Brief** - what the track is for, the reference (prior version, battle context), the lens used from `SKILL.md`.
2. **Inputs** - Style of Music, Exclude, Lyrics with metatags, exactly as pasted.
3. **Settings** - model (v6 / v6-wild / v6-mini), Variety, Weirdness, Style Influence, Max Mode, Persona, Cover/Remaster source.
4. **Take log** - one row per take: link, length, what landed, what missed.
5. **Lessons** - which descriptors or tags moved the result, which were ignored, and the one variable to change next.

Keep it honest: if a tag did nothing, say so. That is the useful part.

## Index

| Creator | Gen | Track | Lens | Status |
| --- | --- | --- | --- | --- |
| Zaal (BetterCallZaal) | [001](zaal/gen-001-electric-vibez-v2/) | WaveWarZ, the electric vibez (v2, house / Jersey club) | Club transformation | Inputs ready, takes pending |
