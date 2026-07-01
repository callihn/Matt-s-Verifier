# <img width="24" height="24" alt="icon" src="https://github.com/user-attachments/assets/135cac6c-9f56-4d17-8cd9-eb309d9a3ef3" /> Matt's Verifier

Matt's Verifier is a proof-of-concept address verification tool that cross-references up to 10 geocoding services in parallel and determines the correct street-frontage location. It also serves as a practical test bed for evaluating geocoding service accuracy and consistency across providers.

---

#### 📦 Downloads

[![Get the App](https://img.shields.io/github/v/release/callihn/Matt-s-Verifier?style=for-the-badge&label=%F0%9F%8C%A4%20Get%20the%20Latest%20Version&color=2ea44f)](https://github.com/callihn/Matt-s-Verifier/releases/latest)

---

# 📸 Screenshots

<details>
<summary>Click here to expand app screenshots</summary>
<br />

| | | |
| :---: | :---: | :---: |
| <img src="https://github.com/user-attachments/assets/26e5ac50-cfb8-453f-af35-0b219d20e28c" width="220" alt="Screenshot 1" /> | <img src="https://github.com/user-attachments/assets/bdaccab6-656a-4a6c-ab75-447aa55469cf" width="220" alt="Screenshot 2" /> | <img src="https://github.com/user-attachments/assets/db55e6a6-8d61-437e-9895-8511bc42644d" width="220" alt="Screenshot 3" /> |
| <img src="https://github.com/user-attachments/assets/09a9b754-41ed-45c9-9f29-a659178a8a66" width="220" alt="Screenshot 4" /> | <img src="https://github.com/user-attachments/assets/1853dd16-43a6-46f9-8d66-c04c901ca2da" width="220" alt="Screenshot 5" /> | <img src="https://github.com/user-attachments/assets/9e6c8b23-235e-44e7-9dd9-5a411a3841b0" width="220" alt="Screenshot 6" /> |
| <img src="https://github.com/user-attachments/assets/9534fcbd-1650-410c-8828-078c91faeb80" width="220" alt="Screenshot 7" /> | <img src="https://github.com/user-attachments/assets/ecfb5333-7518-4f43-965f-895acd82b889" width="220" alt="Screenshot 8" /> | <img src="https://github.com/user-attachments/assets/d3f5a846-b6c0-4ec9-838e-a07abb522443" width="220" alt="Screenshot 9" /> |
| <img src="https://github.com/user-attachments/assets/336873e0-a669-4395-b043-a671bb546e68" width="220" alt="Screenshot 10" /> | <img src="https://github.com/user-attachments/assets/f53ce410-d223-4119-9df2-c6d07c0d3f10" width="220" alt="Screenshot 11" /> | <img src="https://github.com/user-attachments/assets/30795760-4f7a-4e7d-b063-e9d777a10901" width="220" alt="Screenshot 12" /> |
| <img src="https://github.com/user-attachments/assets/aba064b2-7bec-493b-8cd4-53a830e7b7e6" width="220" alt="Screenshot 13" /> | <img src="https://github.com/user-attachments/assets/4c153312-02d6-4124-91db-81f75ced32f6" width="220" alt="Screenshot 14" /> | <img src="https://github.com/user-attachments/assets/693539cd-6de7-4b10-a5e6-00af6297ac86" width="220" alt="Screenshot 15" /> |

</details>

---

## 🪄 Features

- **Multi-source geocoding** — Queries up to 10 geocoding services in parallel
- **Matt's Pick** — Custom algorithm to determine the correct street-frontage location
- **Address autocomplete** — Instant suggestions on every keystroke, powered by Android's native Geocoder with region biasing
- **Street verification** — Reverse-geocodes each result's coordinates to confirm the street matches your search
- **Visual agreement indicator** — Color-coded card shows how well sources agree (green = high, yellow = moderate, red = low)
- **Accuracy-sorted results** — Successful results ordered by proximity to centroid; failed results sort to the bottom
- **Interactive map** — Leaflet map with satellite toggle, colored markers per source, legend click-to-fly, and full-screen mode
- **Matt's Pick link** — Corrected coordinates shown at the top of results; tap to navigate
- **Encrypted API key storage** — Keys are stored encrypted on-device using Android EncryptedSharedPreferences (AES-256)
- **Navigation** — Open coordinates in your choice of navigation app
- **Dark/Light theme** — Toggle from the menu

---

## 📚 How it works

1. Enter an address and tap Verify
2. All configured geocoding services run in parallel
3. Matt's Pick determines the best location for the address
4. A "Matt's Pick" row shows the recommended coordinates
5. Results are displayed with source markers on the map and an agreement indicator

## ⚙️ Settings

Configure your default navigation app, API keys (stored encrypted), and region override in Settings.

--+

## 📝 Attribution

This product uses the Census Bureau Data API but is not endorsed or certified by the Census Bureau.

Map data © OpenStreetMap contributors.

---

### 📜 Legal / Compliance
- **OSM attribution updated** — Map tiles now link to ODbL copyright page; Esri satellite layer shows full data-source credits
- **User-Agent compliance** — All map data requests use descriptive "MattsVerifier/2.5.0" User-Agent for API policy compliance

