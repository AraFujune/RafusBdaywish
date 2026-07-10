# Happy Birthday, My Love 💌

A one-page, romantic birthday site for your wife — a wax-seal envelope that opens into a love letter, a timeline of your story, and a photo gallery. Pure HTML/CSS/JS, no build step, free to host on GitHub Pages.

## 1. Personalize the content

Open `index.html` in any text editor and search for `EDIT:`. Every spot that needs your own words is marked this way, and the visible placeholder text is wrapped in `[ brackets ]` so it's easy to spot. Replace the bracketed text with your own — her name, your letter, your memories, captions — and delete the brackets.

Sections you'll edit:
- **Hero** — her name + one line under the headline
- **Love Letter** — salutation, 3 paragraphs, sign-off
- **Timeline** — 4 memory entries (date, title, short text). Copy/paste the `<div class="t-item">...</div>` block to add more.
- **Gallery** — 6 photo captions
- **Footer** — closing line + your name

## 2. Add your photos

Put your images inside the `images` folder using these exact filenames:

```
images/photo-1.jpg
images/photo-2.jpg
images/photo-3.jpg
images/photo-4.jpg
images/photo-5.jpg
images/photo-6.jpg
```

Any image format works (`.jpg`, `.png`, `.webp`) — just update the `src` in `index.html` to match if you use a different extension. Square-ish photos (close to 1:1) look best in the polaroid frames. If a file is missing, that frame will just show its filename as a placeholder instead of breaking, so you can see at a glance what's left to add.

## 3. Preview it locally

Just double-click `index.html` to open it in your browser. No server needed.

## 4. Publish to GitHub Pages

1. Create a new **public** repository on GitHub (e.g. `happy-birthday`).
2. Upload `index.html` and the `images` folder to it (drag-and-drop on the GitHub website works fine, or use git).
3. Go to the repo's **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`. Save.
5. Wait a minute, then your site will be live at:
   ```
   https://<your-github-username>.github.io/<repo-name>/
   ```
6. Send that link to your wife on her birthday 🎂

## Notes

- The falling petals and reveal animations respect `prefers-reduced-motion`, so it stays graceful on any device.
- Everything is in one file (`index.html`) — no dependencies to install, just the two Google Fonts loaded from a CDN.
