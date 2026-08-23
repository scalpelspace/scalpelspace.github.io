# scalpelspace.github.io

Home page site for [scalpelspace.com](https://scalpelspace.com).

Technical documentation lives in the separate
[`scalpelspace/docs`](https://github.com/scalpelspace/docs) GitHub pages
repository, served at [docs.scalpelspace.com](https://docs.scalpelspace.com).

## Structure

Plain static HTML and CSS. No build step, no dependencies, no JavaScript.
GitHub Pages serves the repository root as-is (`.nojekyll` disables Jekyll
processing).

```
index.html          Landing page: logo, tagline, Docs/Shop/GitHub cards
products.html       Product overview, deep linking into the docs site
about.html          Company overview and contact details
404.html            Not found page
assets/css/site.css Single stylesheet (light and dark via prefers-color-scheme)
assets/img/         Logo and favicon
CNAME               Custom domain: scalpelspace.com
```

## Local Preview

Any static file server works, for example:

```bash
python -m http.server 8000
```

Then open <http://localhost:8000>.
