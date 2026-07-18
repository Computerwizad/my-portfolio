# Portfolio

Static, dependency-free portfolio site (HTML/CSS/JS). No build step.

## Run it in Codespaces

```bash
python3 -m http.server 8080
```
Then open the forwarded port 8080, or just use the "Go Live" / Live Preview extension.

## Deploy free (GitHub Pages)

1. Push this repo to GitHub.
2. Repo → Settings → Pages → Source: `main` branch, `/root`.
3. Your site will be live at `https://<username>.github.io/<repo>`.

## Before you publish — personalize these

- [ ] `assets/portrait.jpg` — add a real photo, then swap the `.portrait-placeholder`
      div in `index.html` for `<img src="assets/portrait.jpg" alt="Dickie">`
- [ ] Contact section (`index.html`, bottom) — real email + LinkedIn URL
- [ ] Project links — confirm `github.com/Computerwizad/mulla` is public, or
      point it at whichever repo you want visible
- [ ] "Faceless Channel" project — add a real link once the channel is live
