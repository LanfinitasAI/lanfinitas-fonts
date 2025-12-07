# lanfinitas-fonts
official fonts

# Lanfinitas Web Fonts

This repository hosts the official Lanfinitas / CircuLab web fonts bundle in WOFF2 format, plus a shared CSS stylesheet for easy embedding.

All fonts are optimized for web usage and intended to be consumed via GitHub Pages from this repo.

---

## Structure

```text
lanfinitas-fonts/
├── fonts/
│   ├── RamaGothicC-*.woff2
│   ├── RamaGothicE-*.woff2
│   ├── RamaGothicM-*.woff2
│   ├── SpaceMono-*.woff2
│   └── stylesheet.css
└── README.md

fonts/stylesheet.css aggregates all @font-face declarations and serves as the single entry point for external sites and tools.

Usage (HTML)

Once GitHub Pages is enabled for this repository, you can include the fonts in any HTML page via:

<link rel="stylesheet" href="https://lanfinitasai.github.io/lanfinitas-fonts/fonts/stylesheet.css">


Then apply the brand font stack:

<body>
  <h1 style="font-family: 'Rama Gothic E', 'Rama Gothic M', 'Space Mono', system-ui, sans-serif;">
    Lanfinitas Heading
  </h1>
  <p>
    Body text will render with the official Lanfinitas type system, falling back to system fonts if needed.
  </p>
</body>


Functional expectation:
If the stylesheet URL is reachable and the browser supports WOFF2 (all modern browsers do), headings and body text will render using Rama Gothic / Space Mono instead of the default system font.

Usage with Claude Skills and Agents

Claude Skills can emit HTML templates that include:

<link rel="stylesheet" href="https://lanfinitasai.github.io/lanfinitas-fonts/fonts/stylesheet.css">


This ensures that any web-based rendering of those outputs (internal tools, static sites, PDF pipelines using a headless browser, etc.) consistently uses the Lanfinitas brand fonts.

License

Fonts and CSS in this repository are provided solely for Lanfinitas / CircuLab branded materials and approved collaborators.

If you are not part of the Lanfinitas ecosystem, please request permission before using these assets.
