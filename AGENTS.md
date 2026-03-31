# Noor Labs Website

Static HTML/CSS marketing site for Noor Labs halal wellness brand.

## Cursor Cloud specific instructions

### Project structure
- `index.html` — single-page landing site
- `styles.css` — all styles (CSS custom properties, responsive layout)
- No build step, no JavaScript framework, no backend

### Development server
```bash
npm run dev          # starts 'serve' on port 3000
```

### Linting
```bash
npm run lint         # runs both HTML and CSS linters
npm run lint:html    # htmlhint on index.html
npm run lint:css     # stylelint on all CSS files
```

### Notes
- The `media-feature-range-notation` stylelint rule is disabled in `.stylelintrc.json` because the existing CSS uses prefix notation (`max-width: 720px`) rather than range notation.
- Google Fonts CDN link in `index.html` loads Playfair Display; the site gracefully degrades to Georgia/serif if offline.
