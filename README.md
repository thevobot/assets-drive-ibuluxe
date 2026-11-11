# assets-drive-ibuluxe

Free image CDN for all ibuluxe projects, served via [jsDelivr](https://www.jsdelivr.com/) + GitHub.

## CDN URL pattern

```
https://cdn.jsdelivr.net/gh/thevobot/assets-drive-ibuluxe@main/<folder>/<path>
```

| Folder | Source project | Contains |
|--------|---------------|----------|
| `ibuluxe_website/` | ibuluxe_website (Next.js) | Logos, favicons, billboards, blog images, product thumbnails, generated brand assets |
| `ibuluxe_admin/images/` | ibuluxe_admin (Flutter web) | Logo variants |
| `ibuluxe_app/images/` | ibuluxe_app (Flutter mobile) | Splash, onboarding and brand assets |

## Examples

```
# Website logo
https://cdn.jsdelivr.net/gh/thevobot/assets-drive-ibuluxe@main/ibuluxe_website/logo-black.png

# Billboard hero image
https://cdn.jsdelivr.net/gh/thevobot/assets-drive-ibuluxe@main/ibuluxe_website/assets/images/billboard/health-and-wellness-1920x550.webp

# Blog card image
https://cdn.jsdelivr.net/gh/thevobot/assets-drive-ibuluxe@main/ibuluxe_website/assets/images/blog/card/morning-wellness-rituals-to-reset-your-day.webp
```

## Why jsDelivr?

- **Free, no API keys, no paywalls** — unlimited requests on the free OSS tier
- **Global CDN** — backed by Cloudflare and Fastly, 99.9 %+ uptime
- **Automatic HTTP/2 and compression** — faster load times than Firebase Hosting
- **Immutable caching** — assets cached at the edge, zero bandwidth cost per repeat request
- **Zero configuration** — any file pushed to `main` is immediately available on the CDN

## Adding or updating assets

1. Add / replace files in the appropriate folder keeping the same directory structure.
2. Commit and push to `main`.
3. jsDelivr picks up the new files automatically within minutes.

> For a hard cache-bust (rare), reference a specific commit SHA instead of `@main`:
> `https://cdn.jsdelivr.net/gh/thevobot/assets-drive-ibuluxe@<SHA>/ibuluxe_website/logo-black.png`

## Reference — vobot sibling repo

Pattern follows [assets-drive-vobot](https://github.com/thevobot/assets-drive-vobot) which serves
`vobotin/`, `vobotcom/`, and `plasmabiotech/` folders for the thevobot.in family of sites.
