# Dev Portfolio

> Developer portfolio of Rahmatul Usra (@xsrazy): 16 projects in 7 categories, from platform-style wedding invitations to web tools, stores, and developer utilities.

[![Live](https://img.shields.io/badge/live-dev.xsrazy.web.id-brightgreen)](https://dev.xsrazy.web.id)
[![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)

**Live site: https://dev.xsrazy.web.id**

## About

A single-page portfolio showcasing 16 projects Rahmatul Usra built and shipped: wedding invitations skinned as familiar platforms (Shopee, YouTube, Spotify, WhatsApp, Netflix), web tools and apps, a temp mail service, stores, a recipe site, developer utilities, and a design resource. Every card links out to the project's live site, and every card can also be previewed in place.

The header also links to the author's [GitHub](https://github.com/xsrazy) and [full CV](https://iam.xsrazy.web.id).

## Projects

| Project | Category | Description |
|---|---|---|
| [NikahPee](https://nikahpee.xsrazy.web.id) | Wedding invitations | Shopee-style wedding invitation for Usra & Zee. |
| [NikahTube](https://nikahtube.xsrazy.web.id) | Wedding invitations | YouTube-style wedding invitation, free and open source. |
| [Wedify](https://wedify.xsrazy.web.id) | Wedding invitations | Spotify-style wedding invitation, free and open source. |
| [samaWA](https://samawa.xsrazy.web.id) | Wedding invitations | WhatsApp-style wedding invitation for Usra & Zee. |
| [Nikah](https://nikah.xsrazy.web.id) | Wedding invitations | Classic digital wedding invitation for Usra & Zee. |
| [NikahFix](https://nikahfix.xsrazy.web.id) | Wedding invitations | Netflix-style wedding invitation. |
| [LinkPass](https://linkpass.xsrazy.web.id) | Web tools and apps | Free open-source link-in-bio generator with a digital pass concept. |
| [TikBulk](https://tikbulk.xsrazy.web.id) | Web tools and apps | Bulk TikTok video downloader, no watermark. |
| [Tools](https://tools.xsrazy.web.id) | Web tools and apps | 1,108 free micro tools that run entirely in the browser. |
| [CekTag](https://cektag.xsrazy.web.id) | Web tools and apps | GetContact tag checker for unknown numbers. |
| [TMail](https://tmail.xsrazy.web.id) | Temp mail | Free temporary email, no sign-up, auto-deletes in 24 hours. |
| [myrobs.store](https://myrobs.store) | Store and catalog | Roblox services store. |
| [FMCreators Marketplace](https://fmc.xsrazy.web.id) | Store and catalog | Curated Roblox clothing catalog. |
| [Masakan Kekinian](https://msknkkn.xsrazy.web.id) | Recipes | Recipe discovery site. |
| [GitHub Readme Stats](https://github-readme-stats.xsrazy.web.id) | Developer | Self-hosted GitHub profile card suite: graph, stats, streak, languages, trophy. |
| [ShareCanva](https://sharecanva.com) | Design | Free monthly Canva Pro invite links. |

## Features

- **Dark and light mode.** Toggle button in the header, persisted in `localStorage`, and defaults to the visitor's OS color scheme preference.
- **Category filter.** Filter chips for All (16) and each of the 7 categories, with per-category counts, filtering the grid in place.
- **In-page preview modal.** Every card has a Preview button that opens a floating window with the project's live site inside an iframe. The modal bar shows the project name and domain, an "Open in new tab" link, and a Close button. It also closes on Escape or backdrop click, locks page scrolling while open, and clears the iframe on close.
- **Visit site links.** Every card has a Visit site button that opens the project in a new tab.
- **Custom thumbnails with fallbacks.** 14 projects have custom 1200x900 screenshots in `thumbs/`. If a custom screenshot fails to load, the card falls back to a WordPress mshots snapshot of the live site, then to the site's favicon, then to no image. Thumbnails load lazily.
- **Header stats and responsive grid.** The header shows 16 live projects and 7 categories; cards lay out in a responsive grid that collapses to a single column on narrow screens.

## Architecture

- **Frontend:** a single static `index.html` file with vanilla HTML, CSS, and JavaScript. No build step, no framework, no dependencies.
- **Backend:** none. No server code and no database. Project data lives in a JavaScript array inside `index.html`; cards and the preview modal are rendered client-side.
- **Hosting:** Vercel, at [dev.xsrazy.web.id](https://dev.xsrazy.web.id).

## Files

- `index.html`: the entire portfolio page (markup, styles, project data, filter, theme toggle, preview modal).
- `thumbs/`: 14 custom 1200x900 PNG screenshots, one per project that has one.
- `LICENSE`: MIT license.
- `.github/FUNDING.yml`: sponsorship links.

## Credits

Built by [Rahmatul Usra (@xsrazy)](https://github.com/xsrazy). Full CV: [iam.xsrazy.web.id](https://iam.xsrazy.web.id).

## License

MIT. Copyright (c) 2026 Rahmatul Usra. See [LICENSE](LICENSE).
