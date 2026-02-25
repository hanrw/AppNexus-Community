# AppNexus Community

A community-curated list of apps that appear in the [AppMate](https://appmate.onegai.app) showcase.

## What is this?

[AppMate](https://appmate.onegai.app) helps indie developers manage their App Store apps.
This repo lets the community add their own apps to the AppMate showcase — just edit `apps.json` and open a PR.

## Add your app

See [CONTRIBUTING.md](./CONTRIBUTING.md) for step-by-step instructions.

**TL;DR** — add your developer ID or app ID to `apps.json` and open a PR:

```json
{
  "developers": ["YOUR_DEVELOPER_ID"],
  "appIds": ["YOUR_APP_ID"],
  "manual": []
}
```

## How it works

1. You open a PR adding your entry to `apps.json`
2. CI validates the JSON against the schema and checks for duplicates
3. A maintainer reviews and merges
4. The AppMate site picks it up on the next build

## File reference

| File | Purpose |
|---|---|
| `apps.json` | The community app list — edit this |
| `schema.json` | JSON schema that validates `apps.json` |
| `CONTRIBUTING.md` | Detailed contribution guide |

## Links

- [AppMate website](https://appmate.onegai.app)
- [AppMate source](https://github.com/hanrw/AppMate)
