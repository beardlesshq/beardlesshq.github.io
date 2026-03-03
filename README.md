# beardless.io

Business card site for Beardless HQ. Technology advisory — Stockholm, Sweden.

## Stack

- [Hugo](https://gohugo.io/) — static site generator
- Zero JavaScript, inline CSS
- GitHub Pages + GitHub Actions for deployment
- Google Fonts: Syne 700, DM Mono 400

## Development

```
hugo server
```

Open http://localhost:1313

## Deploy

Push to `main`. GitHub Actions builds with Hugo and deploys to GitHub Pages automatically.

## Structure

```
hugo.toml          # Site config
layouts/
  index.html       # Homepage template
  404.html         # 404 page
content/
  _index.md        # Homepage content
static/
  CNAME            # Custom domain
  robots.txt
  humans.txt
```
