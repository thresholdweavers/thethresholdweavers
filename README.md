# 🌿 The Threshold Weavers — Website

**Sacred songs for life's crossings · Paonia, Colorado**

---

## Project Structure

```
threshold-weavers/
│
├── index.html                  ← Home page (main site)
│
├── pages/
│   ├── music.html              ← Songs, recordings & lyrics
│   ├── events.html             ← Upcoming & past events
│   ├── gallery.html            ← Photos & videos
│   └── book.html               ← Booking inquiry form
│
├── css/
│   └── shared.css              ← Fonts, colors, nav, footer — shared by all pages
│
├── js/
│   └── shared.js               ← Cursor, scroll, animations — shared by all pages
│
└── assets/
    ├── images/                 ← All photos go here
    │   └── Threshold_Weavers.jpeg
    ├── audio/                  ← Song recordings (.mp3 or .wav)
    └── video/                  ← Video files (.mp4)
```

---

## How to Update the Site

### ✦ Change colors or fonts
Open `css/shared.css` — all the site's colors and font choices live at the top in `:root { }`.

### ✦ Edit the home page
Open `index.html` — update any text directly in the HTML.

### ✦ Add a new song recording
1. Drop the `.mp3` file into `assets/audio/`
2. Open `pages/music.html`
3. Copy an existing `.song-card` block
4. Fill in the title, description, lyrics
5. Update `<source src="../assets/audio/YOUR-FILE.mp3">`

### ✦ Add a new event
1. Open `pages/events.html`
2. Copy an `.event-card` block under "Upcoming"
3. Fill in the month, day, year, title, location, and description
4. When the event has passed, move it to the "Past Gatherings" section

### ✦ Add photos to the gallery
1. Drop image files into `assets/images/`
2. Open `pages/gallery.html`
3. Copy a `.gallery-item` block
4. Update `src`, `alt`, caption text, and `data-category`
5. Categories: `ceremony` · `gathering` · `portrait` · `video`

### ✦ Add videos to the gallery
1. Drop `.mp4` files into `assets/video/`
2. Use the video template block in `pages/gallery.html` (it's commented out, ready to uncomment)

### ✦ Update the booking email
In `pages/book.html`, update `hello@thresholdweavers.com` to your real email address in two places:
- The `<form action="mailto:...">` attribute
- The contact link at the bottom of the form

### ✦ Use a real contact form (no email client popup)
Sign up free at [formspree.io](https://formspree.io), create a form, and replace the form's `action` attribute in `book.html` with your Formspree URL. Add `method="POST"`.

---

## Fonts Used
- **Lovers Quarrel** — display headings & the logo
- **Alumni Sans Pinstripe** — body text & subheadings
- **Poiret One** — small caps labels & eyebrow text
- **Lato Light** — navigation & UI elements

All fonts load from Google Fonts — no files to manage.

---

## Colors
| Name | Value | Used for |
|------|-------|----------|
| Cream | `#f5f0e8` | Main text |
| Gold | `#c8a96e` | Accents, labels |
| Sage | `#8a9e8c` | Secondary accents |
| Rust | `#b5715a` | Warm accents |
| Midnight | `#1e1a16` | Background |

---

## Hosting on GitHub Pages
1. Push all files to a GitHub repository
2. Go to **Settings → Pages**
3. Set branch to `main`, folder to `/ (root)`
4. Your site will be live at `https://yourusername.github.io/threshold-weavers`

---

*Built with love for The Threshold Weavers — Rebecca, Emily, Aja, Katie & Meghann* 🌿
