# AppNexus Community

A community-curated list of apps that appear on the [AppNexus](https://appnexus.app) app wall.

## Add your app

Add your entry to `apps.json` and open a PR:

```json
{
  "developer": "Your Name",
  "apps": [
    "https://apps.apple.com/app/your-app/id123456789"
  ]
}
```

See [CONTRIBUTING.md](./CONTRIBUTING.md) for full instructions.

## How it works

1. You open a PR adding your entry to `apps.json`
2. CI validates the format and checks for duplicates
3. A maintainer reviews and merges
4. The AppNexus site picks it up on the next build
