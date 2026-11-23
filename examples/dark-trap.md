# Dark atmospheric trap

A complete Custom-mode prompt: style block, Exclude list, and lyric metatag structure.

## Style of Music

```text
dark atmospheric trap, 138 BPM halftime, minor-key synth loop, gliding 808 sub, sparse kick, triplet hi-hats, syncopated percussion, glassy bell motif, distorted vocal chops, pitched ad-lib hook, wide dark pads, tape-saturated, spring reverb, pockets of silence, cinematic riser into 808 drop, late-night menace
```

## Exclude

```text
bright, happy, clean pop vocal, EDM build, four-on-the-floor, acoustic guitar
```

On Udio, put the same list in **Style Reduction** rather than writing “no pop vocal” into the prompt.

## Lyrics / structure

Use these tags on their own lines, then add lyrics under each section.

```text
[Intro: drumless, synth loop, bells, distant vocal chop]

[Verse 1: sparse kick, triplet hats, 808 held back, dry close vocal]

[Pre-Chorus: cinematic riser, drums drop out]

[Chorus: 808 drop, full halftime, pitched ad-lib hook]

[Verse 2: 808 glides, syncopated percussion, vocal chops between lines]

[Pre-Chorus: riser, pocket of silence]

[Chorus: 808 drop, wide dark pads, stacked ad-libs]

[Bridge: drumless, spring reverb vocal, bells and pads]

[Final Chorus: hardest 808 drop]

[Outro: loop fades, last vocal chop, silence]
```

## Notes

- The style already asks for pockets of silence and a riser into the 808 drop; the pre-chorus tags should match that, not add a four-on-the-floor EDM build (that’s in Exclude).
- Keep the lead dry and close in the verses so the spring-reverb bridge and stacked chorus ad-libs actually contrast.
- After generation, finish levels in a DAW (see the mix/master checklist in `SKILL.md`). Don’t try to prompt a LUFS number into the model.
