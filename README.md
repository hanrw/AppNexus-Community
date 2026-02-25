# AppNexus Community

A community-curated list of apps that appear on the [AppNexus](https://appnexus.app) app wall.

## Add your app

Edit `apps.json`, add your App Store URL, and open a PR:

```json
[
  "https://apps.apple.com/app/your-app-name/id123456789"
]
```

See [CONTRIBUTING.md](./CONTRIBUTING.md) for full instructions.

## How it works

1. You open a PR adding your App Store URL to `apps.json`
2. CI validates the URL format and checks for duplicates
3. A maintainer reviews and merges
4. The AppNexus site picks it up on the next build
