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
2. **WP Social Chat / Joinchat (Facebook Messenger & LINE Floating Button)**
   - *Purpose:* Thai cafe customers prefer quick messaging for directions, pet-friendly policy queries, and table availability.
3. **Five Star Restaurant Menu / WP Cafe**
   - *Purpose:* Responsive categorized digital menu for Slow Bar Drip Coffee, cold drinks, homemade bakery, and Thai single-dish meals with prices and dietary tags.
4. **WP Cafe Reservation / Restaurant Reservations**
   - *Purpose:* Allows customers to request or reserve prime waterfront seats, especially during weekend peak hours.
5. **WP Go Maps / Leaflet Map**
   - *Purpose:* Interactive map pinned at Bang Chak Soi 19, Choeng Noen, Rayong with a one-tap "Get Directions" trigger for Google Maps mobile navigation.
6. **Rank Math SEO (with Local SEO Module)**
   - *Purpose:* Generates `LocalBusiness` / `CafeOrCoffeeShop` JSON-LD schema with exact opening hours (Tue-Sun 09:00-17:00), phone numbers, and Rayong geo-coordinates to capture "คาเฟ่ระยอง" and "ร้านกาแฟริมคลอง" searches.

---

## 3. Online Table Reservation & Booking System

The website includes an interactive online booking system tailored to the cafe's physical layout and operating schedule:
- **3 Visual Seating Zones:**
  1. *ระเบียงชานไม้ริมคลอง (Waterfront Deck)* — Prime photo & feet-dangling spot overlooking Bang Chak canal.
  2. *เรือนไม้โบราณวินเทจ (Vintage Heritage House)* — Shaded, peaceful indoor seating under vintage wooden beams.
  3. *สวนใต้ร่มไม้โกงกาง (Mangrove Garden)* — Outdoor family & group seating under lush trees.
- **Operating Hours Rules:**
  - Automated Monday detection: Alerts customers that the cafe is closed on Mondays and guides them to select Tue–Sun.
  - Time slots from 09:30 to 16:00 (closing at 17:00).
- **Instant Facebook Messenger & LINE Handoff:**
  - Generates a formatted reservation code (`#TK-XXXX`).
  - Pre-populates a direct message link to the cafe's Facebook Messenger (`https://m.me/100057527526785?text=...`) for instant zero-friction confirmation.
- **Local Client-Side Storage:**
  - Persists active reservations in `localStorage` so customers can view their upcoming bookings.

---

## 4. Local Web Prototype & Live Server

- **Live URL:** [http://localhost:8088#booking](http://localhost:8088#booking)
- **Source File:** `index.html` (Tailwind CSS, Google Fonts Prompt/Sarabun, Lucide icons, LocalBusiness Schema JSON-LD).

