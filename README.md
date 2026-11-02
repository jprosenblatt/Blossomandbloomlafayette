# Marci Rosenblatt · Floral Designer

A one-page contact card for Marci's floral design work. It's plain HTML and CSS with no build step, so GitHub Pages can serve it as is.

| File | What it is |
| --- | --- |
| `index.html` | The page: name, intro, services, and the contact card |
| `styles.css` | Colors (sampled from her arrangement photo), type, layout, motion |
| `marci-rosenblatt.vcf` | The "Save to contacts" card, with her photo, phone, email and Instagram |
| `images/arrangement-*.webp` | Her arrangement photo, extended to portrait for the arch frame |
| `images/og-image.jpg` | The preview shown when the link is texted or posted |
| `favicon.svg`, `images/apple-touch-icon.png` | Browser tab and home-screen icons |

## Preview locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Publish on GitHub Pages

1. The code lives at https://github.com/jprosenblatt/Blossomandbloomlafayette. To connect a local copy and push:

   ```bash
   git remote add origin https://github.com/jprosenblatt/Blossomandbloomlafayette.git
   git push -u origin main
   ```

2. In the repo on GitHub, go to **Settings → Pages**, set **Source** to *Deploy from a branch*, and pick `main` and `/ (root)`.
3. After a minute or so the site is live at https://jprosenblatt.github.io/Blossomandbloomlafayette/.

If the repo is renamed or you add a custom domain, update `og:url` and `og:image` near the top of `index.html` so link previews keep working.

## Common edits

- **Business name:** change the `<h1>`, the `<title>` and `og:title` in `index.html`, the `FN`/`N` lines in `marci-rosenblatt.vcf`, and the footer.
- **Contact details:** the phone number appears in the `tel:` and `sms:` links and the visible number in `index.html`, and in the `TEL` line of the `.vcf`. Email and Instagram work the same way.
- **Colors:** all defined at the top of `styles.css`.
