# scalpelspace.github.io

Home page site for [scalpelspace.com](https://scalpelspace.com).

Technical documentation lives in the separate
[`scalpelspace/docs`](https://github.com/scalpelspace/docs) GitHub pages
repository, served at [docs.scalpelspace.com](https://docs.scalpelspace.com).

## Structure

Plain static HTML and CSS. No build step and no dependencies. GitHub Pages
serves the repository root as-is (`.nojekyll` disables Jekyll processing).

The only JavaScript on the site is an inline snippet in `products.html` that
powers the product search box. Everything else, including the tag filter, is
pure CSS. With scripting disabled the search field is hidden and every product
still lists and filters normally.

```
index.html            Landing page: logo, tagline, Docs/Shop/GitHub cards
products.html         Searchable, filterable product grid
products/<codename>/  One page per product, slugs matching the docs site
about.html            Company overview and contact details
404.html              Not found page
assets/css/site.css   Single stylesheet (light and dark via prefers-color-scheme)
assets/img/           Logo and favicon
sitemap.xml           Sitemap, listing every product page
CNAME                 Custom domain: scalpelspace.com
```

Product slugs match `docs.scalpelspace.com/products/<codename>/`, so
`/products/momentum/` here pairs with the same path on the docs site.

## Local Preview

Any static file server works, for example:

```bash
python -m http.server 8000
```

Then open <http://localhost:8000>.
