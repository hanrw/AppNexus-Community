# Contributing to AppNexus Community

Apps listed here appear in the [AppMate](https://appmate.onegai.app) showcase.

## How to add your app

1. **Fork** this repository.
2. Edit `apps.json` — choose the method that fits your case:

### Option A — Add your developer ID (easiest)

All of your App Store apps are included automatically.

```json
{
  "developers": ["1725133580"],
  ...
}
```

Find your developer ID: open any of your apps in the App Store, tap your name,
then copy the numeric ID from the URL:
`https://apps.apple.com/developer/your-name/id<THIS_NUMBER>`

### Option B — Add individual app IDs

```json
{
  "appIds": ["6448311069"],
  ...
}
```

Find an app ID in its App Store URL:
`https://apps.apple.com/app/your-app/id<THIS_NUMBER>`

### Option C — Manual entry

Use this if iTunes lookup returns the wrong data or your app isn't on the US store.

```json
{
  "manual": [
    {
      "id": "6448311069",
      "name": "Your App Name",
      "icon": "https://is1-ssl.mzstatic.com/..."
    }
  ]
}
```

3. **Open a Pull Request** with the title `feat: add [Your App Name]`.
4. Once merged, your app will appear on the site at the next build.

## Rules

- Only submit apps you own or have permission to feature.
- No duplicate entries (check existing IDs before adding).
- Icon URLs must be from `mzstatic.com` (App Store CDN) or a stable public host.
- PRs that don't follow the schema will fail the validation check automatically.

## Validation

The CI workflow validates `apps.json` against `schema.json` on every PR.
You can validate locally with:

```bash
npx ajv-cli validate -s schema.json -d apps.json
```
