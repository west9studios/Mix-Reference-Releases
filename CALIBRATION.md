# Mix Reference 1.12 — Calibration Report

**60 of 60 checks passed** · verified 25 November 2026 on macOS 15.7.7 (Apple silicon).

Every Mix Reference release is checked automatically before it is published. Reference signals
with known correct answers are measured by the release build, in exactly the way it measures your
tracks, and each reading is compared with the known answer. Where a value can be worked out
directly from the signal itself, such as its sample peak or its energy, that value is shown too.

## Standards

- Loudness: ITU-R BS.1770-4 (K-weighting, 400 ms blocks every 100 ms, −70 LUFS absolute and −10 LU
  relative gates), as used by EBU R128 and the major streaming platforms. Tested with the EBU Tech 3341
  loudness tests 1–5 and the EBU's tolerance of ±0.1 LU.
- True Peak: four points between every pair of samples are checked as well as the samples, so peaks
  between samples are found. Tested with the EBU Tech 3341 true-peak tests and the EBU's tolerance of
  +0.2 / −0.4 dB; the table shows how close each reading came. Mix Reference is not a certified meter.
- Very short sounds: a sound shorter than 0.4 s is measured over its whole length.
- Bands: the average level in each of the seven bands, Sub (20–60 Hz) to Air (12–20 kHz).

## The EBU test signals

The EBU Tech 3341 tests above are made by Mix Reference to the EBU's published specification, with
the EBU's expected readings and tolerances. The EBU's own test files can't be included with the app
or published, under the EBU's terms, so they are used only on the Mac that builds each release.
For this report, the EBU's own files for tests 1, 2, 3, 4, 5, 7, 8, 15, 16, 17, 18, 19, 20, 21, 22, 23 were measured as well (listed under
"EBU official test files").

## Results

| Area | What is verified | Check | Known answer | Mix Reference | Worked out directly | Result |
|---|---|---|---|---:|---:|:---:|
| EBU Tech 3341 loudness | The EBU's loudness tests 1–5, made to its published specification: 1 kHz tones in both channels at set levels and lengths, tolerance ±0.1 LU as the EBU sets. | Test 1: −23 dBFS, 20 s | -23.00 LUFS ± 0.10 | -22.99 | – | ✅ |
|  |  | Test 2: −33 dBFS, 20 s | -33.00 LUFS ± 0.10 | -32.99 | – | ✅ |
|  |  | Test 3: −36 / −23 / −36 dBFS | -23.00 LUFS ± 0.10 | -23.01 | – | ✅ |
|  |  | Test 4: −72 / −36 / −23 / −36 / −72 dBFS | -23.00 LUFS ± 0.10 | -23.01 | – | ✅ |
|  |  | Test 5: −26 / −20 / −26 dBFS | -23.00 LUFS ± 0.10 | -22.98 | – | ✅ |
| Level readings | A steady 997 Hz tone at −23 dBFS in both channels: its peak, its energy (peak − 3.01 dB) and its band. | True Peak | -23.00 dBTP +0.2 / −0.4 | -23.00 | sample peak -23.00 | ✅ |
|  |  | Energy | -26.01 dB ± 0.05 | -26.01 | -26.01 | ✅ |
|  |  | Band | Mid Range (500 Hz–2 kHz) | Mid Range (500 Hz–2 kHz) | – | ✅ |
| Mono files | The same tone at −20 dBFS in a mono file: one channel, so it reads 3 dB quieter than stereo. | Loudness | -23.01 LUFS ± 0.10 | -23.01 | – | ✅ |
|  |  | Energy | -23.01 dB ± 0.05 | -23.01 | -23.01 | ✅ |
| Sample rate and format | The tone at −20 dBFS, stereo, in a 44.1 kHz 24-bit file. | Loudness | -20.00 LUFS ± 0.10 | -20.00 | – | ✅ |
|  |  | Sample rate | 44100 Hz ± 0.50 | 44100 | – | ✅ |
|  |  | Bit depth | 24 bit | 24 | – | ✅ |
| Very short sounds | A 200 ms burst of the tone at −20 dBFS, shorter than one loudness measurement block. | Loudness | -20.00 LUFS ± 0.10 | -20.00 | – | ✅ |
|  |  | Length | 200.00 ms ± 0.50 | 200.00 | – | ✅ |
| EBU Tech 3341 true peak | The EBU's true-peak tests 15–19, made to its published specification: tones whose peaks fall between samples, faded in and out over 10 ms. Tolerance +0.2 / −0.4 dB, as the EBU sets. | Test 15: 12 kHz, 0.50, phase 0° | -6.00 dBTP +0.2 / −0.4 | -6.02 | sample peak -6.02 | ✅ |
|  |  | Test 16: 12 kHz, 0.50, phase 45° | -6.00 dBTP +0.2 / −0.4 | -6.19 | sample peak -9.03 | ✅ |
|  |  | Test 17: 8 kHz, 0.50, phase 60° | -6.00 dBTP +0.2 / −0.4 | -6.09 | sample peak -7.27 | ✅ |
|  |  | Test 18: 6 kHz, 0.50, phase 67.5° | -6.00 dBTP +0.2 / −0.4 | -6.06 | sample peak -6.71 | ✅ |
|  |  | Test 19: 12 kHz, 1.41, phase 45° | 3.00 dBTP +0.2 / −0.4 | 2.82 | sample peak -0.03 | ✅ |
| Frequency bands | A tone at −20 dBFS in the middle of each band, from 40 Hz to 16 kHz: it shows in its own band at the tone's level (−23.01 dB), every other band at least 20 dB lower. | 40 Hz tone: band level | -23.01 dB ± 0.25 | -23.01 | – | ✅ |
|  |  | 40 Hz tone: loudest band | Sub-Bass (20–60 Hz), others ≥ 20 dB lower | Sub-Bass (20–60 Hz), next 34.8 dB lower | – | ✅ |
|  |  | 90 Hz tone: band level | -23.01 dB ± 0.25 | -23.01 | – | ✅ |
|  |  | 90 Hz tone: loudest band | Bass (60–120 Hz), others ≥ 20 dB lower | Bass (60–120 Hz), next 36.9 dB lower | – | ✅ |
|  |  | 250 Hz tone: band level | -23.01 dB ± 0.25 | -23.01 | – | ✅ |
|  |  | 250 Hz tone: loudest band | Low-Mid (120–500 Hz), others ≥ 20 dB lower | Low-Mid (120–500 Hz), next 72.3 dB lower | – | ✅ |
|  |  | 1 kHz tone: band level | -23.01 dB ± 0.25 | -23.01 | – | ✅ |
|  |  | 1 kHz tone: loudest band | Mid Range (500 Hz–2 kHz), others ≥ 20 dB lower | Mid Range (500 Hz–2 kHz), next 97.0 dB lower | – | ✅ |
|  |  | 4 kHz tone: band level | -23.01 dB ± 0.25 | -23.01 | – | ✅ |
|  |  | 4 kHz tone: loudest band | Upper-Mid (2–6 kHz), others ≥ 20 dB lower | Upper-Mid (2–6 kHz), next 97.0 dB lower | – | ✅ |
|  |  | 9 kHz tone: band level | -23.01 dB ± 0.25 | -23.01 | – | ✅ |
|  |  | 9 kHz tone: loudest band | High (6–12 kHz), others ≥ 20 dB lower | High (6–12 kHz), next 97.0 dB lower | – | ✅ |
|  |  | 16 kHz tone: band level | -23.01 dB ± 0.25 | -23.01 | – | ✅ |
|  |  | 16 kHz tone: loudest band | Air (12–20 kHz), others ≥ 20 dB lower | Air (12–20 kHz), next 97.0 dB lower | – | ✅ |
| Harmonic | Low sine tones at known pitches, as a bass or 808 note. | 55.0 Hz (A1) | 55.0 Hz ± 1.0 | 54.8 | – | ✅ |
|  |  | 41.2 Hz (E1) | 41.2 Hz ± 1.0 | 41.2 | – | ✅ |
| Key | Held chords over their root in the bass, eight seconds each. | A Minor chord | A Minor, confidence ≥ 0.55 | A Minor, confidence 1.00 | – | ✅ |
|  |  | C Major chord | C Major, confidence ≥ 0.55 | C Major, confidence 1.00 | – | ✅ |
|  |  | F Minor chord | F Minor, confidence ≥ 0.55 | F Minor, confidence 1.00 | – | ✅ |
|  |  | G Major chord | G Major, confidence ≥ 0.55 | G Major, confidence 1.00 | – | ✅ |
| BPM | Twenty seconds of short clicks at a steady tempo. | 90 BPM clicks | 90 BPM ± 1.0 | 90.09 BPM, confidence 0.67 | – | ✅ |
|  |  | 120 BPM clicks | 120 BPM ± 1.0 | 119.75 BPM, confidence 1.00 | – | ✅ |
|  |  | 128 BPM clicks | 128 BPM ± 1.0 | 127.88 BPM, confidence 1.00 | – | ✅ |
|  |  | 174 BPM clicks | 174 BPM ± 1.5 (see Known limits) | 175.17 BPM, confidence 1.00 | – | ✅ |
| EBU official test files | The EBU's own Tech 3341 test files, measured on the build Mac with the EBU's tolerances. They are not included with Mix Reference or published: the EBU's terms don't allow it. | Test 1 (seq-3341-1-16bit.wav) | -23.00 LUFS ± 0.10 | -22.95 | – | ✅ |
|  |  | Test 2 (seq-3341-2-16bit.wav) | -33.00 LUFS ± 0.10 | -32.96 | – | ✅ |
|  |  | Test 3 (seq-3341-3-16bit-v02.wav) | -23.00 LUFS ± 0.10 | -23.01 | – | ✅ |
|  |  | Test 4 (seq-3341-4-16bit-v02.wav) | -23.00 LUFS ± 0.10 | -23.01 | – | ✅ |
|  |  | Test 5 (seq-3341-5-16bit-v02.wav) | -23.00 LUFS ± 0.10 | -22.98 | – | ✅ |
|  |  | Test 7 (seq-3341-7_seq-3342-5-24bit.wav) | -23.00 LUFS ± 0.10 | -22.99 | – | ✅ |
|  |  | Test 8 (seq-3341-2011-8_seq-3342-6-24bit-v02.wav) | -23.00 LUFS ± 0.10 | -23.00 | – | ✅ |
|  |  | Test 15 (seq-3341-15-24bit.wav.wav) | -6.00 dBTP +0.2 / −0.4 | -6.00 | – | ✅ |
|  |  | Test 16 (seq-3341-16-24bit.wav.wav) | -6.00 dBTP +0.2 / −0.4 | -6.17 | – | ✅ |
|  |  | Test 17 (seq-3341-17-24bit.wav.wav) | -6.00 dBTP +0.2 / −0.4 | -6.07 | – | ✅ |
|  |  | Test 18 (seq-3341-18-24bit.wav.wav) | -6.00 dBTP +0.2 / −0.4 | -6.04 | – | ✅ |
|  |  | Test 19 (seq-3341-19-24bit.wav.wav) | 3.00 dBTP +0.2 / −0.4 | 2.84 | – | ✅ |
|  |  | Test 20 (seq-3341-20-24bit.wav.wav) | 0.00 dBTP +0.2 / −0.4 | -0.13 | – | ✅ |
|  |  | Test 21 (seq-3341-21-24bit.wav.wav) | 0.00 dBTP +0.2 / −0.4 | -0.10 | – | ✅ |
|  |  | Test 22 (seq-3341-22-24bit.wav.wav) | 0.00 dBTP +0.2 / −0.4 | -0.13 | – | ✅ |
|  |  | Test 23 (seq-3341-23-24bit.wav.wav) | 0.00 dBTP +0.2 / −0.4 | -0.10 | – | ✅ |

## Known limits

- True Peak: a sound that starts or stops suddenly at full level can read a few tenths of a dB higher
  than the same sound faded in, because the sudden jump itself makes a peak between samples. The
  EBU's true-peak tests fade in and out over 10 ms, and are made that way here.
- BPM: readings are kept between 70 and 180 BPM and lean towards tempos near 130, so material at
  about 80 BPM or slower can read at double time, and 180 BPM or faster at half time. Near 174 BPM
  the reading can be just over 1 BPM high, so that test allows ±1.5 BPM.
- Key, BPM and Harmonic are estimates. They are checked here on clean test material with known
  answers; on music, the confidence tags in the app show how far to trust each reading.
- Surround files: loudness adds every channel equally, where the standard weights the rear channels
  higher and leaves out the LFE, so 5.1 files are not measured to the standard (EBU test 6 is not run).
- Mix Reference shows integrated loudness only, so the EBU's momentary and short-term tests (9–14)
  do not apply.
- The seven bands are Mix Reference's own. The checks confirm each band reads a tone at its true
  level; there is no outside standard for them.

## Check your own copy

Choose **Help ▸ Check Calibration…** in Mix Reference. It measures the same reference signals on
your Mac (all but the EBU's own files) in a few seconds and shows each reading next to its known
answer.
