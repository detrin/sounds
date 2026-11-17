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
