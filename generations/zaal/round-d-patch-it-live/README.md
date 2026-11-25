# Zaal's Round D - Patch It Live (lore Chapter 5)

**Creator:** Zaal (BetterCallZaal) · **Date:** 25 Nov 2026 · **Status:** 4 tracks generated, auto-reviewed; Zaal's pick pending · **From:** [Round C](../round-c-wavewarz-open-floor/) · **Order:** ORD-602 (Notion Agent orders)

## Brief

First round built from the WaveWarZ lore bible v1 (ORD-601). **Chapter 5, "Patch It Live":** the open-source crew Patch Notes rebuild a broken track live in front of the Chain and turn the night. Clever, groovy; the comeback.

- Genre: UK garage 2-step, 132 BPM: skipped kicks, swung hats (Patch Notes' signature).
- Vocal: breathy male and female duo, close and dry.
- Hooks from the lexicon: "patch it live", "open the code, open the Floor". Sung twice only.
- Real verses about WaveWarZ, The Zow (spelled phonetically from this round on), the Chain and open source.
- Clear-vocal lessons kept: vocal processing in Exclude, Style Influence 0.8, Variety 0.
- One variable between the two calls: Weirdness 0.5 (D1, D2) vs 0.35 (D3, D4), testing Round C's note that lower Weirdness may cut the extra repetition.

## Inputs

### Style of Music

```text
UK garage 2-step, 132 BPM, WaveWarZ comeback anthem about open-source builders.
Skipping 2-step kick pattern, swung shuffled hi-hats, crisp rimshots, warm organ bassline, short organ stabs.
Breathy male and female duo vocal, close and dry, clear diction, every word understood, little reverb.
Verses tell a story; short two-line chorus sung only twice.
Clever, groovy, late-night club energy. Long DJ-friendly intro and outro with drums only.
Dry punchy mix, tight mono low end.
```

### Exclude

```text
vocal chops, pitch-shifted vocals, formant effects, vocal reverb, long hall reverb, four-on-the-floor kick, trap 808 glides, rap verses, acoustic guitar, orchestral strings, ballad, repetitive chant loops, abrupt ending
```

### Lyrics

```text
[Intro: drums only, 2-step shuffle, filtered organ bass]

[Verse 1: male and female duo, breathy, close and dry]
the track went down in the middle of the wave
the kick fell out and the Chain went quiet
two of us stepped up with a laptop open
every line of the fix on the wall where you can read it

[Verse 2: duo trading lines, close and dry]
nobody owns the source, so everybody holds it
we fork the broken bar and we bring it back in time
WaveWarZ on the Floor, The Zow is watching
the bug becomes the groove when the crowd can see the line

[Pre-Chorus: kick drops out, hats only]
commit the swing, commit the bass
ship it while they're in the place

[Chorus: duo in unison, clear words]
patch it live
open the code, open the Floor

[Instrumental Break: skipping kicks, swung hats, organ bass stab]

[Verse 3: female lead, breathy, close]
we don't hide the fixes in a room behind the stage
every artist on the Chain can take the tool and build
no wave gets deleted, every block remembers
the night we turned it round with the code we gave away

[Bridge: drums out, soft organ, duo whisper-close]
broken was the best thing, now the whole room knows how

[Build: 2-step kicks return, hats rising]

[Final Chorus: duo in unison, crowd answers once]
patch it live
open the code, open the Floor

[Outro: drums only, 2-step shuffle, long fade]
[End]
```

## Settings

| Call | Clips | Model | Variety | Weirdness | Style Influence | Duration | Max Mode |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | D1, D2 | v6 | 0 | 0.5 | 0.8 | 240 s target, not strict | Off |
| 2 | D3, D4 | v6 | 0 | 0.35 | 0.8 | 240 s target, not strict | Off |

Suno gives both clips of a call the call's title, so D2 shows in Suno as "Patch It Live (D1)" and D4 as "Patch It Live (D3)". The IDs below are the record.

## Credits

| Credits before | Credits after | Used | Calls | Tracks |
| --- | --- | --- | --- | --- |
| 9,920 | 9,900 | 20 | 2 | 4 |

## Take log

Scored by Suno's listening model (`audio-listen`), 1 to 5 (AI artifacts: 5 = none). Machine first pass; Zaal's ears are the final call.

| Track | Link | Length | BPM / key | Hook | Groove (2-step) | Vocal clarity | AI artifacts | Vocal share | Chorus count | "The Zow" heard as |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| **D1** (pick) | [song](https://suno.com/song/46b413d3-eeb8-40ae-95c7-b353af662a5a) | 3:59 | 133.6 / A# min | 4 | **5** | 4 | 4 (slight smoothing on sustained notes) | ~68% | 2 | rhymes with cow |
| D2 | [song](https://suno.com/song/fcad31a5-f33b-4b95-a92b-e34a62ee7a11) | 3:59 | 133.5 / A# min | 4 | 3 (chorus goes straight four) | 3 | 3 (phasey, metallic smear) | ~45% | 2 + extra refrain bits | rhymes with how |
| D3 | [song](https://suno.com/song/9498fd0d-ee63-4ed9-b814-c62bf5eae222) | 3:52 | 133.3 / A# min | 4 | **5** | 4 | 4 (slight metallic reverb sheen) | ~75% | 3 | "Zoo / Zou" |
| D4 | [song](https://suno.com/song/7c8d9c74-76ad-427a-8af6-ed98ecee9721) | 3:59 | 133 / G min | 4 | **5** | 4 | 3 (metallic sustained notes) | ~75% | 2 | rhymes with how |

**Pick: D1.** Real 2-step groove, chorus exactly twice, cleanest vocal, "The Zow" said right, and the lowest vocal share of the strong takes (Zaal wants fewer vocals). Runner-up: D4.

## Lessons

- **"The Zow" spelling works.** 3 of 4 takes said it right (rhymes with now); D3 drifted to "Zoo". Round C sang "ZAY-oh" and "Desire".
- **UK garage lands on v6.** 3 of 4 takes scored 5 for a real 2-step groove. Putting `four-on-the-floor kick` in Exclude helped; D2 still slid into a straight four on the chorus.
- **Hook twice mostly held:** D1 and D4 sang it twice; D3 added a third; D2 added refrain fragments. Better than Round C.
- **Weirdness 0.35 did not clearly fix repetition** (D3 added a chorus) and did not improve artifacts. Keep 0.5; drop this variable.
- **Drums-only intro and outro still never land** (0 of 4, same as Round C). Fix in post with a DJ edit, or try a `[Intro: 16 bars kick and hats only, no vocals]` style tag next round.
- **Vocal share is high** (45 to 75%). For fewer vocals, cut Verse 3 or the bridge next time.

## Post-production

| Step | What was done | Tool | Who | Output file / location |
| --- | --- | --- | --- | --- |
| Stems / WAV export | | | | |
| DJ edit (drums-only intro/outro) | | | | |
| Mix | | | | |
| Master | | | | |
| Final file | | | | |

Songs stay private in Suno; nothing published.
