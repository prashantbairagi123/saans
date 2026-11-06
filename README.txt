# SAANS – Every breath, decoded. Even offline.

**Live website:** https://prashantbairagi123.github.io/saans/
**Open the app directly:** https://prashantbairagi123.github.io/saans/app.html

SAANS (Hindi for *breath*) is a 74 KB air-pollution control app for India. It works with no internet, no sensor and no login, in English and हिंदी.

## Why SAANS
- 2.1 million deaths in India were linked to air pollution in 2021 (State of Global Air 2024).
- 89 of 96 NCAP cities were still above the national PM10 standard in 2025-26 (CREA).
- Most AQI apps show a number but not what to do, and go blank without internet or a nearby monitor.

## Six tools

| Tool | What it does |
|---|---|
| **Air** | Official CPCB National AQI from up to 7 pollutants, with advice for 6 groups, GRAP stage and a cigarette equivalent |
| **Sky-eye** | Estimates PM2.5 from how far you can see, for places with no monitoring station |
| **Detect** | Explainable source detective that ranks 7 pollution sources and drafts a complaint |
| **Control** | City control lab: 6 policy levers move the AQI and source mix live |
| **Plan** | Cleanest outdoor hours, your inhaled dose, and purifier sizing |
| **Act** | Daily clean-air pledges, points, streaks, badges and myth-busting cards |

## Highlights
- **Offline-first:** after the first visit it keeps working with the internet off; install it from the browser menu (Add to Home screen).
- **Tiny:** the whole app is a single 74 KB file with no libraries.
- **Private:** no login, no tracking, no permissions; data stays on the device.
- **Bilingual:** full English and Hindi.
- **Explainable:** every result shows the reasoning behind it.

## How it works
| Model | Science inside |
|---|---|
| AQI engine | CPCB National AQI breakpoints; overall AQI = highest sub-index |
| Sky-eye | Koschmieder visibility law (b = 3.912 / V) with humidity correction |
| Source detective | Seasonal priors × evidence weights → probabilities |
| Control lab | Source-apportionment shares × lever adoption × lever efficiency |
| Day planner | Daily PM2.5 curve × breathing rate × room and mask filtration |

## Files
- `index.html` – website
- `app.html` – the app (one self-contained file)
- `sw.js`, `manifest.json`, `icon-*.png` – offline install support
- `img/` – screenshots

## Run it yourself
Download the repository and open `app.html` in any browser, with no setup and no internet needed.

## Honest limits
Sky-eye and the source detective give estimates, not monitor readings. The source mixes and daily pollution curve are illustrative, adapted from published patterns. Health tips are general guidance, not medical advice.

## Sources
- Health Effects Institute and UNICEF, *State of Global Air 2024*
- CREA, *NCAP FY 2025-26 progress report* (April 2026); *Tracing the Hazy Air 2025*
- CPCB, *National Air Quality Index*; CAQM, *Graded Response Action Plan*
- WHO, *Global Air Quality Guidelines* (2021)
