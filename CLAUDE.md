# CLAUDE.md — shipthecode.dev

Personal brand blog for Michał — Senior Unity Developer.
Hugo + Blowfish theme, hosted on GitHub Pages.

## Stack
- Hugo Extended + Blowfish theme (git submodule at `themes/blowfish/`)
- Config in `config/_default/` — main files: `hugo.toml`, `languages.en.toml`, `params.toml`
- Content in `content/posts/`
- Auto-deploys to GitHub Pages on push to `main`

## Author Links
- GitHub: https://github.com/Seremonik
- LinkedIn: https://www.linkedin.com/in/micha%C5%82-duziak-09a588120/
- Configured in: `config/_default/languages.en.toml` (`[params.author] links`) and `config/_default/menus.en.toml` (nav icons)

### Landing page (`/`)
- Short author bio + headline
- Recent blog posts section
- Layout: `profile` in `params.toml`

### Blog (`/posts/`)
- List of all posts with card thumbnails
- No sidebar, no extras — just the posts

### About (`/about/`)
- File: `content/about/index.md`
- Contains: bio, career experience, projects worked on, shipped games

## New Post
```powershell
hugo new content posts/post-slug/index.md
```
- Set `draft: false` to publish
- Add `featured.jpg` in the post folder for card thumbnail
- Add `description:` for the card summary

## Local Preview
```powershell
hugo server -D
```
http://localhost:1313

## Deploy
```powershell
git add . && git commit -m "message" && git push
```

## Rules
- Never edit inside `themes/blowfish/` — it's a submodule
- Never delete `static/CNAME` — breaks custom domain