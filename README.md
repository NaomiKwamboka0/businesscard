# Naomi Kwamboka — Business Card (Nude + Gold)

Two files, one card.

## Files

- **`index.html`** — the digital business card. Nude + gold palette, flippable on click, prints clean. Contains the QR code.
- **`choose.html`** — the landing page the QR code opens. Two cards: **View My CV** and **See My Projects**.
- **`cv.pdf`** — *(you add this)* drop your CV PDF into this folder with this exact filename so the "View My CV" button works.

## How the QR code works

The QR encodes a single URL — the public address of `choose.html`. When someone scans it, they land on the choice page and pick CV or Projects.

Right now the QR points to:

```
https://naomikwamboka0.github.io/n8n-Profile/choose.html
```

So you have two options:

### Option A — host on your existing GitHub Pages site (recommended)
1. Copy `choose.html` and `cv.pdf` into your `n8n-Profile` repo root.
2. Push. The QR will work as-is.

### Option B — host this folder separately
1. Push this whole folder to a new GitHub repo, enable Pages.
2. Open `index.html`, find the line near the bottom:
   ```js
   const CHOICE_PAGE_URL = "https://naomikwamboka0.github.io/n8n-Profile/choose.html";
   ```
   Change it to your new `choose.html` URL.
3. Reload `index.html` — the QR regenerates automatically.

## Open it locally

Just double-click `index.html`. Click the card to flip it. Use the "Print card" button to print or save as PDF.

## Colors

| Token | Hex |
|---|---|
| Nude light | `#F5E6D8` |
| Nude | `#E8D2B8` |
| Nude deep | `#C9A876` |
| Gold | `#C9A227` |
| Gold soft | `#D4AF37` |
| Gold dark | `#8B6914` |
| Ink | `#2B1B0E` |

Change them in one place — the `:root` block at the top of either HTML file.
