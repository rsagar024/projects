# Projects

Static web pages for my apps, hosted on GitHub Pages.

Each top-level folder is one project and is published at:

```
https://<user>.github.io/<repo>/<folder>/
```

## Projects

### Color Tap

| Page | Path |
| --- | --- |
| Privacy Policy | [`color-tap/privacy/`](color-tap/privacy/) |
| Terms & Conditions | [`color-tap/terms/`](color-tap/terms/) |
| Delete Account | [`color-tap/delete-account/`](color-tap/delete-account/) |

## Adding a new project

1. Create a new folder at the repo root, e.g. `my-app/`.
2. Put an `index.html` in it (and in any subfolder you want reachable as `/my-app/<sub>/`).
3. Use relative links for assets and other pages (`style.css`, `../terms/`), not root-absolute ones (`/style.css`).
4. Merge to `master` — it deploys automatically.

## Deployment

The workflow in [`.github/workflows/deploy-pages.yml`](.github/workflows/deploy-pages.yml) deploys the whole repo to GitHub Pages on every push to `master`. It can also be run manually from the **Actions** tab.

One-time setup: **Settings → Pages → Build and deployment → Source: GitHub Actions**.

## License

[MIT](LICENSE)
