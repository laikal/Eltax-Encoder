# Third-Party Source Availability — ELTAX Encoder 0.70C

This document records the source-availability evidence shipped with the local 0.70C package. It is a technical provenance note, not a legal opinion.

## FFmpeg / FFprobe 9.0.2 Gyan Full — PARTIAL

- Observed binary: `9.0.2-full_build-www.gyan.dev`.
- The binary reports `--enable-gpl --enable-version3 --enable-static`; `ffmpeg -L` reports GPL version 3 or later.
- The bundled Gyan README names FFmpeg source commit `946fcce07b`: https://github.com/FFmpeg/FFmpeg/commit/946fcce07b.
- Gyan binary archive: `ffmpeg-9.0.2-full_build.7z`; SHA-256 `f0e46253c70dfe902bac915dfb4224f0cf1b7c6eeab9da2ccc9a5581f9a71b13`.
- FFmpeg source archive included in the companion asset: `FFmpeg-946fcce07b.tar.gz`; SHA-256 `0AA2B1DE2A5698B20A23E93D539A9A8E82CA0117496C5BDF05D198805F42BB3B`.
- Companion asset: `FFmpeg-9.0.2-Gyan-Full-Source-PARTIAL.zip`; SHA-256 `CA9B976E7EAF521723D854BD0EDF8903E75A37DE92779769C27162D7A969CC28`.
- The companion includes the exact identified FFmpeg source tree archive, GPL text, Gyan license/README, and captured version/build-configuration/license output.
- **Status: FFMPEG SOURCE PACKAGE PARTIAL.** The public Gyan materials inspected did not provide verified Gyan build scripts/configuration source, exact applied patch set, or build-matched source and license files for every statically linked external library. The FFmpeg source commit and observed build configuration do not close those gaps. The asset is not described as complete corresponding source and may not be used to claim that the bundled static binary can be reproduced exactly from the included files.
- Runtime structure is unchanged: the application executes `ffmpeg.exe` and `ffprobe.exe` as separate processes.

## Model rights summary

- L4: **CLOSED WITH REASONABLE DUE DILIGENCE**.
- L5: **CLOSED WITH DECLARED CONDITIONS**.
- Nine models are included: five `CONDITIONAL`, four `REASONABLE_DUE_DILIGENCE_PASS`, zero excluded. The detailed source, attribution, license conditions, conversion information, and artifact hashes are in `MODEL_NOTICES.txt` and `THIRD_PARTY_COMPONENTS.json`.
- The declared 0.70C distribution plan is free, with no sale, advertising, subscription, or paid features. The five CC model entries retain their applicable NC and/or SA conditions. Code licenses are not assumed to license model weights.

## Other software/runtime notices

The existing .NET, NCNN/native, DAT2, and Microsoft runtime notices and provenance records from the 0.66c baseline are carried forward. Microsoft VC runtime provenance limitations remain explicitly recorded; no new provenance claim is made in this finalization.
