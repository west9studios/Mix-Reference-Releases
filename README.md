![West 9 Studios · Mix Reference](Screenshots/header.png)

# Mix Reference

**Hear and see how your mix compares, in seconds.** Mix Reference is a free macOS app from West 9 Studios that puts your demo or work-in-progress next to a whole folder of reference tracks or samples, so you can audition them, measure them and compare them without leaving one window.

[**Download Mix Reference 1.12**](https://github.com/west9studios/Mix-Reference-Releases/releases/latest) · macOS 13 or later · 2.7 MB · Free, no account or licence key

![Mix Reference comparing a demo against a track from its target library, with the listening filters on the right](Screenshots/main.png)

## What it does

Load your own track as the **Demo Reference**, point the app at a folder as the **Target Library**, and step through the folder with ↑ and ↓. Press ← to hear your demo from the top and → for the selected track: a quick A/B without the mouse. Every track you play is analysed, so the readings fill in as you audition.

- **Nine readings per track:** LUFS loudness, True Peak (ISP), Energy, Harmonic, Key, BPM, dominant Band, length and format, shown for your demo and the selected target side by side.
- **Seven-band frequency comparison:** see where your demo has more or less energy than a chosen track, or than the average of the whole library, from Sub (20-60 Hz) up to Air (12-20 kHz), with the difference in dB.
- **Low-pass, high-pass and band-pass listening:** isolate one slice of the spectrum on the demo, the target, or both, to hear exactly where two tracks differ.
- **Fast library auditioning:** arrow-key navigation plays each track as you land on it. Sort by Name, LUFS, Energy, Key, BPM, Band or Time; the Key column follows the Circle of Fifths. Your Mac's play, previous and next keys work too, even with another app in front.
- **Loop and Reverse:** keep a sample cycling while you browse, or play it backwards to find swells, risers and interesting tails.
- **Drag-and-drop export:** drag chosen files to the Desktop or into your DAW. The app copies them and never touches the originals.
- **Export Report:** save a clean, formatted report of your session as a web page, ready to read, print as a PDF or send to a client.
- **Dark by default, in the West 9 Studios style,** with Light and Match the Mac options, your own colours, and live CPU, memory and disk meters.
- **Built-in Help Center and one-click updates:** a searchable manual is included, and the app tells you when a new version is available and installs it for you.

<table>
  <tr>
    <td width="50%"><img src="Screenshots/help-center.png" alt="The built-in Help Center: every function explained, searchable"></td>
    <td width="50%"><img src="Screenshots/help-keyboard.png" alt="The Help Center's keyboard page: every shortcut in one table"></td>
  </tr>
  <tr>
    <td align="center"><sub>A searchable Help Center is built in</sub></td>
    <td align="center"><sub>Every shortcut in one table</sub></td>
  </tr>
</table>

## Why use it

- Stop switching between a loudness meter, a spectrum analyser and a file browser: the comparison happens in one place.
- Judge your mix against commercial references by ear and by number at the same time.
- Get through hundreds of files quickly, whether you are choosing references, building a set or curating a sample library.
- Your audio files are never modified.

## Who it's for

- **Mixing and mastering engineers** checking tonal balance and loudness against commercial masters.
- **DJs** building sets by key, tempo and loudness.
- **Producers and remixers** matching a rough demo to the sound of a genre.
- **Beat makers and sound designers** auditioning drum loops, samples and FX, including in reverse.
- **Film and game composers** comparing cues against temp tracks.

## What's new

- Help ▸ Check Calibration… confirms on your own Mac that the readings are right: test sounds with known answers, including the EBU's loudness and true-peak tests, measured exactly as your tracks are, with each result next to its answer.
- Every release is now checked the same way before it is published, and its calibration report is on the download page.

The full history is in the app under **Help > What's New**.

## Calibration

Every release is checked before it is published: reference signals with known correct answers, including the EBU's loudness and true-peak tests (EBU Tech 3341), are measured by the release build, and each reading is compared with the known answer and the EBU's tolerance. The report also lists the known limits. [Read the calibration report](https://github.com/west9studios/Mix-Reference-Releases/blob/main/CALIBRATION.md). To check your own copy, choose **Help > Check Calibration…** in the app.

## Install

1. Download the DMG from the [latest release](https://github.com/west9studios/Mix-Reference-Releases/releases/latest).
2. Open it and drag **Mix Reference** into **Applications**.
3. Launch the app. If macOS blocks the first launch, open **System Settings > Privacy & Security** and choose **Open Anyway**.

Once installed, Mix Reference checks for new versions when it starts. Choose **Update & Relaunch** when the orange notice appears and the app updates itself. Each release also publishes a `.sha256` file if you want to verify your download.

Version 1.12 was released on 25 November 2026. DMG SHA-256: `456177ffe2f7191a6faa7482758b9d93bfed28995c991e1fd99c4fb18fce439a`

## More from West 9 Studios

- [Normalizer Pro](https://github.com/west9studios/Normalizer-Pro-Releases): prepare a whole folder of samples in one pass.
- [Mix Reference](https://github.com/west9studios/Mix-Reference-Releases): compare your mix with reference tracks, band by band.
- [Mac Utility](https://github.com/west9studios/Mac-Utility-Releases): audio workstation maintenance: disk space, plugins, startup items and sample-library tidying.
- [Sample Analyzer](https://github.com/west9studios/Sample-Analyzer-Releases): analyse entire folders of samples for loudness, true peak, instrument detection and mix balance.

## Licence

MIX REFERENCE — PLAIN-LANGUAGE LICENCE NOTICE

Mix Reference is free to use. It remains the property of West 9 Studios.

You may not redistribute, resell, modify, or reverse-engineer Mix Reference, or
claim it as your own. No licence key or payment is required to use the app.

Mix Reference is provided “as is”, without any warranty, express or implied.
West 9 Studios is not responsible for loss or damage arising from its use.

OPEN-SOURCE COMPONENTS

Mix Reference contains no third-party or open-source code. It is built only on
the frameworks that come with macOS.

PRIVACY

Mix Reference does not collect, store or send any personal information. It
opens the sound files you choose only to play and measure them, and nothing it
finds leaves your Mac. It never changes your audio files: dragging tracks out
makes copies, and reports are saved only where you choose. The only connection
it makes is the update check: when the app starts, it asks GitHub (github.com)
whether a newer version exists, and it downloads the update from GitHub if you
choose to install it. Like any web request, this lets GitHub see your network
address; GitHub's own privacy policy applies to that. West 9 Studios receives
nothing from these checks. GitHub counts how many times each release is
downloaded; those counts contain no information about who downloaded it.

This is a plain-language notice, not legal advice. It does not replace any
rights or obligations that may apply under the law.
