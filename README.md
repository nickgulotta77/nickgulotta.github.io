# Nick Gulotta — personal site

A 5-page static site (Home, Research, Publications, Popular Press, Contact) built in plain HTML/CSS/JS — no build step, ready for GitHub Pages.

## Publish it on GitHub Pages (free)

1. Create a new **public** repository on GitHub — e.g. `nickgulotta.github.io` (using that exact name gives you the cleanest URL) or any name like `lab-site`.
2. Upload all the files in this folder (`index.html`, `research.html`, `publications.html`, `press.html`, `contact.html`, `styles.css`, `script.js`) to the root of the repo — either drag-and-drop on github.com or via `git push`.
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment," set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`. Save.
5. GitHub gives you a live URL within a minute or two:
   - `https://<username>.github.io/` if the repo is named `<username>.github.io`
   - `https://<username>.github.io/<repo-name>/` otherwise

## Before you publish

- **Popular Press links**: most links on the Press page are placeholders (`#`) since the source CV listed "link" without the actual URL — open `press.html` and swap in the real article URLs.
- **Photos**: there are currently no photos. If you'd like a headshot or field photos, add an `images/` folder and drop `<img>` tags into `index.html` or `contact.html`.
- **Google Scholar / ORCID**: add a link in `contact.html` or `publications.html` if you'd like one.
- **Custom domain** (optional, ~$15/yr from any registrar): add a `CNAME` file with your domain, then point your registrar's DNS at GitHub's IPs — GitHub's Pages docs walk through this under Settings → Pages → Custom domain.

## Editing content later

Everything is plain HTML — no templating engine. Each page repeats the same sidebar markup, so if you rename a nav tab or change contact info, update it in all five `.html` files (or ask Claude to do it for you).
