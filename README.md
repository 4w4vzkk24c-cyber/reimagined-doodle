# crossedkeys.co

The one-page site of Crossed Keys Co., the house name that signs Zane
Robinson's software.

- `site/` is the whole site: static HTML and CSS, no build step, no script.
  Vercel serves this directory (`vercel.json`).
- `site/fonts/` holds the Fell types, digitally reproduced by Igino Marini,
  under the SIL Open Font License (`site/fonts/OFL.txt`). The files are served
  as distributed; the licence reserves the font names, so do not modify them.

To look at it locally, serve `site/` with any static server, for example
`uv run python -m http.server --directory site 8765`.

`vercel.json` also sends security headers. The content policy allows styles,
fonts and images from this site only, so an inline style, a script, or a file
from another host is blocked until the policy is changed to allow it.

A push to the production branch deploys the site.
