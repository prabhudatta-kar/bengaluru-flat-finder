# Bengaluru Flat Finder

Built from the original Flat Finder app by Divy Kairoth (https://github.com/kairothq/flat-finder), using the Bengaluru adaptation and pipeline output from https://github.com/aryabharat/flat-finder. Source code is preserved here. This replaces an earlier from-scratch prototype with guessed project attributes; do not rely on its old CSV downloads.

## Data caveats

This is a third-party snapshot, not a fresh crawl or live inventory. Dataset-reported totals: 14,200 projects listed, 13,566 societies on map, 46,443 sale listings and 12,425 rental listings. These counts are not independently audited. Bedroom dimensions: no plans have been read; unknown dimensions must remain unknown. Portal facts, listing-based medians and modeled prices have different confidence levels. Verify listings, prices, amenities and dimensions at their cited sources before deciding. The dataset covers part, not all, of the city-wide portal directory.

## Source and run

The app is in web/, the data pipeline in pipeline/, and CLI in cli/. Run npm ci then npm run dev inside web/. This repository also contains the compiled site at its root for GitHub Pages. Read ATTRIBUTION.md for authorship and license notes. No paid services are used by this build. The Claude MCP function is preserved as source but is not served by GitHub Pages.
