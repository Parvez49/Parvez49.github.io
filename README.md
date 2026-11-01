# parvez49.github.io

Personal portfolio — plain static HTML/CSS, no build step. Live at
https://parvez49.github.io/

## Editing

Everything is in `index.html`. Push to `main` and GitHub Actions
(`.github/workflows/deploy.yml`) publishes it.

## Adding project screenshots / demo videos

1. **Images** — compress to WebP (keep each under ~300 KB) and put them in
   `assets/img/`. Example: `cwebp -q 80 shot.png -o assets/img/victoria-dashboard.webp`
2. **Short clips** — compressed MP4 under ~10 MB in `assets/video/`:
   `ffmpeg -i demo.mov -vcodec libx264 -crf 28 -an assets/video/victoria-demo.mp4`
3. **Long demos** — upload to YouTube (Unlisted) and embed with an iframe.
4. Each project card in `index.html` has a commented-out `<div class="media">`
   block showing all three options — uncomment and point it at the files.

## CVs

PDFs live in `cv/` and are linked from the footer. Source files are in the
`personal_info` repo (`cv/web/`, `cv/mobile/`); re-copy after updating.
