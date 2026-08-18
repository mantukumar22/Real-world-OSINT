# Module 03 — Geolocation OSINT (Without GPS)

## Concept
"Jagah ka pata — clues se, not GPS se." Bellingcat-style geolocation relies on
**visual reasoning**, not device metadata.

## Core Clue Categories
| Clue | What It Tells You |
|---|---|
| Landmarks / buildings | City / region match via Street View |
| Signboards / language / script | Country, sometimes exact district |
| Sun position & shadow length | Time of day, rough latitude (via SunCalc) |
| Vehicle plates | Country/state (e.g., India: DL, MH prefixes) |
| Weather visible in image | Season, cross-reference with historical weather data |
| Architecture style | Region-specific building conventions |

## Tools
- **Google Street View / Maps** — match physical landmarks
- **Mapillary** — crowd-sourced street-level imagery, useful where Street View is sparse
- **SunCalc.org** — calculate sun position for a given time/date/location to
  verify shadow angles
- **GeoGuessr** — *training* tool to sharpen your visual geolocation instincts
  (not an investigative tool itself)

## Bellingcat-Style Case Study Table

| Case | Year | Focus | Techniques | Outcome |
|---|---|---|---|---|
| MH17 | 2014 | Missile origin | Satellite images, video geolocation | Traced launcher to Russian Buk unit |
| Syrian Chemical Attacks | 2013–2018 | Verifying attack footage | Video metadata, terrain matching | Verified ground footage vs. claims |
| ISIS Execution Sites | 2014 | Locating execution videos | Terrain + shadow matching, Google Earth | Confirmed locations for war-crimes evidence |
| Skripal Poisoning | 2018 | Identifying GRU agents | Leaked passport DBs, travel records | Unmasked undercover officers |

## Practice Exercise (Legal & Fun)
Play GeoGuessr for 20 minutes daily — it directly trains the pattern-recognition
skill used in real geolocation investigations, with zero privacy risk since
locations are randomly generated, not real people's homes.

## Ethics Note
Geolocating a **public figure's public post** for journalism/accountability is
different from geolocating a private individual's casual vacation photo to find
their home. The former is investigative journalism; the latter is stalking.
Scope and consent matter more than technique.
