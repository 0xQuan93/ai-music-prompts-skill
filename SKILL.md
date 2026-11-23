---
name: AI music prompts
description: Use when writing or refining prompts for Suno (v6 / retired v4–v5), Udio, or similar AI music generators; when translating producer and mix-engineer techniques into style descriptors; or when finishing a generated export in a DAW.
---

# AI music prompts

Write prompts that describe a *record*, not a wish list. Genre, groove, vocal character, arrangement contrast, and production feel do more work than "hit song, professional mix, radio ready." After generation, treat the file as a demo: stems and a short DAW pass still matter.

This skill is for prompting and finishing. It is not a license to clone a living artist's voice. Describe production feel, era, and arrangement; do not ask the model to impersonate a specific singer.

## When to use

- The user wants a Suno, Udio, or similar prompt (style field, lyrics, or both).
- They want a track in a producer "lens" (sparse Neptunes bounce, Rubin-minimal, glossy pop, hard rock impact, club transformation).
- They have lyrics and need structure metatags plus a style block.
- They exported a generation and need a practical mix/master checklist before release.

## Prompt structure

Keep **style** and **lyrics** in their proper places. Do not put `[Verse]` / `[Chorus]` tags in the style field.

### Suno (Custom mode)

As of September 2026, new generations run on the **v6 family**. Official help: v6 (precise/polished, Pro/Premier), **v6-wild** (more varied, Pro/Premier), **v6-mini** (faster, all plans). Prior models are retired; existing library tracks still play, remaster, and cover, but new iterations use v6. Generations can run up to **8 minutes**; use **Extend** for more. **Max Mode** costs extra credits and is best for songs longer than about two minutes, tight covers, and vocal/style consistency. Set the **Variety** slider to **0** if you need the style text followed closely (Variety rewrites style prompts to add variation).

Two fields:

1. **Style of Music** — sound only: genre, mood, tempo, instruments, vocal character, production. Plain, concrete language. Official guidance: latest models read rich conversational prompts for mood, instrumentation, structure, and texture.
2. **Lyrics** — lyrics plus structure metatags, each tag on its own line.

**Style template** (front-load identity; trim rather than stack competing adjectives):

```text
[genre + subgenre], [BPM or tempo feel].
[drum / bass character]. [harmony / signature texture].
[lead vocal: range, delivery, gender/timbre — not a celebrity name].
[arrangement contrast: sparse vs stacked, dropouts, bridge, finale].
[production feel: dry/wet, close/wide, tape/digital, space].
[emotional undertow — one concrete tension, not a mood pile].
```

**Controls that actually exist (official):**

- **Exclude** (Advanced Options): instruments, genres, or elements you do not want.
- **Creative sliders:** Weirdness (Safe → Chaos; 50% is the expected result), Style Influence (Loose → Strong). Raise Style Influence when the style block is deliberate.
- **Cover:** restyle an existing *song you created* while keeping the melody. Not for other people's tracks.
- **Remaster:** subtler pass for mix, balance, sonic character, and vocal clarity while keeping structure, lyrics, and arrangement. Variation: Subtle / Normal / High. Not for lyric or genre overhauls (use Cover).
- **Personas / Voices:** capture vocal + style essence from a track (or a verified voice sample) and reuse it. Selecting a Persona auto-fills Style of Music. Combine with Cover when you want voice, structure, and style moved together.
- **Stems / WAV / MIDI export** (paid): pull the generation into a DAW rather than "mastering" only inside the generator.
- **Prompt enhancement:** optional expander for a rough genre idea. Edit the result; do not ship the first expansion uncritically.

**Community-observed, not official:** Style field often cited at ~1,000 characters on late v4.5+ models, Exclude ~200; a mid-length style (about 8–15 concrete descriptors, not 25+ competing tags) is a commonly reported sweet spot; tag *order* may weight earlier terms more. Confirm limits in the current UI and put the identity first.

### Udio (official help)

One **Prompt** field: topic or free-form text, then comma-separated genre/mood/tempo/instrument/vocal tags. Official pattern:

```text
A song about [concrete scene or subject], [genre], [mood], [2–3 instruments], [vocal feel]
```

Official techniques:

- Repeat a word to emphasize it.
- Era tags work ("1970s disco groove", "1980s-inspired synthwave").
- Scene-based prompts often beat abstract mood adjectives.
- `in the style of [name]` is documented as a *musical feel* reference; Udio states it will not copy an artist's voice.
- **Style Reduction** (Advanced Controls) is the negative-prompt equivalent: list genres, styles, or concepts to play down. Do not write "no saxophone" in the prompt; specify the ensemble you want, and put leftovers in Style Reduction.
- **Manual Mode:** exact tags only, no free-text auto-refine; better for custom lyrics, lyrics may be more generic.
- Custom lyrics: structure tags such as `[Chorus]`, `[Guitar Solo]`, `[Scream]`; parentheses for backing vocals.
- Pronunciation: hyphenate syllables, spell acronyms, use accent marks to move stress.
- Instrumentals: Instrumental Mode, or instrument tags.

### What the models respond to (verified vs folklore)

**Works (official or strongly evidenced):**

- Concrete production language: "dry clipped percussion," "warm syncopated sub bass," "close dry vocal," "stacked chant choruses," "drumless bridge."
- Arrangement contrast in the style *and* matching section tags in the lyrics.
- One clear groove + one signature texture, not a studio inventory.
- Exclude / Style Reduction for unwanted colors.
- Iterating: generate several takes, change one variable, keep what works. Cover or Remaster instead of rewriting a good performance from scratch.

**Folklore or weak:**

- Huge style dumps ("cinematic, epic, masterpiece, Grammy, 8k audio, professionally mastered"). These compete and often flatten the result.
- Treating metatags as hard switches. They *bias* section identity, density, and energy; they do not guarantee a drop, a key change, or a perfect repeat.
- Asking the model to hit a LUFS number or a plugin chain. Write the *sound* ("breathing dynamics, not over-limited") and finish levels in a DAW.
- Assuming "in the style of [star]" will clone the voice. It should not, and should not be the goal.

## Producer-style lenses (prompt modules)

Drop one lens into the style block. Do not stack all of them.

### Rubin minimal (reducer)

Philosophy, from Rubin in his own words: get the point across with the least information; "less is more, but to get less you have to do more"; a wall of doubled guitars becomes generic, while one player with fingers on the strings stays human. Vibe and performance over polish. He has called himself a reducer, not a producer.

**Module:**

```text
Sparse arrangement, only essential parts, lots of unfilled space.
Single dry performances, audible fingers and room, not stacked walls of sound.
Intimate, present vocal; little reverb. Feel and performance first, polish second.
Quiet verses, no extra layers "for size"; contrast comes from subtraction.
```

### Neptunes bounce (Pharrell / Chad Hugo)

Verified signatures: Pharrell described the era as minimal — "the least amount of sounds we could use, the better," sparseness that makes you react, and "Drop It Like It's Hot" as a spray-paint "ssss" on top. They called them "skeleton songs": dead-silence pockets, jolting mechanical drums, sometimes no bass. Chad Hugo: usually quantize kicks and snares, leave hats looser for a live feel; make drums hit hard in the body; mute parts so vocals stand out; odd presets and small FX (gate-reverb perk on "Grindin'"). Community craft notes (useful, slightly softer evidence): short pitched-up snares/hats, more sustained kicks, almost no reverb, clavs / electric pianos / synthetic guitars, syncopated chord stabs.

**Module:**

```text
Minimal futuristic funk-hop, skeleton arrangement, pockets of dead silence.
Tight quantized kick and snare, swung live hats, short pitched-up snare snap, sustained kick.
Sparse syncopated stabs, one odd percussive or sci-fi accent, almost no reverb, punchy and dry.
Leave space for the vocal; mute instruments under key lines rather than filling every beat.
```

### Ghenea pop clarity

Ghenea’s own rule: there is no bag of tricks; the song dictates the treatment. Do not get lost in kick/snare fetish — ask whether the song comes across and affects people, then maximize that special thing. Tools are song-by-song (he has mentioned compressors, de-essers, delays, convolution reverbs as regular options, not a fixed vocal chain).

**Module:**

```text
Modern pop mix, vocal sits forward and clear in the center, uncluttered midrange.
Tight, polished, emotionally direct; every part serves the hook.
Clean low end, controlled sibilance, tasteful delay throws, glossy but not brittle.
Chorus gets wider and fuller without burying the lead.
```

### CLA rock impact

From CLA walkthroughs and mix interviews: LCR placement — guitars hard left/right, vocal / bass / kick / snare in the center; compress the vocal into a similar dynamic range as the guitars so it stays above them; don’t be shy with guitar weight; section-dependent space (long anthemic halls in open sections, tight and dry when the band hits); mix into simple bus processing, be careful crushing the drum bus with a limiter; nothing is judged in solo.

**Module:**

```text
Hard-hitting rock, LCR image: wide hard-panned guitars, vocal and rhythm section locked in the center.
Aggressive but musical compression, vocals riding above a wall of guitars.
Open sections can bloom with longer hall; the band sections stay tight, dry, and punchy.
Air on top, weight in the low end, both still able to breathe.
```

### Scheps / Pensado punch and space

Scheps: learn every part before balancing; he uses a lot of **parallel compression** and relatively few effects; guitar-rock impact comes from balance that "makes things explode." Pensado: catalog first impressions; keep an overview of the song; put most effects on sends, not inserts; dark (not trebly) delays on vocals, often short; parallel movement rather than drowning the dry lead.

**Module:**

```text
Explosive but balanced; punch from parallel-compressed drums and close dry lead.
Few effects, mostly short dark vocal delays and one shared room.
Chorus hits bigger through arrangement and punch, not a wash of reverb.
```

### Club transformation (arrangement lens)

Useful writing/production recipe: one chantable hook, one physical groove, one emotional contradiction; *change the production around the hook* rather than repeating identical sections. Subtraction can be the drop (drums out under a gang vocal). Three shapes: direct pop (verse / lift / chorus), escalating transformation, or club progression (same vocal, changing rhythmic rooms).

**Module:**

```text
Memorable short hook, physical drum-and-bass groove, one signature texture.
Each chorus keeps the same phrase but changes bass, drums, density, or vocal treatment.
One major turn: drumless bridge, chopped-vocal build, or distorted finale.
Bright surface, uneasy undertow.
```

## Mix/master vocabulary → prompt descriptors

Models do not run your plugin chain. Translate the technique into audible language:

| Technique | Prompt language that tends to land |
| --- | --- |
| Gain staging / headroom | "clean headroom, not clipped, dynamics preserved" |
| Subtractive EQ / uncluttered mids | "uncluttered midrange, vocal sits in a carved pocket, no muddy low-mids" |
| Parallel compression | "punchy parallel-compressed drums, explosive chorus, close dry lead" |
| Bus glue | "glued mix, cohesive, slightly compressed but still breathing" |
| Vocal chain | "dry close lead, controlled sibilance, short dark delay throws, stacked doubles on the hook" |
| Low-end management | "tight mono sub, kick and bass locked, no rumble, club-ready low end without mud" |
| Stereo width | "hard-panned guitars, narrow center for kick-snare-bass-vocal, wide hooks, mono-compatible" |
| Saturation | "warm tape saturation, analog grit, slight harmonic edge, not harsh digital clipping" |
| Reverb / delay sends | "mostly dry; short room on drums; one hall that opens only in the chorus; dark 1/8-note vocal delay" |
| Reference / restraint | "reference-level dynamics, not over-limited, punch over loudness" |
| Rubin space | "sparse, unfilled space, single performances, fingers on strings" |
| Neptunes dryness | "dry punchy drums, almost no reverb, pockets of silence" |

## Lyric metatag cheat sheet

Put each tag **alone on its line**. No leading/trailing spaces. Inline tags mid-lyric are often ignored (community observation). Tags are generally case-insensitive.

**Structure (most reliable):**

```text
[Intro]
[Verse] or [Verse 1]
[Pre-Chorus]
[Chorus]
[Bridge]
[Break]
[Build]
[Drop]
[Instrumental] or [Instrumental Break]
[Outro]
[End]
```

**Useful color tags (bias performance; less consistent than structure tags):**

```text
[Whisper] / [Whispered]
[Spoken] / [Spoken Word]
[Belted] / [Falsetto]
[Choir] / [Harmony] / [Harmonized]
[Rap]
[Ad-lib]
[Guitar Solo] / [Synth Solo] / [Piano Solo]
[Fade In] / [Fade Out]
```

**Per-section direction** (community pattern, not an official syntax guarantee):

```text
[Chorus: full groove, stacked chants]
[Bridge: no drums, raw close vocal]
[Build: chopped vocals, rising tension]
[Final Chorus: distorted drums, heavy bass, exposed lead]
```

**Backing vocals:** put doubles and answers in `(parentheses)` on their own line or after the lead — documented on Udio; often works in Suno too.

**Writing notes that sit well on these models:**

- Hook first: a short phrase you can chant without accompaniment.
- Specific images and mouthfeel over explained emotion. Leave some connective tissue out.
- Keep chorus lines shorter and more repeatable than verses.
- Mirror the style block in the tags: if you promised a drumless bridge, tag it and write like it.
- If a word is mispronounced, respell or hyphenate and regenerate the section rather than padding the style field.

Suggested starting shape (adapt, don’t transcribe): hook tease 4 bars; verse 8; optional lift 4; chorus 8; verse 8; chorus 8; transformation 8; altered final hook 8–16.

## Example prompts

Generic examples. Swap genre nouns, keep the structure.

### 1. Rubin-minimal indie folk

**Style**

```text
Spare indie folk, 72 BPM. One dry acoustic guitar, audible fingers, soft room tone.
Low upright bass enters late. Brushed snare only in the second verse, no drum kit wall.
Close masculine vocal, almost spoken in the verses, unadorned melody in the chorus.
Minimal arrangement, lots of unfilled space, performance and feel over polish.
Quiet heartbreak, nothing cinematic.
```

**Exclude / Style Reduction:** stacked harmonies, big drums, lush strings, stadium reverb

**Lyrics (excerpt)**

```text
[Intro]
[Verse]
the kettle clicked and I let it sit
your cup is still on the drainboard
[Chorus]
if you come by, the light is on
I won't ask you to stay
[Bridge: voice and guitar only]
...
[Outro]
```

### 2. Neptunes-style bounce

**Style**

```text
Minimal futuristic funk-hop, 98 BPM. Skeleton beat, pockets of dead silence.
Tight quantized kick and snare, swung hats, short pitched-up snare, sustained kick.
Sparse syncopated clav stabs, one odd spray-paint hiss and a tiny sci-fi blip.
Dry, almost no reverb, punchy and close. Playful masculine hook, rhythmic verses.
Leave space; mute the stabs under the vocal.
```

**Exclude:** trap 808 glides, crowded sample loops, long hall reverb, orchestral layers

### 3. Ghenea-clear modern pop

**Style**

```text
Modern alt-pop, 104 BPM. Tight punchy drums, clean sub bass, bright but smooth synths.
Expressive feminine lead, intimate verses, stacked doubles and wide hook on the chorus.
Uncluttered midrange, vocal forward and emotionally direct, short dark delay throws.
Polished and glued, still breathing, not over-limited. Chorus wider and fuller, same melody.
```

**Exclude:** lo-fi warble, deathcore, spoken-word monologue

### 4. CLA rock anthem

**Style**

```text
Hard-hitting alternative rock, 152 BPM. Big dry punchy drums, centered kick and snare.
Heavy hard-panned rhythm guitars, bass locked to the kick, lead vocal compressed and forward in the center.
Open intro can bloom; once the band hits, stay tight and aggressive. Air on top, weight down low, both breathing.
Anthemic chorus, gang vocals on the last hook, short guitar fill, no mushy hall on the kit.
```

### 5. Club-pop transformation

**Style**

```text
Left-field electronic club-pop, 132 BPM. Syncopated rubbery sub bass, crisp off-kilter percussion, hand claps.
Expressive masculine lead, conversational rhythmic delivery, selective tuning.
Intimate sparse verses, explosive stacked-chant choruses, metallic synth accents, sudden silences.
Drumless vulnerable bridge, chopped-vocal build, distorted rave finale.
Late-night euphoria with loneliness underneath.
```

**Lyrics (shape)**

```text
[Intro: filtered, half-spoken]
[Verse 1: sparse, close vocal]
[Pre-Chorus: drums cut]
[Chorus: full groove, stacked chants]
[Verse 2]
[Chorus]
[Bridge: no drums, raw voice]
[Build: chopped vocals, rising tension]
[Final Chorus: distorted rave drums, heavy bass]
[Outro: everything cuts, fading sub]
```

### 6. WaveWarZ battle-style track

**Style**

```text
High-energy battle-rap club hybrid, 140 BPM, half-time hook.
Dry punchy drums, tight mono sub, syncopated hats, one distorted stab and a siren accent.
Aggressive rhythmic verses, call-and-response chants, stacked gang vocals on the hook.
Sudden dropouts before the drop, no-fill bars so the vocal hits, then a wider, heavier chorus.
Close dry lead, short dark delays, almost no hall. Competitive, nocturnal, crowd-cut energy.
Not over-limited; punch and space over wall-of-loudness.
```

**Exclude:** acoustic singer-songwriter, orchestral ballad, lo-fi tape mush

**Lyrics (excerpt)**

```text
[Intro]
[Verse 1: dry, close, rhythmic]
[Build]
hold the line
[Drop: full drums, heavy sub]
[Chorus: gang vocals, call and response]
WAVEZ ON
(wavez on)
[Verse 2]
[Break: drums cut]
[Final Chorus: wider, heavier, stacked]
[Outro]
```

## Post-generation mix/master checklist (DAW)

Generator "remaster" can clean a print. A release still wants stems or a WAV in a real session, plus a reference track in the same genre.

1. **Import & organize.** WAV (or tempo-locked WAV / stems) at the session rate. Name and color tracks. Do not start processing a messy session (CLA).
2. **Reference.** Level-match a commercial reference. Note kick/bass weight, vocal height, and chorus lift — not just loudness.
3. **Gain staging.** Set track faders so the mix bus is not already slamming. A common analog-modeled starting zone is peaks around −18 to −20 dBFS at unity; leave headroom. (iZotope gain-staging guidance.)
4. **Low end.** High-pass anything that does not need sub. Keep kick and bass from occupying the same moment or the same tone; consider mono below ~120 Hz. Listen for rumble, not just "more bass."
5. **Subtractive EQ first.** Cut mud and resonances before boosting "air." Carve a pocket for the vocal instead of piling brightness on everything. (Standard practice; iZotope subtractive-EQ guidance.)
6. **Balance before effects.** Scheps’s point: impact often comes from balance (and parallel punch), not a pile of reverbs.
7. **Parallel compression.** Blend a harder-compressed drum (or vocal) bus under the dry transients. Do not replace the dry kit.
8. **Vocal.** De-ess, compress so the lead stays audible in the chorus, effects on *sends*. Short dark delays usually sit better than bright slaps. Longer halls only where the section should bloom, then ride them down.
9. **Width.** Hard-panned sides, solid center. Check mono compatibility. Do not widen the sub.
10. **Saturation / bus glue.** Gentle tape or console color, modest mix-bus compression. CLA’s caution: a limiter on the 2-bus can flatten drums — be careful.
11. **Automation.** Section contrast: mute or drop instruments under important lines (Hugo/Pensado instinct); open width and effects in the hook; subtract for the turn.
12. **Mastering targets (streaming, current official / widely documented):**
    - **Spotify** normalizes to **−14 LUFS** (ITU-R BS.1770) on the Normal setting (Loud −11, Quiet −19). Spotify’s mastering tips: target about **−14 LUFS integrated**, true peak **below −1 dBTP**; if the master is *louder* than −14 LUFS, keep true peak **below −2 dBTP** to reduce codec distortion. Louder masters are turned down; they do not play back louder, they just sound denser.
    - **Apple Music (Sound Check)** is commonly documented around **−16 LUFS**; YouTube / many others around **−14**. Confirm if a platform is the primary destination.
    - Prioritize dynamics and punch over winning a loudness war. Katz and Grundman both treat mastering as serving the music’s impact and translation, not just making it louder. Grundman’s job, in his terms: optimize so it works on many systems, enhance what is already strong, stay with the emotion of the record.
13. **Print.** True-peak limiter at the ceiling above. Bounce WAV. Listen on headphones, small speakers, and a phone. If it only works slammed into the limiter, fix the mix.

## Working loop

1. Pick one lens and one emotional tension.
2. Write the style block (short, concrete, contrast included).
3. Write lyrics with matching metatags; hook first.
4. Generate two or more takes (Suno: consider v6 for a tight brief, v6-wild to explore, then refine on v6). Style Influence up, Variety at 0 when the prompt is deliberate.
5. Keep the take with the best performance, not the busiest arrangement.
6. Cover / Remaster / section edit, or pull stems and finish in the DAW.
7. Change one variable per iteration.

## Sources

Primary and official sources are listed in `research-notes.md` beside this skill. Prefer those over recycled "Suno god prompt" blogs. When a claim is only community-reported, say so.
