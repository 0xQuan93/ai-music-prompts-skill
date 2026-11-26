# Zaal's Round B - WaveWarZ Red Line DJ

**Creator:** Zaal (BetterCallZaal) · **Date:** 25 Nov 2026 · **Status:** 2 tracks generated, auto-reviewed; Zaal's feedback pending · **From:** [Generation 3](../gen-003-club-workout-bangers/) (Red Line)

## Naming (from this round on)

Zaal, 25 Nov 2026: one Suno call per round, so each round makes **two new tracks, numbered 1 and 2**. Each feedback round gets the next letter: B, C, D, E, F... Suno titles: `<Working title> (B1)`, `(B2)`. Every song is WaveWarZ-related. Generations 1 to 3 keep their old names.

## Brief

A DJ-length, WaveWarZ version of Red Line, the Gen 3 track with the cleanest vocal. Gen 3's lessons applied:

- About 4 minutes (`duration: 240`) with "16 bars of drums only" at the start and end, so a DJ can blend in and out.
- "one memorable four-note siren synth riff on every drop" for a stronger drop hook.
- `abrupt ending` added to Exclude.
- Lyrics rewritten around WaveWarZ.

## Inputs

### Style of Music

```text
Bass house and Jersey club, 140 BPM, WaveWarZ battle-room workout banger.
Long DJ-friendly intro and outro, 16 bars of drums only at the start and end.
Hard four-on-the-floor kick, switching to Jersey club triplet kick bounce on the drops.
Growling mid-bass, punchy claps, one memorable four-note siren synth riff on every drop.
Mostly instrumental; one short chant hook, dry close lead vocal, little reverb.
Each drop heavier than the last; one bar of silence before the final drop.
Dry punchy drums, tight mono low end, loud but not over-limited.
```

### Exclude

```text
acoustic guitar, orchestral strings, ballad, lo-fi, trap 808 glides, rap verses, vocal chops, pitch-shifted vocals, formant effects, long hall reverb, slow tempo, abrupt ending
```

### Lyrics

```text
[Intro: 16 bars, drums only, four-on-the-floor kick and hats]

[Build: riser, claps speeding up]

[Drop: Jersey club bounce, growling bass, siren riff, instrumental]

[Break: drums cut, dry close vocal]
two names up, the wave decides

[Build: riser]

[Drop: hard bass house, siren riff, chant]
red line
(red line)
WaveWarZ don't fold

[Instrumental Break: bass and percussion]

[Break: one bar of silence]

[Final Drop: heaviest Jersey club bounce, siren riff, chant]
red line
WaveWarZ don't fold

[Outro: 16 bars, drums only, kick and hats, slow fade]
[End]
```

**Copyright filter:** the first attempt used "WaveWarZ, push it to the red line" and "push it" in the chant. Suno rejected both clips with "Your lyrics contain copyrighted material" and charged nothing. Rewriting those lines (no "push it") passed. Avoid well-known hook phrases in lyrics.

## Settings

| Model | Variety | Weirdness | Style Influence | Duration | Max Mode |
| --- | --- | --- | --- | --- | --- |
| v6 | 0 | 0.5 | 0.8 | 240 s target, not strict | Off |

## Credits

| Credits before | Credits after | Used | Calls | Tracks |
| --- | --- | --- | --- | --- |
| 9,940 | 9,930 | 10 | 1 (plus 1 rejected, free) | 2 |

A 4-minute track cost the same as a 2-minute one: 10 credits per call.

## Take log

Scored by Suno's listening model (`audio-listen`), 1 to 5. Machine first pass; Zaal's ears are the final call.

| Track | Link | Length | BPM / key | Club ready | Workout drive | Drop impact | Vocal clarity | AI artifacts | Vocals | Drums-only intro / outro | Siren riff memorable |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| B1 | [song](https://suno.com/song/d1b48a1f-4ccf-47dc-9474-4857d9325930) | 3:59 | 140 / G min | 3 | 5 | 4 | 4 | mild | 68% | 11 s / 10 s | yes |
| B2 | [song](https://suno.com/song/42bb4d3b-b0d0-42db-b525-d3f921f7eac0) | 3:59 | 140 / G min | 3 | 5 | 4 | 3 | mild | 45% | 15 s / 15 s | yes |

B1 map (approximate): intro drums to 0:11; drops at 0:45, 1:25, 2:00; Jersey club triplets from 2:15; final build 3:00 to 3:39; silence 3:40 to 3:44; final drop 3:45; outro 3:55.
B2 map: intro drums to 0:15; first drop 0:46, second 1:47, third 2:49. The listener's later timestamps for B2 ran past the track's real length, so trust B2's map only up to about 3:00.

## Lessons

- **Worked:** about 4 minutes on both (asked 240 s, got 239 s). The siren riff landed and is memorable on both, which fixes Gen 3's "drops have no hook". Workout drive stays 5 of 5.
- **Missed: the DJ intro and outro are too short.** "16 bars" at 140 BPM is about 27 seconds; we got 10 to 15 seconds (roughly 6 to 9 bars). Club-ready dropped from 4 to 3 because of it.
- **More vocals in a longer song:** B1 repeated the chant to 68%. The model filled the extra length with the hook.
- **Fix for Round C (one variable):** ask for "32 bars of drums only" at both ends (expect about half), or fix it in post (below). Post is the more reliable route.

## Teaching point: bars and seconds

One bar = 4 beats. At 140 BPM a beat is 60 / 140 = 0.43 s, so a bar is 1.71 s, and 16 bars = 27.4 s. B1's 11-second intro is about 6 bars, so a DJ has only 6 bars to blend. Check it yourself: count "1-2-3-4" from 0:00 on B1 until the bass comes in.

## Post-production

For club play, loop the drums-only bars at the start and end in a DAW to 16 or 32 bars, cutting on the bar line (see [`POST-GEN.md`](../../../POST-GEN.md)).

| Step | What was done | Tool | Who | Output file / location |
| --- | --- | --- | --- | --- |
| Stems / WAV export | | | | |
| DJ edit (extend intro / outro to 16-32 bars) | | | | |
| Mix | | | | |
| Master | | | | |
| Final file | | | | |

Songs stay private in Suno; nothing published.
