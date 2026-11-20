# Sustain Six riff and lick loops (set 2)

Audio for the Riffs and Licks pages of Sustain Six (https://sustainsix.com), served through jsDelivr.
The app asks for these files at one exact commit:
`https://cdn.jsdelivr.net/gh/macosta/fret-legend-riffs-2@<commit>/<version>/<file>`.

This repo holds 8 of the 16 riffs and licks first published in `macosta/fret-legend-samples/riffs/` (2026-11-01).
They were copied here, byte for byte, on 2026-11-20. jsDelivr refuses a GitHub repo over 50 MB, that repo is over it,
and so about a third of first requests for these files were refused. The copies in the old repo stay where they are:
the store apps already shipped still ask for them there.

- `chug_e`: Chug in E
- `lick_a_minor`: Lick in A minor
- `lick_e_minor`: Lick in E minor
- `rock_a`: Rock in A
- `boogie_a`: Boogie in A
- `drive_d`: Drive in D
- `lick_a_pent`: Pentatonic Bend in A
- `lick_a_major`: Major Pentatonic in A

## Rules

- **Keep this repo under 40 MB in total.** The jsDelivr limit is 50 MB for the whole repo at the commit asked for.
  A new riff goes to a repo with room, never here once this one is near 40 MB.
- **Never rewrite history.** The app names a commit; a rewritten commit is a dead address.
- **Never overwrite a published file name.** New audio gets a new version folder.

## Files

`<version>/<item>_<preset>_<speed>_<version>.flac`: one riff or lick, rendered alone at that percent of its tempo,
16-bit stereo 44.1 kHz FLAC (lossless, so the length is sample-exact). Each file is EXACTLY one loop long; ring-out
and effects tails are folded onto the head, so it loops seamlessly. Rendered by `scripts/tone/render_library.py`
in the app repo, which also writes the app's `scripts/tone/riffs/manifest.json`.

## Attribution and licences

See [CREDITS.md](CREDITS.md).
