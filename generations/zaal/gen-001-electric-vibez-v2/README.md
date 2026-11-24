# Zaal's Generation 1 - WaveWarZ, the electric vibez (v2)

**Creator:** Zaal (BetterCallZaal) · **Date:** 24 Nov 2026 · **Status:** inputs ready, takes pending

## Brief

Second version of "WaveWarZ, the electric vibez", the most-battled track on WaveWarZ (38 battles, 21W / 17L as of Jul 2026). v1 sits around 125 BPM. v2 goal: a house / Jersey club banger built for battle rooms: one chantable hook, a physical groove, and a switch from four-on-the-floor house into Jersey club bounce.

- **Lens:** Club transformation (from `SKILL.md`): same hook every chorus, production changes around it.
- **Emotional tension:** euphoric and competitive on top, a little ruthless underneath.
- **Tempo choice:** 140 BPM. Jersey club usually lives around 130-145; house at 140 is fast but holds as a driving four-on-the-floor. A single tempo is safer than asking the model to change BPM mid-song.

## Inputs

### Style of Music (Take A / B)

```text
House and Jersey club hybrid, 140 BPM, electric and bouncy.
Four-on-the-floor house kick in the verses, switching to a Jersey club kick pattern with triplet kick bounce and bed-squeak chops on the hook.
Rubbery syncopated sub bass, crisp claps, open hats, one bright detuned synth stab as the signature.
Chantable call-and-response hook, stacked crowd chants, confident rhythmic lead vocal.
Filtered intro, drums cut before each drop, pocket of silence, then the hook hits wider and heavier.
Dry punchy drums, tight mono low end, short dark vocal delays, not over-limited.
Euphoric battle-room energy with a ruthless edge.
```

### Exclude

```text
trap 808 glides, acoustic guitar, orchestral strings, lo-fi tape warble, ballad, long hall reverb
```

### Lyrics

```text
[Intro: filtered house groove, half-spoken]
lights low, wave up
lights low, wave up

[Verse 1: four-on-the-floor, dry close vocal]
step in the room where the bass talk loud
two names up and the chain is the crowd
I don't need a mic when the floor says yes
every vote is a heartbeat in my chest

[Pre-Chorus: drums cut, rising claps]
hold it, hold it
let it build, let it build

[Chorus: Jersey club bounce, stacked chants]
electric vibez
(electric vibez)
WaveWarZ, light it up
(light it up)
electric vibez
(electric vibez)
WaveWarZ, run it up

[Verse 2: house groove returns, bass more syncopated]
you came to battle, I came to stay
thirty-eight rounds and I'm still in play
win or lose it, the wave don't stop
we keep it moving from the floor to the top

[Break: everything cuts, voice only]
wave up

[Build: chopped vocal, triplet kicks rising]
e-lec-tric, e-lec-tric

[Final Chorus: full Jersey club, heaviest bass, crowd chants]
electric vibez
(electric vibez)
WaveWarZ, light it up
(light it up)
electric vibez
(electric vibez)
WaveWarZ, run it up
(run it up)

[Outro: filtered groove fades, last chant]
wave up
[End]
```

## Settings

| Take | Model | Variety | Weirdness | Style Influence | Max Mode | Change vs previous |
| --- | --- | --- | --- | --- | --- | --- |
| A | v6 | 0 | 50% | Strong | Off | Baseline |
| B | v6-wild | 0 | 50% | Strong | Off | Model only (explore) |

One variable per take, per the skill's working loop. If Take B finds a better groove, carry it back to v6 in Generation 2.

## Take log

Fill in after generating.

| Take | Link | Length | Hook lands? | House to Jersey switch? | Vocal / chant | Notes |
| --- | --- | --- | --- | --- | --- | --- |
| A | | | | | | |
| B | | | | | | |

## Lessons

Fill in after listening.

- Descriptors that clearly moved the result:
- Descriptors or tags that were ignored:
- Pronunciation fixes needed (respell, hyphenate):
- One variable to change in Generation 2:

## Prompt checks (against `SKILL.md`)

- Style is sound only; no `[Verse]` tags in the style field.
- Seven short prose lines, identity first, about 12 concrete descriptors (inside the 8-15 sweet spot).
- Arrangement promises in the style (drums cut, silence, wider hook) are mirrored by section tags in the lyrics.
- Backing chants in parentheses on their own lines.
- No artist names or voice imitation.
- No LUFS numbers in the prompt; finish in a DAW with the checklist.
