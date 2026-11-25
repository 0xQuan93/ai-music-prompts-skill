# Zaal's Generation 2 - WaveWarZ, the electric vibez (v2), clear vocals

**Creator:** Zaal (BetterCallZaal) · **Date:** 25 Nov 2026 · **Status:** 4 songs generated, auto-reviewed; Zaal's pick pending · **From:** [Generation 1](../gen-001-electric-vibez-v2/) (Zaal picked Take A, v6)

## Brief

Zaal, 25 Nov 2026: "one of the goals is to showcase vocals on these tracks and clean them up, and make it not sound like AI vocals... generate some music where initially there are fewer vocals, and focus on clarity of vocals."

- **Goal:** fewer vocals, and the ones that are there clear and human.
- **Kept from Gen 1:** 140 BPM, Jersey club bounce on the hook, dry punchy mix, the Exclude list, v6.
- **Gen 1 fix applied:** house first in the identity line ("deep-house-driven Jersey club, steady four-on-the-floor kick under every verse") and "sung-chant lead vocal" in place of "rhythmic lead vocal".

### What `SKILL.md` says, and how it was used

| Skill lesson | Where it comes from in `SKILL.md` | Used as |
| --- | --- | --- |
| "dry close lead, controlled sibilance, short dark delay throws" | Mix/master vocabulary table, Vocal chain row | Style line 4 and 5 |
| "uncluttered midrange, vocal sits in a carved pocket, no muddy low-mids" | Mix/master vocabulary table, Subtractive EQ row | Style line 5 |
| Single dry performances, not stacked walls; contrast from subtraction | Rubin minimal (reducer) lens | Style line 6, `no stacks` tags |
| Leave space; mute instruments under key lines | Neptunes bounce lens | Style line 6 |
| Mirror the style block in the tags | Lyric metatag cheat sheet, writing notes | `[Bridge: no drums, raw close vocal]`, `[Instrumental Break]` |
| 8 to 15 concrete descriptors, identity first; Variety 0 | Suno section, community-observed notes; Working loop | 7 lines, Variety 0 |
| Describe the vocal by range, delivery, timbre, never a singer's name | Style template | "warm mid-range, natural human tone" |
| Metatags bias, they don't switch | What the models respond to | Tested below: instrumental tags did not stop vocal chops |

## Inputs

### Style of Music (Take A / B)

```text
Deep-house-driven Jersey club, 140 BPM, steady four-on-the-floor kick under every verse.
Jersey club triplet kick bounce on the hook, rubbery sub bass, crisp claps, one bright detuned synth stab.
Mostly instrumental with long breaks; vocal only on the hook and the bridge.
Sung-chant lead vocal, warm mid-range, natural human tone, dry close lead vocal, intimate and present, little reverb.
Vocal sits in a carved pocket, uncluttered midrange, controlled sibilance, short dark delay throws.
Single dry vocal performance, not stacked; instruments drop out under key lines.
Dry punchy drums, tight mono low end, not over-limited.
```

### Exclude

```text
trap 808 glides, acoustic guitar, orchestral strings, lo-fi tape warble, ballad, long hall reverb, rap verses, stacked choir vocals, autotune
```

Added vs Gen 1: `rap verses, stacked choir vocals, autotune`.

### Lyrics

Short on purpose: one hook, two bridge lines, the rest instrumental sections.

```text
[Intro: instrumental, filtered house groove]

[Verse: four-on-the-floor house, instrumental]

[Pre-Chorus: drums cut]
hold it

[Chorus: Jersey club bounce, clear sung chant, single voice]
electric vibez
WaveWarZ, light it up
electric vibez
WaveWarZ, run it up

[Instrumental Break: house groove, no vocals]

[Bridge: no drums, raw close vocal]
win or lose it, the wave don't stop
we keep it moving from the floor to the top

[Build: triplet kicks rising, instrumental]

[Final Chorus: full Jersey club, clear lead vocal, no stacks]
electric vibez
WaveWarZ, light it up

[Outro: instrumental, filtered groove fades]
[End]
```

## Settings

| Take | Model | Variety | Weirdness | Style Influence | Max Mode | Change vs previous |
| --- | --- | --- | --- | --- | --- | --- |
| A | v6 | 0 | 0.5 | 0.8 | Off | Gen 1 baseline controls |
| B | v6 | 0 | 0.5 | 0.95 | Off | Style Influence only |

Generated through Suno's MCP server (`audio-create`, custom mode) on 25 Nov 2026, 10:55 UTC.

## Credits

| Credits before | Credits after | Used | Calls | Clips | Model | Per clip |
| --- | --- | --- | --- | --- | --- | --- |
| 9,980 | 9,960 | 20 | 2 | 4 | v6 | 5 |

Scoring with `audio-listen` cost 0.

## Take log

Scored by Suno's listening model (`audio-listen`) with a vocal-focused brief. Clarity is 1 to 5. Vocal share is the estimated percent of the track with vocals or vocal chops. Machine first pass; Zaal's ears are the final call.

| Clip | Link | Length | BPM / key | Vocal clarity | AI artifacts | Vocal share | House verses | Jersey hook | Bridge dry and exposed |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| A1 | [song](https://suno.com/song/49281707-ebb0-4a61-8091-9882f88ca369) | 1:31 | 138.4 / B min | 4 | mild | 48% | yes | no | no |
| A2 | [song](https://suno.com/song/db524c7b-4e88-4fbe-9b4e-4a3a8d8e4d03) | 1:46 | 139 / A# min | **5** | mild | **38%** | no | yes | no |
| B1 | [song](https://suno.com/song/0c87669b-6eb2-434b-a8e1-0c3510aa4aea) | 1:32 | 137.9 / A# min | 4 | mild | 58% | no | yes | partial |
| B2 | [song](https://suno.com/song/ea6bab65-9271-44c5-9ee1-c7f856135998) | 1:23 | 140.5 / G min | 2 | strong | 65% | yes | yes | no |

Artifact notes:

- **A1:** phasey, warbly upper tone; mildly smeared sibilants on the layered vocals; consonants a little soft.
- **A2:** clear diction; the only artifacts are tuning / formant processing and chopped delays that sound intentional. No metallic warble or slurred consonants.
- **B1:** subtle metallic warble, smeared sibilants, quantized-sounding pitch movement.
- **B2:** robotic pitch-shifted tone, heavily chopped phrasing, smeared consonants. Least intelligible.

## Lessons

- **Best clip for the goal: A2.** Clearest vocal (5 of 5), fewest vocals (38%), Jersey club hook lands.
- **Fewer vocals only half worked.** The lyric is short, but every clip still runs 38 to 65% vocal: the model fills instrumental sections with vocal chops. `[Instrumental Break: ... no vocals]` biased it, it did not switch it off (the skill's own "metatags bias, they don't switch").
- **Higher Style Influence made vocals worse, not cleaner.** Take B (0.95) averaged 62% vocal and the only strong-artifact clip; Take A (0.8) averaged 43% with clarity 4 and 5. Keep 0.8.
- **The dry bridge never happened.** 0 of 4 fully dry and close; every bridge came back with reverb or processing. "raw close vocal" in the tag and "little reverb" in the style were not enough.
- **House verses improved:** 2 of 4 clear (A1, B2) vs 0 of 4 in Gen 1. Putting house first in the identity line helped.
- **Change for Generation 3 (one variable):** add the processing the model keeps adding to Exclude: `vocal chops, pitch-shifted vocals, formant effects, vocal reverb`. Keep everything else, Style Influence 0.8.

## Zaal's pick

Pending.

## Post-production

Nothing done yet. Suggested cleanup for the picked clip (see [`POST-GEN.md`](../../../POST-GEN.md)):

1. Pull stems so the vocal can be worked on alone.
2. De-ess and gently control sibilance (A1, B1 have smeared sibilants).
3. Subtractive EQ on the vocal: cut mud and the phasey upper resonance before adding air.
4. Reduce or replace the reverb on the bridge vocal; keep it dry and close.
5. For the most-processed parts, mute the vocal chops in the instrumental sections so the voice only shows up on the hook and bridge, as the brief asked.

| Step | What was done | Tool | Who | Output file / location |
| --- | --- | --- | --- | --- |
| Stems / WAV export | | | | |
| Vocal cleanup (de-ess, EQ, reverb) | | | | |
| Edits | | | | |
| Mix | | | | |
| Master | | | | |
| Final file | | | | |

Songs stay private in Suno; nothing published.

## Open questions for Zaal

Not used in this generation; each needs his yes (credits or a change to the song):

- **Max Mode** - SKILL.md says it helps vocal and style consistency; costs a multiple of the song's credits.
- **Subtle Remaster** of the picked clip - aimed at vocal clarity without changing the song.
- **Persona** from the picked clip - lock in the voice for future generations.
