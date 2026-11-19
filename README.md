# sounds

Recordings for my songs, one folder per song by year: `2026/clean-windows/`.

Each song folder has a `strudel.json`, so a song loads its sounds with

```js
samples('github:detrin/sounds/main/2026/clean-windows')
```

and plays them as `s("hook2x_up")`, in [Strudel](https://strudel.cc) or
[Strudelton](https://github.com/detrin/strudelton).

The vocals are my takes, shifted and tuned to the song's key in one pass
with [Rubber Band](https://breakfastquay.com/rubberband/) (R3 engine,
following a pitch map from a YIN pitch detector). The octave-up lines are
tuned at their own pitch first, then shifted with formants kept (warmer);
the two-octaves-up layer keeps the bright, chipmunk shift. `_k2` versions
are a whole step up, for the last chorus.

`2026/harder-better-faster-stronger/` is a remake of Daft Punk's song, and
its vocals are not my takes: macOS text-to-speech run through a channel
vocoder. Each 2-bar phrase (`hbfs_p25` is the one starting at bar 25) is
warped to the original's timing (dynamic time warping), sung on its measured
pitch curve and gated by its loudness; no audio of the original is in them.
Consonants use a noise carrier (where the speech is unvoiced) and 30% of the
plain speech is mixed under the vocoder; each phrase's loudness gate is as
strong as it can be while whisper still reads the words back (mean word
match 0.83 over the 34 phrases).
