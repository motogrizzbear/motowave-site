# MotoWave Site

Public product, support, and privacy site for **MotoWave**, the iPhone internet-radio app.

MotoWave is an iPhone port of [GNOME Shortwave](https://apps.gnome.org/Shortwave/), adapted with a Rust core, UniFFI bridge, and SwiftUI frontend.

The application source stays in the separate private `motogrizzbear/motowave` repository. This repository intentionally contains only public-facing website copy, screenshots, and static assets.

## Structure

```text
motowave-site/
├── index.html
├── support/
│   └── index.html
├── privacy/
│   └── index.html
├── assets/
│   ├── favicon.png
│   ├── site.css
│   ├── theme.js
│   └── screenshots/
│       ├── motowave-iphone-01.png
│       ├── motowave-iphone-02.png
│       ├── motowave-iphone-03.png
│       ├── motowave-iphone-04.png
│       └── motowave-iphone-05.png
├── 404.html
└── .nojekyll
```

## Local preview

No build step or package manager is required.

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## GitHub Pages

GitHub Pages is configured to publish from the `mainline` branch at the repository root.

Expected URLs:

- Product: `https://motogrizzbear.github.io/motowave-site/`
- Support: `https://motogrizzbear.github.io/motowave-site/support/`
- Privacy: `https://motogrizzbear.github.io/motowave-site/privacy/`

Use the support URL for App Store Connect’s **Support URL**, the privacy URL for **Privacy Policy URL**, and the root URL as the optional **Marketing URL**.

## Privacy and maintenance

- No analytics, ads, tracking pixels, forms, accounts, or third-party JavaScript.
- Plain semantic HTML, CSS, and a small local theme script.
- Keep product claims aligned with the private MotoWave app repository and current App Store metadata.
- Support email: `motowave@motobear.dev`.
- Public, non-sensitive bug reports can be filed in this repository’s Issues.
