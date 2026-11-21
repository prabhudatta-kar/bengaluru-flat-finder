# Bengaluru Flat Finder

An interactive map of 100 major apartment societies/projects across Bengaluru - search by area, filter by budget (buy or rent), BHK, home size, smallest-room size and amenities, and pull every match onto one map. Inspired by the Gurugram flat-finder from the video "Real estate is going to change forever (This time by Claude)".

## Run it

It is a fully static site - open `index.html` in a browser, or serve the folder:

```
python3 -m http.server 8000
# then http://localhost:8000
```

Or use the hosted GitHub Pages link (see the repo's About section).

## Features

- Full-city map (OpenStreetMap + CARTO dark tiles, Leaflet) with a marker per society
- Search by area, locality, corridor, builder or society name; map zooms to matches
- Buy / Rent toggle with a budget slider (buy: ₹40L-₹6Cr, rent: ₹15k-₹1.5L/mo)
- BHK multi-select (1/2/3/4 BHK)
- Minimum home size (sqft) and minimum smallest-room size (sqft) filters
- Amenity filters: gym, pool, tennis, clubhouse, kids play area, badminton, squash, spa, golf, power backup
- Live match count + scrollable shortlist; click to fly to the society
- Detail card per society: configs, sizes, est. buy/rent ranges, indicative rating, amenities, and deep links to Google Maps, 99acres, MagicBricks and NoBroker
- Download the current filtered list as CSV

## Data & method

- **Society list & coordinates**: curated list of 100 well-known projects across 17 corridors (Whitefield, Sarjapur Road, Electronic City, HSR, Koramangala, Bellandur, Marathahalli, Hebbal, Thanisandra, Yelahanka, Devanahalli, Bannerghatta Road, Kanakapura Road, JP Nagar, Central-West, CBD, Indiranagar), geocoded against OpenStreetMap (Nominatim). Hits that did not validate against their corridor were dropped, so some good projects are missing from v1.
- **Prices & rents**: corridor-level estimates built from Q3 2026 market data (e.g. corridor ₹/sqft and median 2BHK rents) multiplied by typical configuration sizes. They are shortlisting aids, **not** listings - always verify on the portals.
- **Amenities / ratings**: indicative, from project class (standard / township / premium); verify per project.

## Files

- `index.html`, `styles.css`, `app.js` - the app
- `data.js` - the society dataset (`window.SOCIETIES`)

No build step, no dependencies beyond Leaflet from CDN.
