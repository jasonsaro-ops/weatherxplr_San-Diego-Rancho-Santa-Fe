# WEATHERXPLR · Rancho Santa Fe 92067

Local WeatherXplr board for Rancho Santa Fe / ZIP 92067 (San Diego County, CA — SGX CWA).

## Layout
- **Left rail** — sample point, current conditions, gauges, AQI
- **Center** — dual Windy maps (radar + wind); secondary column bottom = **NWS alerts** (92067 point + San Diego County coastal)
- **Right rail** — 10-day forecast, temp / PoP / wind sparklines, NOAA tides, San Diego County hydro

## Features
- Dual Windy embeds (layer selectors)
- NWS alerts for **92067 + Rancho Santa Fe / San Diego County** (SGX CWA)
- Current conditions (Open-Meteo) + 48h sparklines
- Air quality (Open-Meteo) + 48h AQI / PM2.5 sparklines
- Hydro — USGS San Diego County gauges:
  - San Diego River at Fashion Valley `11023000`
  - San Luis Rey River at Oceanside `11042000`
  - San Diego River at Santee `11022480`
  - Sweetwater River near Alpine `11025500`
  - Santa Margarita River at Fallbrook `11046530`
- NOAA tides (station 9410170, San Diego)
- Click **WEATHERXPLR** (top left) to refresh data and recenter Windy maps on 92067

## Deploy
Static site — GitHub Pages. No worker required.

## Files
| Path | Role |
|------|------|
| `index.html` | Board UI |
| `app.js` | Feeds + dual Windy + alerts + sparks + tides + hydro |
