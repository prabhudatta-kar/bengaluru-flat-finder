# Bengaluru Flat Finder, prototype

**PROTOTYPE, ESTIMATED DATA. This is not a faithful reproduction of the source video or its project.**

This site contains 100 selected Bengaluru project names with OpenStreetMap geocoding. It is not a complete city directory. Locations have not been individually checked against primary sources.

Buy and rent ranges are rough corridor-based calculations using assumed unit sizes, not live listings or verified project prices. They are not reliable evidence of current price or availability.

## Correction after audit

The first version assigned BHK configurations, home sizes, smallest-bedroom sizes, amenities and ratings using project-class assumptions. These were not verified project facts. Those fields have now been removed from the shipped dataset, cards, shortlist and CSV. Their filters have been disabled. Do not rely on an earlier downloaded CSV.

Search, map markers, indicative budget filtering and CSV export remain as prototype interactions. CSV price columns are explicitly labeled estimates. Portal buttons are generic search attempts, not verified listings.

## Difference from the video

The video points to https://github.com/kairothq/flat-finder and https://flat-finder.pages.dev/. Its city-adaptation route reuses that project and its data pipeline. This prototype was instead built from scratch using Leaflet and hand-selected projects. It has not run the original Magicbricks city-wide pipeline, sourced floor-plan verification, building-outline map, confidence states, CLI or Claude connector.

A faithful version needs the original project and source-grounded Bengaluru data. No such rebuild has been completed here.

## Run locally

Open index.html, or run `python3 -m http.server 8000` in this folder. The app is a single static HTML file with Leaflet from a CDN and OpenStreetMap tiles. No paid services are used.
