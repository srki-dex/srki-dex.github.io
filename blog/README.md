# Srki Dex Jekyll Blog

Jekyll blog koji se objavljuje na:

https://srki-dex.github.io/blog/

Blog je namerno izolovan u `/blog/`. Postojeći glavni sajt u root-u repozitorijuma nije Jekyll sajt i ne mora da se menja.

## Nova objava

Napravi:

`_posts/YYYY-MM-DD-naziv-teksta.md`

Primer:

```yaml
---
title: "Naslov teksta"
description: "Kratak SEO opis."
date: 2026-08-20 12:00:00 +0200
categories:
  - SEO
tags:
  - google
  - seo
---
```

## Lokalno testiranje

Iz foldera `blog`:

```bash
bundle install
bundle exec jekyll serve --baseurl /blog
```

## GitHub Pages

Root workflow u `.github/workflows/blog-pages.yml` kopira postojeći glavni sajt u deployment folder i zatim gradi samo `blog/` kao Jekyll projekat u `_site/blog/`.

Na taj način finalni GitHub Pages artifact sadrži i postojeći sajt i generisani blog.
