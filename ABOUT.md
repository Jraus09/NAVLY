# Navly — VFR Pilotage Waypoint Planner

A free, self-contained VFR flight planning tool for general aviation pilots. Plan visual routes, identify pilotage waypoints, and export directly to SkyVector or as a GPX file.

**Live app:** https://jraus09.github.io/NAVLY/index.html

---

## Features

- **Automatic waypoint selection** — scores 22,000+ US airports and 500+ named landmarks to find the best visual checkpoints along your route
- **Full airport coverage** — every public and private airport in the US from OurAirports data
- **Printable kneeboard** — half-letter (4.25in) card with DMS coordinates, magnetic headings, leg distances, field elevations, and frequencies
- **GPX export** — load your route into any GPS or moving map app
- **SkyVector export** — opens your full route in SkyVector with one click, plotted on the sectional chart
- **Terrain profile** — elevation chart along the route with cruise altitude overlay
- **Offline** — no internet required after the page loads (terrain elevation fetched on demand)

---

## How to Use

1. Enter your **departure** and **destination** ICAO/FAA identifiers (e.g. `KAVL`, `KATL`)
2. Set your **cruise altitude** and number of **waypoints** (5–8)
3. Click **Plan Route**
4. Review waypoints, terrain profile, and route summary
5. Export via **GPX**, **SkyVector**, or print the **Kneeboard**

---

## Waypoint Scoring

Waypoints are selected by scoring all airports and landmarks within 35nm of the route corridor:

| Type | Priority |
|---|---|
| Named landmarks (towns, lakes, rivers) | Highest |
| Major hub airports | Very high |
| Towered airports (Class C/D) | High |
| Public GA airports | Medium |
| Private airstrips | Low (last resort) |

Private strips include a note to confirm on sectional before use.

---

## Data Sources

- **Airports** — OurAirports (22,094 US airports, public and private)
- **Landmarks** — curated database of 506 VFR-relevant visual references
- **Terrain** — OpenTopoData (USGS NED 10m / SRTM 30m)
- **Magnetic declination** — IGRF2024 polynomial fit

---

## Disclaimer

**NOT FOR NAVIGATION.** For flight planning reference only. Always consult current sectional charts, NOTAMs, TFRs, and official FAA sources. File a VFR flight plan before every cross-country flight.

---

## Built With

Vanilla JavaScript · Single HTML file · No frameworks · No server required
