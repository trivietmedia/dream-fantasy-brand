# Video2X — Upscale Settings (720p → 1080p)

Saved settings for upscaling Dream Fantasy ambient clips with **Video2X Qt6 6.4.0** on Windows.

- Machine: Intel Core i7-12700K, 16 GB DDR4, SSD 512 GB, HDD 2 TB, **NVIDIA GeForce RTX 3060 12 GB**
- Source: 6-second AI-generated clips at 720p (loop/stitch after upscaling, not before)
- Target: 1920×1080 MP4 for Canva / YouTube

> Items marked *(unverified)* were not confirmed on the installed build.

## 1. Processing Settings tab

| Field | Value seen in app | Recommended |
|---|---|---|
| 1. Vulkan Device (GPU) | 0. NVIDIA GeForce RTX 3060 | keep |
| 2. Processing Mode | Filter (Upscaling) | keep |
| 3. Filter | Real-ESRGAN | keep |
| 4. Scaling Factor | 4 | `4` with `realesrgan-plus` (only option); `2` with `realesr-animevideov3` |
| 5. Model | realesr-animevideov3 | `realesrgan-plus` for real photos; `realesr-animevideov3` is tuned for anime and can look smooth/plastic |

Notes:
- `realesrgan-plus` only allows scaling factor 4 → output 5120×2880, then downscale to 1080p.
- `realesr-animevideov3` allows smaller factors → faster, 2x gives 1440p, then downscale to 1080p.
- Test both on one 6-second clip and compare water ripples, fabric, glass details and the star sky.

## 2. Encoder Options tab

| Field | Value seen in app | Recommended |
|---|---|---|
| suffix | `.mkv` | `.mp4` |
| codec | `libx264` | keep |
| pix_fmt | `auto` | `yuv420p` *(unverified: may need typing the value)* |
| bit_rate | `0` | keep (quality controlled by crf) |
| Custom: crf | `20` | `14` for the 4x intermediate, `16–18` for final-quality output |
| Custom: preset | `slow` | keep |

## 3. Downscale to 1080p (FFmpeg)

```
ffmpeg -i video_4x.mp4 -vf "scale=1920:1080:flags=lanczos" -c:v libx264 -crf 16 -preset slow -pix_fmt yuv420p -c:a copy video_1080p.mp4
```

## 4. Command-line equivalent *(unverified syntax — check `video2x --help`)*

```
video2x -i "D:\Upscale\input\clip.mp4" -o "D:\Upscale\output\clip_4x.mp4" -f realesrgan -r 4 -m realesrgan-plus
```

## 5. Folders

- Program: default install, `%LOCALAPPDATA%\Programs\video2x` (on the SSD)
- Working folders without spaces or accents: `D:\Upscale\input`, `D:\Upscale\output`
- Keep 50 GB+ free for temporary files; delete intermediates after downscaling.
- Output folder: not found in the GUI screenshots. Try Edit / File menus, or use the command line `-o` option.

## 6. Checks after upscaling

- Water ripples and sea: no shimmering or plastic look
- Stars: not turned into blotches or noise
- Candle flame and glass edges: no jitter
- Frame edges: nothing shifted

## 7. Download links

- Video2X releases: https://github.com/k4yt3x/video2x/releases
- Docs: https://docs.video2x.org
- FFmpeg: https://ffmpeg.org/download.html
