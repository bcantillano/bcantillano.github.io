# Portfolio hub documentation

## Purpose

This repository (`bcantillano.github.io`) is the **user GitHub Pages site** served at:

`https://bcantillano.github.io/`

It is the main portfolio hub. Individual projects keep their own repos and, when enabled, their own project Pages sites. The hub links out to those sites with normal HTML anchors.

## Linking to Character OS

Character OS is a separate repository with GitHub Pages enabled. Its public URL is:

`https://bcantillano.github.io/character-os/`

From this hub, links use that absolute URL, for example:

```html
<a href="https://bcantillano.github.io/character-os/">Open Character OS</a>
```

That works because GitHub Pages sites can link to any public URL. Project Pages do not need to live inside this repo.

### URL pattern reminder

| Site type | Repo name pattern | URL |
| --- | --- | --- |
| User site (this repo) | `username.github.io` | `https://username.github.io/` |
| Project site | any other repo with Pages | `https://username.github.io/repo-name/` |

## Cleanup decisions

Old course lab folders (`lab_5`, `lab_6_ajax`, `lab_7`, `lab_8`, `Assignment 1`) and local junk (`.DS_Store`, `.Rhistory`) were removed so this repo only hosts the portfolio hub.

## Site structure

```
index.html              # Portfolio hub page
assets/portfolio.css    # Hub styles
assets/hero.svg         # Full-bleed hero atmosphere
DOCUMENTATION.md        # This file
```

## Design direction

- **Role:** personal brand gateway, not a project case study.
- **Look:** signal desk — cool stone ground, vermillion accent, Fraunces (display) + Sora (body). Distinct from Character OS’s mist/teal case-study theme.
- **Hero:** brand name as the primary signal; one headline, one lede, CTA group, full-bleed visual.
- **Projects:** list of outbound links (Character OS case study + GitHub source). Add more `<li>` entries as other project Pages or repos are ready.

## Adding another project link

1. Prefer a project Pages URL when the repo has Pages enabled.
2. Otherwise link to the GitHub repository.
3. Add a new list item under `#work` in `index.html` using the same `project-link` markup.

## Publishing

Push to the branch that GitHub Pages uses for this user site (typically `master` / `main`). After merge, the hub updates at `https://bcantillano.github.io/`.
