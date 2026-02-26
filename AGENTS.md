# AGENTS.md

## Cursor Cloud specific instructions

This is a static single-page school website ("SMA Negeri Harapan Bangsa") consisting of a single `index.html` file. It uses Tailwind CSS loaded via CDN — no build step, no package manager, no backend.

### Running the website

Serve the file with any static HTTP server:

```
python3 -m http.server 8080
```

Then open `http://localhost:8080` in a browser.

### Key caveats

- **Internet required**: Tailwind CSS is loaded from `cdn.tailwindcss.com`. Without internet the page renders unstyled.
- **No tests / linter / build**: There is no `package.json`, no test suite, and no linting configuration. Validation is done by visual inspection in a browser.
- **No dependencies to install**: The update script is a no-op (`echo "No dependencies"`).
