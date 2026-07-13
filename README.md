# Koty & Lolty — Our Little Forever 💕

A romantic keepsake website for **Abdullah & Aisha (Koty & Lolty)** — together since 12 June 2025.

## What's inside
- `index.html` — the website
- `assets/` — all your photos and videos

Keep `index.html` and the `assets` folder **together** in the same folder. Don't rename anything.

## How to put it online for FREE (easiest first)

### Option 1 — Netlify Drop (no account needed, ~1 minute) ⭐ recommended
1. Go to **https://app.netlify.com/drop**
2. Drag the **whole folder** (the one containing `index.html` and `assets`) onto the page.
3. Wait a few seconds — you get a free live link like `https://something.netlify.app`.
4. (Optional) Make a free account to rename it to something like `koty-and-lolty.netlify.app`.

### Option 2 — Tiiny.host
1. Go to **https://tiiny.host**
2. Zip the folder and upload the zip (the included `koty-lolty-website.zip` works directly).
3. Pick a free subdomain and publish.

### Option 3 — GitHub Pages (free, keeps it forever)
1. Create a free account at **https://github.com**
2. Make a new repository, upload `index.html` and the `assets` folder.
3. In the repo: **Settings → Pages → Deploy from branch → main → /(root) → Save**.
4. Your site appears at `https://yourusername.github.io/repo-name/`.

## Want a custom name like koty-lolty.com?
The hosts above give a free `.netlify.app` / `.github.io` address. A custom `.com` costs a little (usually a few dollars/year) at Namecheap, GoDaddy, or Cloudflare, and you can point it to the free hosting above.

## Visit tracking 👀
The site quietly logs every page open to your Firebase project (`our-corner-a8019`, collection `visits`): who, when, and how many minutes they stayed (only time the tab was actually visible counts).

- **Who is who:** share personalized links — e.g. send her `https://your-site/?v=lolty` and open it yourself as `?v=koty`. The name is remembered on that device, so later plain visits are still tagged. Visits without a name show as `unknown`.
- **See the results:** open `stats.html` on the site (e.g. `https://your-site/stats.html`). It shows per-person totals and every visit with date, minutes, and device.
- **Firestore rules:** the `visits` collection must be readable/writable, same as `messages`:
  ```
  match /visits/{doc} { allow read, write: if true; }
  ```
- **Heads-up:** `stats.html` has no password — anyone who knows the URL can see it. Rename the file to something unguessable if you want it more private.

## Tip
Videos are large (~19 MB total). On the free hosts above that's totally fine. If a video ever loads slowly, that's just the file size — give it a moment.

Made with love. ❤️
