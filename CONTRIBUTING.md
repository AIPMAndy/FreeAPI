# Contributing to FreeAPI

Thank you for your interest in contributing to FreeAPI! 🎉

## How to Contribute

### Adding a New API

1. **Fork** this repository
2. **Edit** `apis.json` — add your API to the appropriate category
3. **Submit** a Pull Request

### API Entry Format

```json
{
  "name": "API Name",
  "url": "https://api-docs-url.com",
  "description": "Brief description of what this API does",
  "auth": "No|apiKey|OAuth|token",
  "https": "Yes|No",
  "cors": "Yes|No|Unknown"
}
```

### Guidelines

- ✅ **Must be free** — the API must have a free tier (no paid-only APIs)
- ✅ **Must be working** — test the API before submitting
- ✅ **Must have docs** — link to the API documentation
- ✅ **Accurate description** — clear, concise, factual
- ✅ **Correct auth type** — `No`, `apiKey`, `OAuth`, `token`, or `X-Mashape-Key`
- ❌ No deprecated or dead APIs
- ❌ No duplicates
- ❌ No self-promotion without a genuinely useful API

### Reporting Issues

Found a broken API? Please open an issue with:
- API name
- What's broken (dead link, returned error, etc.)
- Suggested replacement (if any)

## Code of Conduct

Be respectful, be helpful, be constructive.

## Questions?

Open an issue or start a discussion. We're friendly!
