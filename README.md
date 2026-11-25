# AI music prompts skill

An agent skill for writing prompts for [Suno](https://suno.com) (v6 family; retired v4/v5 notes included) and [Udio](https://udio.com), with producer and mix-engineer “lenses” folded into style language: Rick Rubin (reduction), Pharrell / The Neptunes (sparse bounce), and elite mix/master approaches from people like Serban Ghenea, Chris Lord-Alge, Andrew Scheps, Dave Pensado, Manny Marroquin, Bob Katz, and Bernie Grundman.

**by 0xQuan (Quantum X) · WaveWarZ**

- X: [@_0xQuan](https://x.com/_0xQuan)
- [poselab.studio](https://poselab.studio)

## Who it's for

Producers, songwriters, and anyone using an AI music generator who wants prompts that describe a *record* — groove, vocal character, arrangement contrast, and production feel — instead of a pile of “hit song, radio ready” adjectives. Also useful after generation, when you pull a WAV or stems into a DAW and need a short mix/master checklist for streaming.

## How to use it

**As a skill (Claude, Cursor, and similar agent skill folders):**

1. Copy this repo (or just the folder that contains `SKILL.md`).
2. Drop it into your agent’s skills directory. Typical locations:
   - Claude Code: `.claude/skills/ai-music-prompts/` (project) or `~/.claude/skills/ai-music-prompts/` (user)
   - Cursor / other SKILL.md-compatible agents: the project or user skills folder your tool documents
3. The agent should pick it up when you ask for a Suno or Udio prompt, a producer-style lens, or a finishing checklist. You can also invoke it by name.

**As a system prompt (any LLM):**

Open `SKILL.md` and paste the body into the system prompt (or as the first message) before you ask for a track. Keep `research-notes.md` handy if you want source citations.

Then ask for a style block, lyrics with metatags, an Exclude / Style Reduction list, or a DAW finish pass.

## Quick example

**Style of Music**

```text
Minimal futuristic funk-hop, 98 BPM. Skeleton beat, pockets of dead silence.
Tight quantized kick and snare, swung hats, short pitched-up snare, sustained kick.
Sparse syncopated clav stabs, one odd spray-paint hiss and a tiny sci-fi blip.
Dry, almost no reverb, punchy and close. Playful masculine hook, rhythmic verses.
Leave space; mute the stabs under the vocal.
```

**Exclude / Style Reduction:** trap 808 glides, crowded sample loops, long hall reverb, orchestral layers

More complete examples — including a WaveWarZ battle-style track and a dark atmospheric trap prompt — live in `SKILL.md` and `examples/dark-trap.md`.

## Suno v6 notes (as of September 2026)

- New generations run on the **v6 family**: **v6** (precise/polished, Pro/Premier), **v6-wild** (more varied, Pro/Premier), **v6-mini** (faster, all plans). Prior models are retired; library tracks still play, remaster, and cover, but new iterations use v6.
- Generations can run up to **8 minutes**; use **Extend** for more. **Max Mode** costs extra credits and helps with longer songs, tight covers, and vocal/style consistency.
- Set the **Variety** slider to **0** if you need the style text followed closely (Variety rewrites style prompts to add variation).
- Put sound in **Style of Music** and lyrics plus `[Verse]` / `[Chorus]` (etc.) metatags in **Lyrics**. Use **Exclude** for instruments or colors you do not want. Raise **Style Influence** when the style block is deliberate.
- **Cover** restyles a song you created while keeping the melody. **Remaster** is a subtler mix/character pass, not a lyric rewrite. Pull **stems / WAV** into a DAW for release levels — prompting a LUFS number into the generator does not replace mastering.

Platform features change. Prefer official help pages linked in `research-notes.md` over recycled “god prompt” blogs. Claims that are only community-reported are labeled as such in the skill.

## What’s in this repo

- `SKILL.md` — the skill (when to use, prompt template, producer lenses, mix vocabulary, metatag cheat sheet, example prompts, DAW checklist)
- `research-notes.md` — sources and a verified-vs-folklore table
- `examples/dark-trap.md` — a complete dark atmospheric trap prompt
- `generations/` - a log of real tracks made with the skill: exact inputs, settings, takes, and lessons (starting with Zaal's Generation 1)
- `songs/INDEX.md` - song index and Suno credit ledger: how every song was made, what it cost, what was done after
- `research/music-basics.md` - the building blocks of a track, house and Jersey club basics, and how each maps to Suno prompt words
- `lessons/` - learn production by comparing our own generations, with timestamps
- `POST-GEN.md` - draft checklist for turning a generated clip into a finished song
- `LICENSE` — MIT

## License

MIT © 2026 0xQuan
