# Generations log

A public record of real tracks made with this skill: the exact inputs (style block, Exclude list, lyrics, settings) and what came out (take links, what worked, what didn't, what to change next). The point is to learn which prompt moves actually change the output, not just collect prompts.

## Layout

```text
generations/
  <creator>/
    gen-NNN-<track-slug>/
      README.md   inputs, settings, take log, lessons
```

One folder per generation, each with its own working title (never reuse an earlier generation's name). Suno clip titles: `<Working title> (Gen N <clip>)`. A generation is one prompt brief and the takes made from it. When you change the brief, start the next generation and link back to the one it came from.

## What each generation records

1. **Brief** - what the track is for, the reference (prior version, battle context), the lens used from `SKILL.md`.
2. **Inputs** - Style of Music, Exclude, Lyrics with metatags, exactly as pasted.
3. **Settings** - model (v6 / v6-wild / v6-mini), Variety, Weirdness, Style Influence, Max Mode, Persona, Cover/Remaster source.
4. **Take log** - one row per take: link, length, what landed, what missed.
5. **Lessons** - which descriptors or tags moved the result, which were ignored, and the one variable to change next.
6. **Credits** - Suno balance before and after, credits used, calls, clips, models.
7. **Pick** - which clip was chosen and why.
8. **Post-production** - every step after generation (stems, WAV, edits, mix, master), who did it, and where the final file lives. See [`POST-GEN.md`](../POST-GEN.md).

Every generation also gets a row in [`songs/INDEX.md`](../songs/INDEX.md).

Keep it honest: if a tag did nothing, say so. That is the useful part.

## Index

| Creator | Gen | Track | Lens | Status |
| --- | --- | --- | --- | --- |
| Zaal (BetterCallZaal) | [001](zaal/gen-001-electric-vibez-v2/) | WaveWarZ, the electric vibez (v2, house / Jersey club) | Club transformation | Done, Zaal picked Take A (v6), 20 credits |
| Zaal (BetterCallZaal) | [002](zaal/gen-002-electric-vibez-v2-clear-vocals/) | Electric Vibez: Clear Signal | Club transformation + Rubin reducer | 4 songs generated, auto-reviewed, 20 credits |
| Zaal (BetterCallZaal) | [003](zaal/gen-003-club-workout-bangers/) | Rep Count / Red Line | Club transformation | 4 songs generated, auto-reviewed, 20 credits |
