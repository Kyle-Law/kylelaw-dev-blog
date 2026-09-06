# blog.kylelaw.dev

Static site for **blog.kylelaw.dev**. Plain HTML/CSS, no build step.

## Hosting

| | |
|---|---|
| Host | `blog.kylelaw.dev` |
| Cloudflare Pages project | `kylelaw-blog` |
| Production branch | `main` |
| Framework preset | None |
| Build command | *(empty)* |
| Output directory | `/` |

Push to `main` deploys to production. Any other branch gets a preview URL at
`<hash>.kylelaw-blog.pages.dev`.

## Local preview

```sh
python3 -m http.server 8000
```

## Notes

- Links to the other kylelaw.dev sites are **absolute URLs** — they cross origins.
- `style.css` is duplicated across the three site repos on purpose. If it starts
  drifting, promote it to `https://kylelaw.dev/shared/site.css` and link cross-origin.
- `_headers` sets baseline security headers; Cloudflare Pages applies it at the edge.
