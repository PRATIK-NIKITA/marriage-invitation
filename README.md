# प्रतीक ♡ निकिता — Wedding Invitation

A beautiful, mobile-first Maharashtrian wedding invitation built as a single self-contained HTML file. Hosted on GitHub Pages.

## Live Site

```
https://YOUR_USERNAME.github.io/pratik-nikita
```

---

## Features

- Marathi language throughout
- Traditional Maharashtrian color palette — deep maroon, saffron, gold
- Lotus SVG + Om symbol with glow animation
- Tap-to-open splash screen
- Background music (embedded as base64, no external file needed)
- Rose petal shower animation (30 petals, 6 drift paths)
- Live countdown timer in Devanagari numerals
- Event timeline — हळद, स्नेहभोजन, विवाह सोहळा
- Clickable Google Maps link for venue
- Tap-to-call contact numbers
- Family section — वधू पक्ष & वर पक्ष
- Mobile-first, max-width 450px
- Single HTML file — no framework, no build step

---

## Wedding Details

| | |
|---|---|
| **वर** | चि. प्रतीक (सौ. दिपाली व डॉ. कैलास माणिकराव चौधरी यांचे कनिष्ठ सुपुत्र, मोयखेडा दिगर, ता. जामनेर, जि. जळगाव) |
| **वधू** | चि. सौ. कां. निकिता (सौ. ज्योती व श्री. राजेंद्र वसंतराव राऊत यांची कनिष्ठ सुकन्या, रा. पांगरखेड ह. मु. मेहकर जि. बुलढाणा) |
| **दिनांक** | शनिवार, १२ डिसेंबर २०२६ |
| **मुहूर्त** | गोरज मुहूर्त सायं. ६:४५ वा. — मार्गशीर्ष शुद्ध तृतीया, शके १९४८ |
| **विवाह स्थळ** | कृषी वैभव लॉन्स, डोणगाव रोड, मेहकर, जि. बुलढाणा |
| **हळद व स्नेहभोजन** | शुक्रवार, ११ डिसेंबर २०२६ — मोयखेडा दिगर, ता. जामनेर (हळद स. १० वा., स्नेहभोजन दु. १२ पासून) |

---

## File Structure

```
InVitation/
├── index.html   # Entire site — styles, content, audio (base64), JS
└── README.md
```

The MP3 is embedded as a base64 data URL inside `index.html` so there are no external dependencies.

---

## Deploy to GitHub Pages

```bash
# First time
git init
git add index.html README.md
git commit -m "Add wedding invitation"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/pratik-nikita.git
git push -u origin main
```

Then: **GitHub repo → Settings → Pages → Branch: main / root → Save**

Site goes live at `https://YOUR_USERNAME.github.io/pratik-nikita` within ~60 seconds.

```bash
# Every update after that
git add index.html
git commit -m "describe change"
git push
```

---

## Customisation

All edits are in `index.html`. Key locations:

| What | Search for |
|---|---|
| Wedding date (countdown) | `new Date('2026-12-12T18:45:00+05:30')` |
| Couple names | `चि. प्रतीक` / `चि. सौ. कां. निकिता` |
| Muhurta date & time | `गोरज मुहूर्त सायं. ६.४५ वा.` |
| Venue | `कृषी वैभव लॉन्स` |
| Contact numbers | `tel:+919421513709` |
| Background music | `<audio id="weddingAudio"` — base64 Shehnai music |
| Family & Nimantrak | `familySection` |

---

## Tech

- Vanilla HTML / CSS / JS — zero dependencies
- [Noto Serif Devanagari](https://fonts.google.com/noto/specimen/Noto+Serif+Devanagari) via Google Fonts
- CSS `@keyframes` for petals and animations
- Base64-embedded MP3 audio
- Hosted free on GitHub Pages
