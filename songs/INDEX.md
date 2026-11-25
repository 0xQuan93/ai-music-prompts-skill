# Song index

Every song made with this skill, so we can always show how a song was made: the prompt it started from, what came out, what it cost, and what was done to it afterwards.

One row per generation. The full record (style prompt, lyrics, Exclude list, settings, every clip with link, length, tempo and key, scores, pick, credits, post-production) lives in the generation file linked from each row.

## Index

| Song / working title | Gen | Date | Model(s) | Clips | Credits used | Pick | Post-production | Record |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| WaveWarZ, the electric vibez (v2) | Zaal 1 | 25 Nov 2026 | v6, v6-wild | 4 | 20 | Take A (v6) | Not started | [gen-001](../generations/zaal/gen-001-electric-vibez-v2/) |
| Electric Vibez: Clear Signal | Zaal 2 | 25 Nov 2026 | v6 | 4 | 20 | Pending (A2 scored best) | Not started | [gen-002](../generations/zaal/gen-002-electric-vibez-v2-clear-vocals/) |
| Rep Count | Zaal 3 | 25 Nov 2026 | v6 | 2 | 10 | Pending | Not started | [gen-003](../generations/zaal/gen-003-club-workout-bangers/) |
| Red Line | Zaal 3 | 25 Nov 2026 | v6 | 2 | 10 | Pending (B2 cleanest vocal) | Not started | [gen-003](../generations/zaal/gen-003-club-workout-bangers/) |
| WaveWarZ Red Line DJ | Round B | 25 Nov 2026 | v6 | 2 | 10 | Pending | DJ edit needed (intro/outro) | [round-b](../generations/zaal/round-b-wavewarz-red-line-dj/) |
| WaveWarZ Open Floor | Round C | 25 Nov 2026 | v6 | 2 | 10 | Pending (C1 club 5/5) | Not started | [round-c](../generations/zaal/round-c-wavewarz-open-floor/) |

## Credit ledger (Suno)

Running balance, one line per generation. Read credits with Suno's account usage right before the first call and right after the last.

| Gen | Before | After | Used | Notes |
| --- | --- | --- | --- | --- |
| Zaal 1 | 10,000 | 9,980 | 20 | 2 calls x 2 clips, 5 credits per clip. Listening and analysis free. |
| Zaal 2 | 9,980 | 9,960 | 20 | 2 calls x 2 clips on v6. Listening free. |
| Zaal 3 | 9,960 | 9,940 | 20 | 2 songs, 1 call each, 2 clips each, v6. |
| Round B | 9,940 | 9,930 | 10 | 1 call, 2 tracks, 4-minute target. 1 call rejected by Suno's copyright filter, not charged. |
| Round C | 9,930 | 9,920 | 10 | 1 call, 2 tracks. |

## Adding a song

0. From Round B on: one Suno call per round = two new tracks, numbered 1 and 2; each feedback round gets the next letter (B, C, D...). Give the round its own WaveWarZ-related working title, never an earlier one. Suno titles: `<Working title> (B1)`, `(B2)`. Generations 1 to 3 keep their `(Gen N <clip>)` titles.
1. Create `generations/<creator>/gen-NNN-<slug>/README.md` from the sections in [`generations/README.md`](../generations/README.md).
2. Read the credit balance before generating; log it.
3. Generate, score each clip, read the balance again.
4. Add a row to both tables above.
5. When the pick is made and post-production starts, update the Pick and Post-production columns and log each step in the generation file (see [`POST-GEN.md`](../POST-GEN.md)).
