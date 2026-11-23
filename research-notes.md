# AI music prompts — research notes

Sources and verification notes for the skill in this repo. Compiled 22 Nov 2026.

## Highest-value findings

1. **Suno is on v6 as of 9 Sep 2026.** Official blog and help: v6 / v6-wild / v6-mini; previous models retired; up to 8 minutes per generation; Max Mode for long/consistent work; Variety slider at 0 to stop style-prompt rewriting. Sources: [Introducing v6](https://suno.com/blog/introducing-v6), [v6 FAQ](https://help.suno.com/en/articles/13924481), [How long will my song be?](https://help.suno.com/en/articles/13924929).
2. **Split Style vs Lyrics.** Style = sound. Lyrics = words + metatags on their own lines. Official Suno llms.txt (updated 29 May 2026, still useful on capabilities; model numbers have since moved to v6): Custom mode uses Style of Music + lyrics; latest models take rich conversational prompts. [suno.com/llms.txt](https://suno.com/llms.txt).
3. **Real Suno controls, not folklore:** Exclude ([help](https://help.suno.com/en/articles/3161921)); Weirdness / Style Influence sliders ([help](https://help.suno.com/en/articles/6141377)); Cover keeps melody, restyles *your* song ([help](https://help.suno.com/en/articles/2872257)); Remaster is a subtler mix/character pass, Subtle/Normal/High, not a lyric rewrite ([help](https://help.suno.com/en/articles/8105281)); Personas/Voices capture vibe for reuse ([help](https://help.suno.com/en/articles/3484161)); stems/WAV/MIDI and Studio on paid plans ([llms.txt](https://suno.com/llms.txt)). Character-limit numbers (Style ~1000, Exclude ~200) are **community-reported**, not published in the official help pages checked.
4. **Udio official prompt recipe** is short and specific: topic + tags; repeat to emphasize; era and scene prompts; Style Reduction as the negative channel; Manual Mode for exact tags; `in the style of` = feel, not voice clone. [Prompt Like a Master](https://help.udio.com/en/articles/10716541-prompt-like-a-master). Style Reduction was also announced by Udio staff on Reddit (2 Oct 2024) as similar to negative prompting.
5. **Rubin is a reducer.** “Least amount of information possible”; less is more but you have to do more to get less; walls of doubled guitars hide the player; credit “Reduced by” because production sounded like building up. Sources: [CBS 60 Minutes interview](https://www.cbsnews.com/news/rick-rubin-60-minutes-transcript-2023-05-28/), [MasterClass / “Finding Your Life’s Work” remarks](https://www.youtube.com/watch?v=g6MEDOY7tHo), [Complex interview on The Creative Act](https://www.complex.com/music/a/eric-skelton/rick-rubin-interview-the-creative-act), [Tim Ferriss interview](https://tim.blog/2023/01/16/rick-rubin-2-transcript/).
6. **Neptunes signatures are well documented in first-person interviews:** minimalism and sparseness (Pharrell, NPR, including the “spray paint” hiss on “Drop It Like It’s Hot”); “skeleton songs,” silence pockets, sometimes no bass ([The Age / interview feature](https://www.theage.com.au/entertainment/music/like-the-song-these-guys-wrote-it-20040515-gdxu7b.html)); Chad Hugo on quantizing kicks/snares but not hats, muting under vocals, hard-hitting drums, Tritons/presets, gate reverb on the “Grindin’” hook (Chad Hugo “Behind the Beats” interview, circulated from *Sound & Recording* / DOI — treat gear anecdotes as interview-true, not as a required toolkit). Secondary craft writeups (e.g. RouteNote producer profile) add short pitched snares and dry mixes; mark those as secondary.
7. **Elite mixers agree on song-first, and disagree on “magic chains.”** Ghenea: no bag of tricks; maximize what emotionally carries the song ([Waves interview](https://www.waves.com/waves-grammys-2021-serban-ghenea-taylor-swift)). CLA: LCR guitars vs centered vocal/rhythm; compress vocal into the guitars’ dynamic range; don’t judge in solo; simple mix bus, careful with 2-bus limiting ([Production Expert / Waves ITB walkthrough notes](https://www.production-expert.com/production-expert-1/get-top-chris-lord-alge-mixing-tips); [SOS, Welcome to the Black Parade](https://www.soundonsound.com/techniques/secrets-mix-engineers-chris-lord-alge) for section-dependent reverbs). Scheps: learn every part, parallel compression, few effects, balance makes rock explode ([ProSoundWeb / Owsinski](https://www.prosoundweb.com/in-the-studio-an-interview-with-noted-mix-engineer-andrew-scheps/)). Pensado: first impressions, effects on sends, dark vocal delays ([SOS](https://www.soundonsound.com/techniques/secrets-mix-engineers-david-pensado)). Marroquin: structure and emotional connection; today’s mix often anticipates the master ([Tape Op](https://tapeop.com/interviews/109/manny-marroquin-bonus)).
8. **Streaming loudness is normalization, not “louder wins.”** Spotify official: playback target **−14 LUFS** (ITU 1770) on Normal; tips = master around −14 integrated, **< −1 dBTP**, or **< −2 dBTP** if louder than −14. Louder masters are turned down. [Spotify for Artists](https://support.spotify.com/us/artists/article/loudness-normalization/). Apple Music is widely documented near **−16 LUFS** (e.g. [iZotope](https://www.izotope.com/community/blog/mastering-for-streaming-platforms)); always re-check the platform. AES TD1008 discusses internet-stream true peak and music-service targets.
9. **Mastering philosophy vs numbers.** Katz argued for normalization and preserved dynamics (Tape Op #116; some *platform figures in that older interview are outdated* — use current official docs for LUFS). Grundman: post-production to optimize translation to many systems; enhance what’s already strong rather than overhaul it; stay with the emotion while working ([RBMA masterclass](https://daily.redbullmusicacademy.com/2017/10/bernie-grundman-mastering-masterclass/)).
10. **Translate techniques into audible descriptors; finish in a DAW.** Models respond to “dry close vocal,” “pockets of silence,” “drumless bridge,” not to “1176 at 4:1” or “−14 LUFS.” Standard DAW practice still applies after export: gain staging ([iZotope](https://www.izotope.com/community/blog/gain-staging-what-it-is-and-how-to-do-it)), subtractive EQ ([iZotope](https://www.izotope.com/community/blog/7-tips-for-using-subtractive-eq-when-mixing-audio)), parallel compression, send-based FX, mono-checked low end.

## Verified vs folklore

| Claim | Status |
| --- | --- |
| Suno Style vs Lyrics split; Exclude; sliders; Cover / Remaster / Personas; v6 length 8 min | Official help / blog |
| Style ~1000 chars, Exclude ~200, “8–15 tags,” order-weighting | Community / third-party guides; not in official help checked |
| Metatags as hard switches or guaranteed key changes | Folklore; treat as biases |
| Udio Style Reduction, repeat-to-emphasize, era/scene, no voice clone | Official Udio help |
| Rubin reducer / least information / singular performances | Primary interviews |
| Neptunes minimal, silence, spray-paint hiss, hat swing, mute-for-vocal | Primary interviews |
| Exact “Neptunes snare pitch + no reverb recipe” | Partly secondary craft writing |
| Ghenea fixed vocal chain | Folklore; he denies a bag of tricks. Plugin lists online are reconstructions |
| CLA LCR + vocal dynamics vs guitars | Strong (walkthrough quotes) |
| Spotify −14 LUFS / −1 dBTP (−2 if louder) | Official |
| “Master as hot as possible for streaming” | False under normalization |
| Prompting a LUFS number into Suno/Udio | Ineffective; do it in the DAW |

## Sources

### Official platform

- https://suno.com/blog/introducing-v6
- https://help.suno.com/en/articles/13924481 (v6 FAQ)
- https://help.suno.com/en/articles/13924929 (song length)
- https://help.suno.com/en/articles/3161921 (Exclude)
- https://help.suno.com/en/articles/6141377 (Creative sliders)
- https://help.suno.com/en/articles/2872257 (Cover)
- https://help.suno.com/en/articles/8105281 (Remaster)
- https://help.suno.com/en/articles/3484161 (Personas)
- https://suno.com/llms.txt (capabilities; dated 29 May 2026)
- https://suno.com/release-notes/introducing-v5-the-world-s-best-music-model
- https://about.suno.com/blog/introducing-v4-5 (v4.5 announcement)
- https://help.udio.com/en/articles/10716541-prompt-like-a-master
- https://support.spotify.com/us/artists/article/loudness-normalization/

### Producers / engineers

- https://www.cbsnews.com/news/rick-rubin-60-minutes-transcript-2023-05-28/
- https://www.complex.com/music/a/eric-skelton/rick-rubin-interview-the-creative-act
- https://tim.blog/2023/01/16/rick-rubin-2-transcript/
- https://www.npr.org/sections/therecord/2013/12/31/258406317/pharrell-williams-on-juxtaposition-and-seeing-sounds
- https://www.theage.com.au/entertainment/music/like-the-song-these-guys-wrote-it-20040515-gdxu7b.html
- https://community.livejournal.com/-pharrell/16085.html (Chad Hugo interview reprint; use cautiously, prefer locating the original *Sound & Recording* feature if tightening citations)
- https://www.waves.com/waves-grammys-2021-serban-ghenea-taylor-swift
- https://www.production-expert.com/production-expert-1/get-top-chris-lord-alge-mixing-tips
- https://www.soundonsound.com/techniques/secrets-mix-engineers-chris-lord-alge
- https://www.soundonsound.com/techniques/secrets-mix-engineers-david-pensado
- https://www.prosoundweb.com/in-the-studio-an-interview-with-noted-mix-engineer-andrew-scheps/
- https://tapeop.com/interviews/109/manny-marroquin-bonus
- https://tapeop.com/interviews/116/bob-katz-bonus
- https://daily.redbullmusicacademy.com/2017/10/bernie-grundman-mastering-masterclass/

### Mix / master practice

- https://www.izotope.com/community/blog/gain-staging-what-it-is-and-how-to-do-it
- https://www.izotope.com/community/blog/7-tips-for-using-subtractive-eq-when-mixing-audio
- https://www.izotope.com/community/blog/mastering-for-streaming-platforms
- https://aes.org/wp-content/uploads/2026/10/20210924_TD1008_v3.13.pdf (AES TD1008 loudness for streaming)

### Community / secondary (useful, labeled as such)

- https://blakecrosley.com/guides/suno (metatag catalogs, descriptor-count rules)
- https://www.tonedraft.com/en/blog/suno-ai-prompt-guide-2026 (character limits, tag-count “sweet spot”)
- https://create.routenote.com/blog/producer-profile-pharrell-williams/ (Neptunes craft profile)
- https://www.reddit.com/r/udiomusic/comments/1fupzja/new_feature_style_reduction_tell_udio_that_you/ (Udio staff Style Reduction announcement)
