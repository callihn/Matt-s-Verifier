# Matt's Verifier

An Android app that verifies street addresses by cross-referencing up to 10 geocoding services in parallel, then picks the best pin location so navigation routes to the street frontage — not the rooftop.

## Features

- **Multi-source geocoding** — Queries up to 10 geocoding services in parallel: Google Maps (native Android), US Census, Geocode.maps.co, Geoapify, LocationIQ, MapTiler, OpenCage, Positionstack, Radar, and TomTom
- **Matt's Pick** — Uses Matt's custom algorithm to determine the street frontage.
- **Address autocomplete** — Instant suggestions on every keystroke, powered by Android's native Geocoder with region biasing
- **Street verification** — Reverse-geocodes each result's coordinates to confirm the street matches your search
- **Visual agreement indicator** — Color-coded card shows how well sources agree (green = high, yellow = moderate, red = low)
- **Accuracy-sorted results** — Successful results ordered by proximity to centroid; failed results sort to the bottom
- **Interactive map** — Leaflet map with satellite toggle, colored markers per source, legend click-to-fly, and full-screen mode
- **Matt's Pick link** — Corrected coordinates shown at the top of results; tap to navigate
- **Encrypted API key storage** — Keys are stored encrypted on-device using Android EncryptedSharedPreferences (AES-256)
- **Navigation** — Open coordinates in Google Maps, Waze, Here WeGo, Here WeGo Beta, Open Street Maps, or TomTom
- **Dark/Light theme** — Toggle from the menu. All text properly rendered in white on dark backgrounds for readability

## Recent updates

### 2.4.0
- API key input fields now mask entered keys with dots instead of showing them in plain text

### 2.3.0
- Fixed content drawing under the title bar on Android 15+ — status bar and action bar spacing handled properly
- Dark theme readability for settings labels and dividers
- API key status indicator uses red (not orange) when no key is set
- Geocoder names in results use matching marker colors
- Street View button uses blue text in dark theme

## How it works

1. Enter an address and tap Verify
2. All configured geocoding services run in parallel
3. Matt's Pick uses Matt's custom algorithm to determine the street location.
4. A "Matt's Pick" row shows the coordinates determined by the algorithm to be closest to the street frontage.
5. Results are displayed with source markers on the map and an agreement indicator.

## Geocoding Sources

| Source | Coverage | Cost | Key Required |
|--------|----------|------|-------------|
| Google Maps | Worldwide | Free (unlimited) | No |
| Matt's Pick | Worldwide | Free (unlimited) | No |
| US Census | US only | Free (unlimited) | No |
| Geocode.maps.co | Worldwide | 25,000 free/day | Yes |
| Geoapify | Worldwide | 3,000 free/day | Yes |
| Radar | Worldwide | 100,000 free/month | Yes |
| LocationIQ | Worldwide | 5,000 free/day | Yes |
| TomTom | Worldwide | 2,500 free/day | Yes |
| OpenCage | Worldwide | 2,500 free/day | Yes |
| MapTiler | Worldwide | 100,000 free/month | Yes |
| Positionstack | Worldwide | 25,000 free/month | Yes |

## Settings

Configure your default navigation app, API keys (stored encrypted), and region override in Settings.

## Attribution

This product uses the Census Bureau Data API but is not endorsed or certified by the Census Bureau.

Map data © OpenStreetMap contributors.
