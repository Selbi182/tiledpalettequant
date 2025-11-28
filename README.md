# Tiled Palette Quant - MD fork

This is a fork of [rilden's Tiled Palette Quant web tool](https://rilden.github.io/tiledpalettequant), with the intention of changing a handful of details to make development for Sonic hacking easier -- namely by changing default values.

It's permanently accessible here: https://tiledpalettequant.selbi.club/

## Differences to [original version](https://github.com/rilden/tiledpalettequant)

- Quantization:
  - Palette images are generated with 8x8 pixels per color instead of 16x16. This is a requirement of many art importers, including SonPLN and GetArt.NET
  - Always download quantized image as .png (never .bmp)
  - Changed default values:
    - Palettes: 1 (used to be 8)
    - Colors per palette: 16 (used to be 4)
    - Bits per channel: 4 (used to be 5)
- Website:
  - Gave the site a huge visual facelift to make it look less like it was created in the 90s
  - Disable dither settings when set to Off
  - Disabled autocomplete for all inputs
  - Dereference image loading to avoid quirks with client-side width/height adjustments
- Project:
  - Restructured original folder layout
  - Changed [sample image](https://wallscloud.net/en/wallpaper/nature/plants/Pablo-Garcia-Saldana/pKL1)
  - Added favicon (based on sample image)
  - Removed TS stuff
  - Removed duplicated v0.1 source folder