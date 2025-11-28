# Tiled Palette Quant - MD fork

This is a fork of [rilden's Tiled Palette Quant web tool](https://rilden.github.io/tiledpalettequant), with the intention of changing a handful of details to make development for Sonic hacking easier -- namely by changing default values.

## Differences to [original version](https://github.com/rilden/tiledpalettequant)

- Palette images are generated with 8x8 pixels per color instead of 16x16. This is a requirement of many art importers, including SonPLN and GetArt.NET.
- Changed default values:
  - Palettes: 1 (used to be 8)
  - Colors per palette: 15 (used to be 4)
  - Bits per channel: 4 (used to be 5)
- Improved CSS styling to make the app look less like it came from the 90s
- Removed some junk files from the source and changed default image