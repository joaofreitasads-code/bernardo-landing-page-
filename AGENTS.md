# bernardo-landing-page-

A single-file, static marketing landing page (Portuguese / pt-BR) for the digital
product "Método Constância com Deus". The page is plain **HTML5 + inline CSS + inline
vanilla JavaScript** — there is no build system, package manager, framework, backend, or
database.

## Cursor Cloud specific instructions

### Services / structure
- This is a **static site** consisting of a single `index.html` file. There are no
  dependencies to install and nothing to build or compile.
- Note: the product file `index.html` currently lives on the feature branch
  `cursor/add-constancia-landing-7fbf`, not on `main` (which only has this `AGENTS.md`
  and `README.md`). When working on the page, make sure `index.html` is present in the
  working tree (it may need to be brought in from that branch).

### Running it (development)
- Serve the directory with any static file server and open it in a browser, e.g.
  `python3 -m http.server 8000` (Python 3.12 and Node 22 are available), then visit
  `http://localhost:8000/`. Opening `index.html` directly via `file://` also works.
- There is **no lint, test, or build step** — the only "run" step is serving the static file.

### Gotchas
- The page references external resources (Google Fonts, an `i.imgur.com` image, and a
  WhatsApp deep link). These require internet access but are non-blocking: the page renders
  with serif fallback fonts and remains fully functional offline.
- CTA buttons currently use placeholder links (`href="#"` / `#oferta`); there is no real
  checkout/backend integration to run.
