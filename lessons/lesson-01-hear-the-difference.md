# Lesson 1 - Hear the difference

Learn production by comparing songs we already made. Each comparison: play clip X at the time given, then clip Y, listen for one thing, learn the word for it, see which prompt words caused it.

Timestamps come from Suno's listening model and are approximate (within a second or two). Use headphones first, then a phone speaker.

## 1. Kick patterns: four-on-the-floor vs Jersey club

- **Play:** [Rep Count A1](https://suno.com/song/6fcad18d-fab4-4c65-9ab7-a45d93a54da3) at **0:30**, then [Red Line B2](https://suno.com/song/7ede338a-0e6f-43a0-9bc2-7337f460931c) from **1:00 to 1:15**.
- **Listen for:** Rep Count's kick lands on every beat, 1-2-3-4, like a metronome. Around 1:10 Red Line's kick stops marching and starts stuttering in quick groups of three.
- **Words:**
  - *Four-on-the-floor*: a kick on every beat. House and techno run on it.
  - *Triplet*: three hits in the space of two.
  - *Syncopation*: hits that land between the beats. The Jersey club "bounce" is syncopated triplet kicks.
- **How we got it:** "driving four-on-the-floor kick" (Rep Count) and "switching to Jersey club triplet kick bounce on the drops" (Red Line).
- **Why it matters:** four-on-the-floor is steady, so you can run or lift to it. The triplet bounce is jumpy, so it hits hardest as a surprise on a drop.

## 2. Tempo: 128 vs 140 BPM

- **Play:** Rep Count A1 at 0:30, then Red Line B2 at 0:15. Tap your foot to each.
- **Listen for:** 128 feels like a fast jog. 140 feels urgent, closer to sprint intervals.
- **Word:** *BPM* (beats per minute). House sits around 120 to 130. Jersey club, bass house and hard dance sit around 135 to 150.
- **How we got it:** the BPM number in the first line of the style prompt. Suno hit it within 2 BPM on every clip so far.
- **Why it matters:** in a set, DJs move between tracks at close tempos, so a 128 track and a 140 track don't blend without a tempo change or a cut.

## 3. Space: lots of vocal vs few vocals

- **Play:** [Gen 1 A1](https://suno.com/song/c32c4845-f6e5-4068-9de3-52857ece7ccb) from **0:00 to 0:35**, then [Gen 2 A2](https://suno.com/song/db524c7b-4e88-4fbe-9b4e-4a3a8d8e4d03) from **0:46 to 1:12**.
- **Listen for:** Gen 1 has a voice almost all the time. In Gen 2 A2's bridge the drums drop out and the track breathes; when the voice is there, it has room.
- **Words:**
  - *Arrangement*: what plays when.
  - *Subtraction*: making a part hit harder by taking things away around it (the skill's "Rubin reducer" lens).
  - *Breakdown*: a section with the drums out.
- **How we got it:** a full lyric in Gen 1 vs a 7-line lyric plus `[Instrumental Break]` and `[Bridge: no drums]` tags in Gen 2. Gen 2 A2 measured about 38% vocals (Gen 1's share wasn't measured, but its vocal starts at 0:00 and runs through every verse).
- **Why it matters:** in a club the groove carries the track. Fewer, clearer vocal moments make each one land.

## 4. Tension: the cut before the drop

- **Play:** Rep Count A1 from **0:23 to 0:32**, then Red Line B2 from **1:29 to 1:46**.
- **Listen for:** Rep Count's snare roll builds, the drums cut for a beat at 0:29, and the drop slams in at 0:30. Red Line goes almost silent at 1:42 before the final drop at 1:44.
- **Words:**
  - *Build*: rising energy, from snare rolls, risers or filters opening.
  - *Drop*: where the full beat and bass come back.
  - *Drum cut*: removing the drums for a moment so their return hits harder.
- **How we got it:** "drums cut for one bar, then a heavy drop" and "one bar of silence before the final drop", mirrored by `[Build]` and `[Break: one bar of silence]` tags.
- **Why it matters:** the silence is what makes the drop feel big. Loudness alone doesn't.

## 5. DJ-friendly intro and outro

- **Play:** the first 20 seconds and last 40 seconds of Rep Count A1 (outro starts around **1:46**), then the same on Red Line B2 (vocal at **0:00**, cuts off at **2:06**).
- **Listen for:** Rep Count starts with just the beat and strips back down at the end, which gives a DJ a window to blend. Red Line starts on a vocal and ends suddenly, so there is no clean beat to mix over.
- **Words:**
  - *Mix-in / mix-out*: the beat-only stretch a DJ overlaps with the previous or next track.
  - *Phrase*: club tracks move in blocks of 8, 16 or 32 bars, and DJs mix on those blocks.
- **How we got it:** both prompts asked for an instrumental intro and outro. Rep Count's longer total length (2:38 vs 2:06) left room for it. Red Line's didn't.
- **Fix next time:** "long DJ-friendly intro and outro, 16 bars of drums only", or set a 4-minute duration.

## 6. Center vs wide, dry vs wet

- **Play:** any clip on headphones, then on one phone speaker.
- **Listen for:**
  - **Center vs wide:** the kick, bass and lead vocal stay in the middle and survive on a phone. Claps, hats, effects and vocal chops spread wide and get quieter in mono.
  - **Dry vs wet:** Gen 1 A1's lead is fairly dry (close, little echo). Gen 2 A2's bridge vocal is wet (medium-to-high reverb), even though we asked for "raw close vocal".
- **Words:**
  - *Stereo width / panning*: where a sound sits left to right.
  - *Mono*: one speaker. Club systems often run the low end in mono.
  - *Dry / wet*: without or with reverb and delay.
- **Why it matters:** keep the kick and bass centered so they stay strong on any system. Too much reverb and pitch processing on a voice is a big part of why it "sounds AI".

## What the prompts taught us (so far)

| We asked for | We got | Lesson |
| --- | --- | --- |
| "vocal chops" in Exclude (Gen 3) | Chops still appeared on Rep Count | Exclude reduces, it doesn't forbid |
| "raw close vocal" on the bridge (Gen 2) | Reverb on every bridge | The model adds space to exposed vocals; plan to dry them in post |
| BPM in the first line | Within 2 BPM every time | Tempo is the most reliable control |
| Short lyric + instrumental tags | 23 to 65% vocals | Short lyrics help; shortest (Red Line) worked best |

## Homework (5 minutes)

1. Clap along to Red Line B2 and mark the second where the kick changes pattern.
2. On Rep Count A1, count the bars from 0:00 until the first drop (count "1-2-3-4" per bar).
3. Pick one clip and decide: what would you remove to make the vocal hit harder?

Send the answers back and Lesson 2 builds on them: EQ and why some sounds fight each other.
