# Song index

Every song made with this skill, so we can always show how a song was made: the prompt it started from, what came out, what it cost, and what was done to it afterwards.

One row per generation. The full record (style prompt, lyrics, Exclude list, settings, every clip with link, length, tempo and key, scores, pick, credits, post-production) lives in the generation file linked from each row.

## Index

| Song / working title | Gen | Date | Model(s) | Clips | Credits used | Pick | Post-production | Record |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| WaveWarZ, the electric vibez (v2) | Zaal 1 | 25 Nov 2026 | v6, v6-wild | 4 | 20 | Pending | Not started | [gen-001](../generations/zaal/gen-001-electric-vibez-v2/) |

## Credit ledger (Suno)

Running balance, one line per generation. Read credits with Suno's account usage right before the first call and right after the last.

| Gen | Before | After | Used | Notes |
| --- | --- | --- | --- | --- |
| Zaal 1 | 10,000 | 9,980 | 20 | 2 calls x 2 clips, 5 credits per clip. Listening and analysis free. |

## Adding a song

1. Create `generations/<creator>/gen-NNN-<slug>/README.md` from the sections in [`generations/README.md`](../generations/README.md).
2. Read the credit balance before generating; log it.
3. Generate, score each clip, read the balance again.
4. Add a row to both tables above.
5. When the pick is made and post-production starts, update the Pick and Post-production columns and log each step in the generation file (see [`POST-GEN.md`](../POST-GEN.md)).
