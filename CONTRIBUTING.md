# Contributing to AppNexus Community

Apps listed here appear on the [AppNexus](https://appnexus.app) app wall.

## Add your app in 3 steps

1. **Fork** this repository.

2. **Add your entry** to `apps.json`:

```json
{
  "developer": "Your Name",
  "apps": [
    "https://apps.apple.com/app/your-app/id123456789"
  ]
}
```

You can copy the App Store URL directly from the App Store or App Store Connect.
Add multiple apps under one entry if you have more than one.

3. **Open a Pull Request** — once merged, your apps appear on the wall at the next build.

## Rules

- Only submit apps you own or have permission to feature.
- One entry per developer.
- No duplicate App Store URLs.
- Must be a valid App Store URL containing `/id` followed by a numeric ID.
