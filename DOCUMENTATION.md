# Portfolio hub documentation

## Purpose

This repository (`bcantillano.github.io`) is the **user GitHub Pages site** served at:

`https://bcantillano.github.io/`

It is the main portfolio hub. Individual projects keep their own repos and, when enabled, their own project Pages sites. The hub links out to those sites with normal HTML anchors.

## Linked projects

### CrowdPleaser

Live product site (external domain):

`https://www.crowdpleaser.io`

Linked from the hero CTA and the Projects list:

```html
<a href="https://www.crowdpleaser.io">Open CrowdPleaser</a>
```

CrowdPleaser is an event app for hosts and guests (song requests via Spotify,
invitations, iOS + web join flows). It is hosted outside this repo.

Tech badges shown on the project row: Swift, Spring Boot, Java, React, Spotify API.

### Character OS

Character OS is a separate repository with GitHub Pages enabled. Its public URL is:

`https://bcantillano.github.io/character-os/`

From this hub, links use that absolute URL, for example:

```html
<a href="https://bcantillano.github.io/character-os/">Open Character OS</a>
```

Tech badges shown on the project row: Python, ChatGPT.

That works because GitHub Pages sites can link to any public URL. Project Pages
and external product sites do not need to live inside this repo.

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
assets/portrait.jpg     # Smaller hero portrait (replace anytime)
assets/hero.svg         # Optional abstract atmosphere (unused)
DOCUMENTATION.md        # This file
```

## Design direction

- **Role:** personal brand gateway, not a project case study.
- **Look:** signal desk — cool stone ground, vermillion accent, Fraunces (display) + Sora (body). Distinct from Character OS’s mist/teal case-study theme.
- **Hero:** brand name as the primary signal; one headline, one lede, CTA group, plus a smaller discrete portrait beside the copy (not a full-bleed background).
- **Skills:** Core skills section mirrored from the resume (languages through AI tools), placed before Projects.
- **Projects:** CrowdPleaser and Character OS, each with compact tech badges beside the title.

## Updating the portrait

Replace `assets/portrait.jpg` with a newer image (same filename, or update the `src` in `index.html`).

## Adding another project link

1. Prefer a live product URL or project Pages URL when available.
2. Otherwise link to the GitHub repository.
3. Add a new list item under `#work` in `index.html` using the same `project-link` markup, including a `tech-badges` group next to the title.

## Publishing

Push to the branch that GitHub Pages uses for this user site (typically `master` / `main`). After merge, the hub updates at `https://bcantillano.github.io/`.
