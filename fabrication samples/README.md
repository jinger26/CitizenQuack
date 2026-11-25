# Fabrication samples — material tests

Part of the **Maker Faire Shenzhen 2026 version**. The goal is to compare three
filaments for the duck shell, as input to the open decision on shell materials
(see the main [README](../README.md#maker-faire-shenzhen-2026-version)).

Started 2026-11-25. Status: **printing**. Photos and results to follow.

## Progress log

| Date | Material | Update |
|---|---|---|
| 2026-11-25 | TPU | Printing the head and body together on the Prusa MK4S. Video: [`printingonprusa20261125.mp4`](printingonprusa20261125.mp4) |
| | PLA Silk | Not yet printed |
| | PETG | Not yet printed |

## What is being printed

Miriam Choi's Duck Options, 2 mm hollow version
([`cad/miriam-duck-options/`](../cad/miriam-duck-options/)):

- `Mduck_head_2mmhollow.stl` (90.6 × 69.1 × 40.8 mm)
- `Mduck_bod_2mmhollow.stl` (93.5 × 83.3 × 36.0 mm)

Each G-code file prints **both the head and the body on one plate**, even though
the file name starts with `Mduck_bod`. The parts were printed lying flat, as exported
(tallest part 40.8 mm).

## Printer and slicer

| | |
|---|---|
| Printer | Original Prusa MK4S, 0.4 mm HF nozzle |
| Slicer | PrusaSlicer 2.9.6 |
| Print profile | 0.20mm SPEED @MK4S HF0.4 (same for all three) |
| Layer height | 0.2 mm |
| Perimeters | 2 |
| Top / bottom solid layers | 5 / 3 |
| Infill | 15 % grid |
| Seam | aligned |
| Brim | none |
| G-code format | binary G-code (`.bgcode`) |

## The three samples

| | TPU | PLA Silk | PETG |
|---|---|---|---|
| G-code | [`…_FLEX_MK4S_5h3m.bgcode`](Mduck_bod_2mmhollow_0.4n_0.2mm_FLEX_MK4S_5h3m.bgcode) | [`…_PLA_MK4S_2h18m.bgcode`](Mduck_bod_2mmhollow_0.4n_0.2mm_PLA_MK4S_2h18m.bgcode) | [`…_PETG_MK4S_1h35m.bgcode`](Mduck_bod_2mmhollow_0.4n_0.2mm_PETG_MK4S_1h35m.bgcode) |
| Filament profile | Prusament TPU 95A @MK4S | Generic PLA Silk @MK4S | Generic PETG @MK4S HF0.4 |
| Nozzle temp (first layer / rest) | 230 / 230 °C | 230 / 225 °C | 250 / 250 °C |
| Bed temp (first layer / rest) | 65 / 65 °C | 60 / 60 °C | 85 / 90 °C |
| Supports | **none** | yes (painted/enforced, not auto) | yes (painted/enforced, not auto) |
| Estimated time (normal / silent) | 5 h 3 m / 5 h 8 m | 2 h 18 m / 2 h 25 m | 1 h 35 m / 1 h 51 m |
| Filament used | 57.2 g (19.3 m) | 52.5 g (17.6 m) | 53.7 g (17.6 m) |
| Slicer cost estimate | 4.46 | 1.33 | 1.49 |
| Actual print time | _tbd_ | _tbd_ | _tbd_ |

Notes from the slicer settings:
- TPU is about 2–3× slower than PLA or PETG with the same print profile, because
  flexible filament has to be fed slowly.
- TPU was sliced **without supports**, while PLA Silk and PETG use supports that were
  placed by hand (supports on, auto-generation off). Overhangs on the TPU duck may
  show this.
- The slicer cost uses the price set in each filament profile, not what we paid.

## Process

1. Downloaded Miriam's Duck Options zip (see main README, Resources) and kept the
   2 mm hollow head and body, which leave room for electronics.
2. Opened both STLs together in PrusaSlicer 2.9.6 with the MK4S HF0.4 printer profile.
3. Used the same print profile (0.20mm SPEED) for all three, changing only the
   filament profile, so the results compare materials rather than settings.
4. Added supports by hand for PLA Silk and PETG; none for TPU.
5. Exported one `.bgcode` per material and printed them on the MK4S.
6. Recorded a video of the TPU print (head + body) on the MK4S, 2026-11-25:
   [`printingonprusa20261125.mp4`](printingonprusa20261125.mp4).
7. _To do:_ photograph each finished sample and record the results below.

## Results

_To be filled in once the prints are finished._

| | TPU | PLA Silk | PETG |
|---|---|---|---|
| Print succeeded? | | | |
| Surface finish | | | |
| Overhangs / support marks | | | |
| Flexibility / feel | | | |
| Head–body fit | | | |
| Floats? (pond test) | | | |
| Would we use it for Shenzhen? | | | |

## Photos and video

- Video, TPU printing on the Prusa MK4S (2026-11-25): [`printingonprusa20261125.mp4`](printingonprusa20261125.mp4)

Put photos in [`photos/`](photos/) and add them here, for example:

<!--
![TPU sample](photos/tpu.jpg)
![PLA Silk sample](photos/pla-silk.jpg)
![PETG sample](photos/petg.jpg)
-->
