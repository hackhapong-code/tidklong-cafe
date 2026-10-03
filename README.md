# 🌿 ติดคลอง คาเฟ่ (Tid Klong Cafe) — Website & Plugin Blueprint

> **Website Blueprint & Plugins based on Facebook Page:** [https://www.facebook.com/profile.php?id=100057527526785](https://www.facebook.com/profile.php?id=100057527526785)  
> **Location:** ซอยบางจาก 19 ตำบลเชิงเนิน อำเภอเมืองระยอง จังหวัดระยอง 21000  
> **Contact:** 080-576-8179 / 094-850-1553  
> **Hours:** อังคาร – อาทิตย์ 09:00 – 17:00 น. (ปิดวันจันทร์)

---

## 1. Antigravity AI Assistant Plugins Installed

To equip Antigravity with full design and local business intelligence for building, iterating, and maintaining this website, the following plugins have been validated and installed via `agy plugin install`:

| Plugin Name | Components | Purpose |
| :--- | :--- | :--- |
| **`ui-ux-pro-max`** | Skills, Palettes, Rules, Typography | Local design intelligence database (79 styles, 192 product palettes, 74 font pairings, responsive layout rules, cafe/restaurant UX patterns). |
| **`frontend-design`** | Skills, Aesthetic Engine | Anthropic's distinctive frontend design intelligence ensuring handcrafted, anti-generic visual identity tailored specifically to wooden riverside cafes. |
| **`local-seo`** | `seo-local`, `seo-maps`, `seo-schema` | Local SEO optimization, Google Maps Pack ranking, and `CafeOrCoffeeShop` Schema markup for local discovery in Rayong. |

### Verification:
```bash
agy plugin list
```
Output:
```json
{
  "imports": [
    { "name": "ui-ux-pro-max", "components": ["skills"] },
    { "name": "frontend-design", "components": ["skills"] },
    { "name": "local-seo", "components": ["skills"] }
  ]
}
```

---

## 2. Production Website Plugins (WordPress / Web CMS Suite)

If deploying this cafe's web presence on a content management system (such as WordPress), the following 6 plugins are specifically required to match the Facebook page operations:

1. **Smash Balloon Social Post Feed (Custom Facebook Feed)**
   - *Purpose:* Automatically pulls daily cafe updates, seasonal drink announcements, and photos directly from `https://www.facebook.com/profile.php?id=100057527526785` so the website stays fresh without double-posting.
2. **WP Social Chat / Joinchat (Facebook Messenger Floating Button)**
   - *Purpose:* Direct customer messaging via Facebook Messenger (`m.me/100057527526785`) and phone (`080-576-8179`) for directions, pet-friendly policy queries, and table availability.
3. **Five Star Restaurant Menu / WP Cafe**
   - *Purpose:* Responsive categorized digital menu for Slow Bar Drip Coffee, cold drinks, homemade bakery, and Thai single-dish meals with prices and dietary tags.
4. **WP Cafe Reservation / Restaurant Reservations**
   - *Purpose:* Allows customers to prepare table reservation requests for waterfront and garden zones.
5. **WP Go Maps / Leaflet Map**
   - *Purpose:* Interactive map pinned at Bang Chak Soi 19, Choeng Noen, Rayong with a one-tap "Get Directions" trigger for Google Maps mobile navigation.
6. **Rank Math SEO (with Local SEO Module)**
   - *Purpose:* Generates `LocalBusiness` / `CafeOrCoffeeShop` JSON-LD schema with exact opening hours (Tue-Sun 09:00-17:00), phone numbers, and Rayong geo-coordinates to capture "คาเฟ่ระยอง" and "ร้านกาแฟริมคลอง" searches.

---

## 3. Online Table Reservation Request System

The website includes a bilingual (`index.html` TH / `en.html` EN) reservation request builder tailored to the cafe's layout and operating schedule:
- **4 Authentic Seating Zones:**
  1. *ศาลาไม้จิกน้ำริมคลอง (Waterfront Sala Pavilion)*
  2. *โซนโกงกางริมน้ำ (Mangrove Riverside Bar)* — Showcased with 3 authentic zone photos
  3. *ซุ้มระเบียงไม้ล้อเกวียน (Rustic Covered Terrace)*
  4. *ลานสวนร่มไม้ธรรมชาติ (Shaded Outdoor Garden)*
- **Operating Hours & Time Slots:**
  - Automated Monday detection: Alerts customers that the cafe is closed on Mondays and guides them to select Tuesday – Sunday.
  - 16 selectable 30-minute arrival intervals (`09:00` – `16:30`) plus a custom arrival time picker (`09:00` – `16:45`) with no fixed seating duration limit.
- **Device-Only Request Storage (`localStorage`):**
  - Submitting the form saves a draft request on the user's device only (`tidklong_bookings`, status `request_awaiting_staff_confirmation`) and **does not transmit anything to the cafe automatically**.
  - Explicitly labeled in both Thai and English as a local request awaiting staff confirmation, not a confirmed reservation.
- **Facebook Messenger Handoff & Prefill Caveat:**
  - Generates a reference ID (`#TK-XXXX`) and populates `https://m.me/100057527526785?text=...` with the URL-encoded request details.
  - **Messenger Prefill Caveat:** Opening the `m.me` link redirects (`HTTP 302`) to Facebook Messenger (`facebook.com/msg/...`). It does not send a booking automatically—the customer must be signed into Facebook/Messenger and manually send the message for staff to receive and confirm the request. On some desktop browsers requiring a fresh login redirect, Facebook may not preserve the `?text=` prefill parameter across authentication.

---

## 4. Production Deployment, Domain Status & QA Verification

### Primary Public URLs
- **Primary Public URL (Thai):** [https://canalbound.vercel.app/](https://canalbound.vercel.app/)
- **Primary Public URL (English):** [https://canalbound.vercel.app/en.html](https://canalbound.vercel.app/en.html)
- **Additional Active `.vercel.app` Aliases:**
  - `https://ติดคลองคาเฟ่.vercel.app/` (`https://xn--42cai4ce8dwb2d4bn3l2d.vercel.app/`)
  - `https://tidklong-cafe.vercel.app/`
  - `https://canal-bound.vercel.app/`
- **GitHub Pages Mirror:**
  - Thai: [https://hackhapong-code.github.io/tidklong-cafe/](https://hackhapong-code.github.io/tidklong-cafe/)
  - English: [https://hackhapong-code.github.io/tidklong-cafe/en.html](https://hackhapong-code.github.io/tidklong-cafe/en.html)
- **Source Deployment Commit:** `5321a041c6fbe2276a95711f3ddc42e13c214338` (`main` on [hackhapong-code/tidklong-cafe](https://github.com/hackhapong-code/tidklong-cafe))

### Domain & Security Status
- **Unpaid `.com` Domain Status:** `ติดคลองคาเฟ่.com` (`xn--42cai4ce8dwb2d4bn3l2d.com`) remains **unregistered and unpaid** (`No match for domain` in WHOIS). No domain purchases or charges were made.
- **Security Settings:** Vercel project deployment protection (`--sso`) and account permissions remain enabled and unchanged.

### Actual QA Evidence
- **Live Bilingual Verification:** Independently verified in-browser on `https://canalbound.vercel.app/` and `https://canalbound.vercel.app/en.html`; both pages render the updated request-only wording and pass JS syntax/source parsing.
- **DOM XSS Hardening Regression:** All dynamic booking rendering in `#modalSummaryBox` and `#myBookingsList` uses `document.createElement(...)`, `.textContent`, and `.replaceChildren(...)` (`0` `.innerHTML` occurrences in `index.html` and `en.html`). Tested against hostile payloads (`<img src=x onerror=...>`, `<script>`, `<svg onload=...>`, `<iframe>`) with `xssTriggered: false` and `0` injected elements.
- **Corrupted `localStorage` Recovery:** Verified `readStoredBookings()` with malformed JSON (`"{bad_json[["`) and non-array payloads (`{"not":"an array"}`); corrupted entries are automatically cleared (`null`) and recover cleanly to the empty state with `0` console/page errors.
- **Mobile Layout (`390x844`):** Verified `0px` horizontal overflow (`scrollWidth === innerWidth`) and `0` failed asset requests across both Thai and English pages.
