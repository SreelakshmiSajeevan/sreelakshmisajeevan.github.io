# Sreelakshmi Sajeevan — Portfolio

Personal portfolio site, hosted on GitHub Pages at
https://sreelakshmisajeevan.github.io

It's one static page with no build step: `index.html` (HTML, CSS and JS all in one file).

## Files

| File | Purpose |
|---|---|
| `index.html` | The whole site |
| `Sreelakshmi_Sajeevan_CV.pdf` | The file behind the "Download CV" buttons |
| `profile.png` | *(optional)* Your photo for the About section. Use a square image, about 600×600. Until you add one, the site shows "SS" initials. |

## Deploy (replace the current site)

From this folder:

```bash
git clone https://github.com/SreelakshmiSajeevan/sreelakshmisajeevan.github.io.git repo
cp index.html Sreelakshmi_Sajeevan_CV.pdf repo/
# cp profile.png repo/        # if you have a photo
cd repo
git add .
git commit -m "Redesign portfolio"
git push
```

GitHub Pages republishes within a minute or two. You can watch it under the repo's **Actions** tab.

## Preview locally

```bash
python3 -m http.server 8765
```

Then open http://localhost:8765.

## Editing

- **Text and projects:** each project is an `<article class="card project">` block. Copy one to add an app. `data-cat` (`commerce`, `mobility` or `services`) sets which filter it shows under.
- **Store links:** to make a store icon clickable, wrap it in a link, e.g. `<a href="https://play.google.com/store/apps/details?id=..."><i class="fa-brands fa-google-play"></i></a>`.
- **Colours:** change the `--accent` / `--grad` variables at the top of the `<style>` block.
