# velynox.de

Personal website. Static HTML, TailwindCSS via CDN, no build step, no framework.

## Structure

```
velynox.de/
├── index.html      # markup
├── css/
│   └── style.css   # custom styles (scrollbar, selection, font baseline)
└── js/
    └── main.js     # reserved for future lightweight interactivity
```

## Stack

- HTML5
- [TailwindCSS](https://tailwindcss.com) (CDN, config inlined in `index.html`)
- [JetBrains Mono](https://www.jetbrains.com/lp/mono/) via Google Fonts
- [Catppuccin Mocha](https://github.com/catppuccin/catppuccin) color palette
- Inline SVGs from [Lucide](https://lucide.dev) / [Feather Icons](https://feathericons.com)

## Design

See [`../DESIGN.md`](../DESIGN.md) for the full visual spec.

Key rules:
- No emojis in the UI — inline SVGs only
- Monospace everywhere (JetBrains Mono)
- Catppuccin Mocha palette, no deviations
- `max-w-3xl` centered layout

## Development

No build step required. Open `index.html` directly in a browser, or serve it:

```bash
php -S localhost:8080
# or
python3 -m http.server 8080
```

## Deployment

Deployed to [velynox.de](https://velynox.de) from the `main` branch.
Active development happens on `dev`.

## License

MIT
