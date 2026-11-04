# The Urban Plate — Restaurant Management System

A complete, single-file restaurant management system with **Customer → Kitchen → Waiter → Customer** order flow.

![Demo](https://img.shields.io/badge/Demo-Live-brightgreen) ![License](https://img.shields.io/badge/License-MIT-blue) ![Tech](https://img.shields.io/badge/Stack-HTML%2FCSS%2FJS-orange)

## ✨ Features

| Role | Capabilities |
|------|-------------|
| **Customer** | Scan QR → Browse menu → Order → Track status (Kitchen → Preparing → Ready → Served) → Pay (Apple Pay / Google Pay / PayPal / Card / Cash) → Loyalty points & offers → Play games while waiting → Review dishes & rate waiters |
| **Waiter** | Accept table requests → View open tables & bills → See ready orders → Mark served → Handle cash payments & calls |
| **Kitchen** | New orders board → Start preparing → Mark ready → Late-order highlighting (15+ min) |
| **Manager** | Sales dashboard (today/week/month) → Menu & photo management → Offers & loyalty config → QR code generator (printable sheets) → Reports & settings |

## 🛠 Tech Stack
- **Single HTML file** — no build step, no dependencies (except QRCode.js via CDN)
- **Vanilla JS** — ES6 modules, localStorage persistence with cross-tab sync
- **CSS Custom Properties** — dark/light themes + custom "warm" theme
- **Responsive** — mobile-first, bottom nav, touch-friendly

## 🚀 Quick Start

### Local
```bash
# Just open the file in a browser
open "restaurant-v11 (1).html"
# or serve locally (avoids CORS for QRCode lib)
npx serve .
```

### Deploy to GitHub Pages
1. Push this repo
2. Settings → Pages → Source: `main` branch → `/ (root)`
3. Live at `https://yourusername.github.io/restaurant-app/`

## 📱 Usage Flow
1. **Manager** prints QR codes for each table (Manager → Tables & QR → Print sheet)
2. **Customer** scans QR → picks table → "Request to open" → gets 4-digit code
3. **Waiter** accepts request → table gets unique code
4. **Customer** orders → goes straight to **Kitchen** (no waiter approval step)
5. **Kitchen** preps → marks Ready
6. **Waiter** sees Ready → marks Served
7. **Customer** tracks live progress → pays → earns loyalty points

## 🎮 Bonus
- **Games**: Memory Match, Tap Challenge, Tic-Tac-Toe (cross-table multiplayer)
- **Reviews**: Dish ratings + comments (only after served)
- **Waiter ratings**: 5-star system per visit
- **Sound alerts**: Role-specific notifications (kitchen chime, waiter ping)

## 📄 License
MIT — free to use, modify, deploy.

---

**Built with ☕ by [oshitha sadew](https://github.com/ozisadew)**