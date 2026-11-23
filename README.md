<p align="center">
  <img src="https://i.postimg.cc/gJS5K4MT/banner.png" alt="CleanCut Offline Background Remover — Batch Transparent PNG Cutouts Without Watermarks" width="100%">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Windows%2010%2F11%20x64-0078D6?style=flat-square&logo=windows" alt="Platform: Windows 10/11 x64">
  <img src="https://img.shields.io/badge/Mode-Offline%20BG%20Remover-2EA44F?style=flat-square" alt="Mode">
  <img src="https://img.shields.io/badge/Release-cleancut--ai--v1.1-5391FE?style=flat-square" alt="Release Tag">
  <img src="https://img.shields.io/badge/License-MIT-8B5CF6?style=flat-square" alt="License: MIT">
</p>

# CleanCut Offline Background Remover — Batch Transparent PNG Cutouts Without Watermarks

**Web background removers shrinking your 4K photos down to blurry 500px previews unless you pay? Remove backgrounds from product shots, YouTube thumbnails, portraits, and stickers in full native resolution—100% offline on Windows.**

CleanCut Offline Background Remover runs local neural segmentation models on your PC: **preserving full original image resolution, outputting crisp alpha-channel `.png` cutouts (`*_nobg.png`), and supporting bulk folder processing with zero watermarks**.

This project is aimed at **Windows 10 and Windows 11 (64-bit) creators, e-commerce sellers, and designers** who need fast, full-resolution transparent PNGs without cloud subscriptions.

## Quick Use-Case & Troubleshooting Reference

| Scenario / Issue | Cause | Solution |
| --- | --- | --- |
| Online background removers downscale HD images to 625×400 | Websites paywall full-resolution transparent PNG downloads | Process images locally at 100% original resolution (up to 4K+) |
| Need to cut out 50 product photos or game icons at once | Manual lasso/pen masking in editors takes hours | Drop an entire folder for automatic batch `*_nobg.png` export |
| Hair, fur, and fine edges look jagged | Basic color-key magic wand tools leave harsh halos | Use local neural alpha-matting for smooth semi-transparent edges |
| Uploading client photos or unreleased assets is restricted | Cloud editors store uploaded images on third-party servers | Run 100% offline with zero network traffic |

## Download for Windows

[**Download CleanCutAI.zip — Latest GitHub Release (Windows x64)**](../../releases/latest/download/CleanCutAI.zip)  
[View All Releases & Changelog](../../releases) · [Report an Issue](../../issues)

### Why use `CleanCutAI.exe`? (Key features)

- Removes backgrounds from `.jpg`, `.png`, `.webp`, and `.bmp` images at full native resolution.
- Outputs clean 32-bit RGBA transparent PNG files (`*_nobg.png`) with zero watermarks.
- Supports batch folder processing for dozens of product photos or thumbnail assets at once.
- Runs locally via ONNX Runtime (DirectML / CPU) with no Python setup required.

### Sample Output

```text
[CleanCutAI] Loaded 12 images from D:\Thumbnails\Raw_Portraits
[INFO] Inference Engine : DirectML Hardware Acceleration (Full Resolution 2560x1440)
[OK]   portrait_01.jpg  -> portrait_01_nobg.png (1.8 MB | 0.9s)
[OK]   Batch Complete   : 12/12 transparent PNGs saved to D:\Thumbnails\Cutouts
```

The release ZIP is named `CleanCutAI.zip`; the Windows executable inside is named `CleanCutAI.exe`.

1. Close CleanCut AI before updating or replacing executable files.
2. Click **Download CleanCutAI.zip** above.
3. Right-click the downloaded archive and choose **Extract All**.
4. Open the extracted folder and run `CleanCutAI.exe`.
5. Review the options and output paths before processing files.

**Requirements:** Windows 10 or 11 (64-bit), 8 GB+ RAM (DirectML / CUDA GPU acceleration supported).

### Verification & Windows SmartScreen Note

- **Offline & standard user permissions:** `CleanCutAI.exe` runs locally without uploading your files and does not require disabling Windows Defender.
- **Windows SmartScreen:** Because this is an independent open-source utility without a commercial EV code-signing certificate, Windows SmartScreen may show *"Windows protected your PC"* on first launch. Click **More info → Run anyway** after verifying the release checksum on the [Releases](../../releases) page.

## Problems this project solves

### Paywalled high-resolution exports on web tools

Most online background removers restrict free users to low-resolution previews.

### Slow one-by-one manual masking

Batch processing turns a whole folder of raw photos into transparent PNGs in seconds.

### Full privacy for personal and commercial assets

Images are processed strictly in local memory.

### Zero installation dependencies

Portable `.exe` runs directly after extraction.

## Default folders and configuration paths

CleanCut AI saves transparent cutouts into a `Cutouts` subfolder next to your source images:

```text
%USERPROFILE%\Pictures\Cutouts\
```

Typical directory layout:

```text
Pictures\Products\
├── item_01.jpg
└── Cutouts\
    └── item_01_nobg.png   (Full-resolution RGBA transparent PNG)
```

Original images are never overwritten.

## Quick start guide

Follow these steps to get started:

1. **Extract `CleanCutAI.zip` to a local folder.** No installer or admin elevation needed.
2. **Launch `CleanCutAI.exe` and drag images or folders onto the window.** Supports JPG, PNG, WebP, and BMP.
3. **Choose output mode (`Transparent PNG` or solid color backdrop).** Optionally enable edge-feathering refinement.
4. **Click **Remove Backgrounds**.** Processed files appear in `Cutouts\` within seconds.

### Data safety note

Source images remain untouched in their original folder.

## What the status summary shows

CleanCut AI displays **input resolution, active hardware backend, processing time per image, and output PNG path**.

## FAQ

**Does CleanCut AI reduce image resolution or add watermarks?**

No. Every output PNG keeps 100% of the source image's pixel dimensions with zero watermarks.

**Does it work offline without an internet connection?**

Yes—all segmentation runs locally on your PC.

**What formats can I import?**

JPG, JPEG, PNG, WebP, and BMP.

## Useful reading

- [ONNX Runtime DirectML Documentation](https://onnxruntime.ai/docs/execution-providers/DirectML-ExecutionProvider.html)

## More Windows Desktop Utilities

- [SnapFormat-BatchMediaConverter](../SnapFormat-BatchMediaConverter) — Offline batch HEIC/WebP/MKV to JPG/PNG/MP4 converter
- [ExifScrub-PhotoMetadataCleaner](../ExifScrub-PhotoMetadataCleaner) — Strip GPS, EXIF & camera metadata from photos offline
- [ClipShrink-DiscordCompressor](../ClipShrink-DiscordCompressor) — Compress gameplay clips to exact 10 MB / 50 MB Discord limits
- [SnipText-ScreenOCRClipboard](../SnipText-ScreenOCRClipboard) — Instant hotkey screen region OCR text extractor to clipboard

*Independent open-source desktop utility for Windows.*
