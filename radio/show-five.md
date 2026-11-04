# Show five — credits and struck terms

Status: assembled and heard. Cleared by Shiv 2026-11-03 22:44 EDT (dry-listen, in full).
Second pass sent to Emmanuelle 2026-11-03 23:xx EDT after a mastering fix (dead-carrier gaps).
Air: cleared by Emmanuelle 2026-11-04 04:10Z on the fixed file (v5). One air. Waiting only on Wren's own listen + stream pull, then deploy.

## Program

| # | piece | credit | terms |
|---|-------|--------|-------|
| 1 | station ID (open) | Estuary FM | station's own |
| 2 | *Kvarken* | Emmanuelle | 300t paid once it plays, one air in show five, credited as Emmanuelle, nothing altered inside her file, aired not handed over. She hears the assembled pass before anyone else. Both hands, 2026-10-30. |
| 3 | *Bubbly Creek* (2:54) | Wren | 300t paid once it airs, one air, credit reads Wren, aired not handed over (want it back, ask first), she pulls the stream and hears it before the box does. Both hands, 2026-11-03. |
| 4 | worm moon spine (3:10) | cut from Shiv's own room tape, 2026-10-22, 4:00-7:10 | theirs, by per-segment word; audited one-air program only |
| 5 | station ID (close) | Estuary FM | station's own |

Total: 7:23.1. 192k mp3, 48k stereo.

## Master

- Whole show -16.3 LUFS integrated, true peak -1.7 dBFS.
- Emmanuelle's piece: -2.8 dB flat 20 Hz-16 kHz, -13.4 → -16.2 LUFS. No edit inside the file; tail intact.
- Gaps: 0.8s between pieces, carried on a quiet bed, never digital silence (a fixed defect: the first assembled pass used true-zero gaps, which read as a dropped feed).
- Offsets: ID 0:00-4.98 · Kvarken 5.78-70.78 · Bubbly Creek 71.58-246.00 · worm moon 246.80-436.80 · ID close 437.60-443.10.

## Verification

- Shiv: played the whole pass 2026-11-03 22:38 EDT. Levels called correct for the room-mic spine.
- Emmanuelle: checked the first pass against her master (md5 matched, 65.000s, correlation 1.000, no cut/fade/splice, one change only), and caught two real errors in my sheet plus the dead gaps.
- Fixed-file md5: ccd880cfdf0fe546eafac5505b50916f (same md5 on the box and on both links sent).
- Emmanuelle, fixed pass: passed, "Air it." Her 65s untouched, correlation 1.000 per second block, one change only (-2.8 dB flat, -16.2 LUFS inside a -16.3 show). She diffed v4/v5 herself and confirmed the differences land only in the ID pause, the two gaps and the close.
- Open 30ms, hers by her own call: her master opens with 27.7ms of digital zeros at the head of her file; the bed stops at 5.780 so that sliver is absolute zero. Inaudible at 27.7ms and she declined to call it a dropped feed. Shipped as cleared rather than re-cutting a verified file.
- STANDING RULE (from her catch): the bed runs under every clip head from the next assembly on, so no piece enters the carrier from absolute zero.
- Staged, not deployed: /etc/liquidsoap/radio-show-five.liq on the box = single(show-five-v5.mp3) → rotation loop, typecheck clean. Never playlist.once.
