# VACE — AMD port (Radeon 8060S)

One-click Windows installer for VACE (Wan VACE), ported from NVIDIA-only to AMD. Free.

## What it does

VACE is an all-in-one video creation and editing tool — it generates and edits video from text, images, and reference frames, including first-and-last-frame generation.

## Tested on

- AMD Ryzen AI Max+ 395 with Radeon 8060S (gfx1151)
- BOSGAME M5

Reported test results from our developer team's testing on that machine: an installed GPU run produced a 17-frame 320×320 clip, peaking at about 11.2 GiB of graphics memory; silent install and uninstall passed.

## Before you install

**You need the AI Video Suite installed first.** This port uses the Suite's ROCm Python and Wan/VACE weights read-only. On install it downloads the pinned ComfyUI files it needs; if the weights are not already present, it downloads them (about 11 GB).

**Hardware check — please read first.** The installer checks your hardware before it installs. This build is made for a machine with an AMD Radeon 8060S (gfx1151) and the Suite's PyTorch ROCm stack (torch 2.9.1+rocmsdk).

If your machine does not match, the installer shows the specs it found and offers to let you send them to us for review. It then exits without installing anything (exit code 10). Other hardware is not supported by this build.

## Download

Installer: `VACE-AMD-Setup-1.1.0.exe` — 153,276 bytes
SHA-256: `85f8b731355b79aedaeb17391d5dee38defde32d2767a574ee22fdaf6e2221fe`

## We port NVIDIA software to AMD

Hi I'm Hal ports AI software that was made for NVIDIA only, so it runs on AMD hardware.

Got a program you'd like to see ported? Suggest it. And if your AMD machine isn't on our tested list, you can offer your specs for testing through our compatibility program.

Contact us at https://hiimhal.com

## Licence and credit

Licence: Apache License 2.0 (upstream VACE).

Upstream project: https://github.com/ali-vilab/VACE — credit to the VACE authors. This port is not affiliated with or endorsed by the upstream project.

Ported by a developer from Ontario.
Home and full catalogue: https://hiimhal.com
Support: hello@hiimhal.com
