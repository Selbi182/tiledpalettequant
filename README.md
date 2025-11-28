# Tiled Palette Quant - MD fork

This is a fork of [rilden's Tiled Palette Quant web tool](https://rilden.github.io/tiledpalettequant), with the intention of changing a handful of details to make development for Sonic hacking easier -- namely by changing default values.

It's permanently accessible here: https://tiledpalettequant.selbi.club/

## Differences to [original version](https://github.com/rilden/tiledpalettequant)

- Palette images are generated with 8x8 pixels per color instead of 16x16. This is a requirement of many art importers, including SonPLN and GetArt.NET.
- Changed default values:
  - Palettes: 1 (used to be 8)
  - Colors per palette: 15 (used to be 4)
  - Bits per channel: 4 (used to be 5)
- Dereference image loading to avoid quirks with client-side width/height adjustments
- Gave the site a huge visual facelift to make it look less like it was created in the 90s
- Restructured original folder layout, changed default image, added favicon, removed TS stuff, removed duplicate folder