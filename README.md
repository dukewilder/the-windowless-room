# The Windowless Room

The landing page for *The Windowless Room: On the Unintelligibility of Theism*
by Dylan Allman. Public domain, CC0.

The page is the cover standing up. The room is drawn live in SVG from the
printed cover's own measurements: the ceiling arms falling into the corner, the
skirting rising out of it, the floorboards running from a vanishing point set
between the two. The cross and the table are the cover's, traced off the
artwork itself.

## What is here

```
index.html               the whole site, one file, no external requests
404.html                 not-found page
og.png                   1200x630 social card
favicon.svg              vase, 64 viewBox
favicon.ico              16, 32, 48, PNG-in-ICO
favicon-32.png
apple-touch-icon.png     180
icon-192.png             manifest, purpose any
icon-512.png             manifest, purpose any
icon-maskable-512.png    manifest, purpose maskable, inset for the safe zone
site.webmanifest
robots.txt
.nojekyll
LICENSE
```

`index.html` makes no network requests at all. Both weights of EB Garamond are
inlined as woff2 data URIs, the room is script-drawn SVG, and there are no
images, no stylesheets, no analytics, and no third-party anything. The only
outbound links are the four buttons and the CC0 deed.

The icons are the vase off the cover, traced to a solid silhouette. The
maskable icon is a separate file because the standard icon sits at 39.7% of the
canvas half-diagonal, close enough to the 40% safe zone that an aggressive mask
would clip the lip.

## Deploying on GitHub Pages

1. Push this directory to the repository root on the default branch.
2. Settings, Pages, Source: Deploy from a branch. Branch: `main`, folder: `/`.
3. For a custom domain, add a `CNAME` file at the root holding the bare domain,
   one line, no scheme and no trailing slash. Then point the DNS at GitHub.

`.nojekyll` is here so Pages serves the files as they are rather than running
them through Jekyll.

## Still open

- The four buttons in `index.html` point at `#TODO-amazon-paperback`,
  `#TODO-amazon-hardcover`, `#TODO-archive-pdf` and `#TODO-archive-audio`.
- The domain in the metadata is a placeholder: `the-windowless-room.com`
  appears in the canonical link and in three `og:image` tags. Update those and
  add the `CNAME` file together.

## Licence

CC0 1.0 Universal. See `LICENSE`. If you want GitHub's licence detector to
recognise it, replace that file with the full legal code from
creativecommons.org.
