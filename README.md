# Sensing with Spikes — project page

Project website for *Sensing with Spikes: Neuromorphic Optical Tactile Sensor for Contact Force and Position Detection* (IROS 2026).

Plain static HTML: no build step.

## Deploy on GitHub Pages
1. Create a repo (e.g. `sensing-with-spikes`) and push these files to `main`.
2. Repo **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, folder `/ (root)`.
3. The site appears at `https://<user-or-org>.github.io/sensing-with-spikes/`.

## Layout
- `index.html`: the page
- `static/images/`: figures cropped from the paper
- `static/videos/`: short looping clips cut from the supplementary video, plus the full video
- `static/paper.pdf`: the paper

## Deploy on GitLab Pages (private repo, public site)
1. Create a **private** project inside the lab group and push these files to the default branch (`main`).
2. `.gitlab-ci.yml` runs a `pages` job that copies the site into `public/`. Check **Build → Pipelines** to confirm it passed.
3. **Settings → General → Visibility, project features, permissions → Pages**: set to **Everyone**. The repo stays private; only the website is public.
4. **Deploy → Pages** shows the site URL. It is usually `https://<top-level-group>.<pages-domain>/<project>/`.

If **Everyone** isn't offered, the instance admin has Pages access control turned off, or public Pages are disabled at the instance or group level.
