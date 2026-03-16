# OfflineOwl Resources

First-party resources for [OfflineOwl](https://offlineowl.app) — your offline survival and preparedness companion.

This repository contains original guides, interactive tools, games, and media created by the OfflineOwl team and contributors.

## Structure

```
resource/
├── basic-first-aid-k2m8/        # One folder per resource
│   ├── index.md                  # Markdown version
│   ├── index.mdx                 # Interactive MDX version
│   └── index.html                # HTML version
│
├── nuclear-fallout-protection-n8f2/
│   ├── index.mdx
│   ├── index.txt
│   ├── manifest.json             # Multi-format manifest
│   ├── shelter-diagram.svg
│   └── print-version.pdf
│
├── CONTRIBUTING.md               # How to contribute
└── README.md
```

**Flat structure** — every resource is a folder at root level. No nested categories.

## Folder Naming

Folders use the format `{slug}-{id}`:

- `basic-first-aid-k2m8/`
- `water-purification-wkdx/`
- `survival-quiz-a7x9/`

The ID is a unique 4-character alphanumeric string generated via the [ID Generator](https://offlineowl.app/tools/id-generator).

## Supported Formats

| Type | Formats |
|------|---------|
| Text | `.md`, `.mdx`, `.txt` |
| Documents | `.pdf` |
| Audio | `.mp3`, `.ogg` |
| Video | `.mp4`, `.webm` |
| Interactive | `.html`, `.js`, `.ts` |
| Data | `.json`, `.csv` |

Resources can include multiple formats (e.g., MDX for interactive + PDF for printing). See [CONTRIBUTING.md](CONTRIBUTING.md) for details on multi-format resources.

## How Content Is Indexed

Each resource has a corresponding JSON file in the [registry](https://github.com/offlineowl/registry) repo that defines its metadata — title, description, category, tags, license, etc. The registry is what the OfflineOwl app reads to display and search resources.

## Contributing

Want to create and share your own resource? See the full guide:

- **[CONTRIBUTING.md](CONTRIBUTING.md)** — step-by-step instructions for creating and submitting resources
- **[Web Docs](https://offlineowl.app/docs/contributing)** — the same guide on the OfflineOwl website

## Content Guidelines

- **Accuracy** — information must be factually correct, especially survival/medical content
- **Clarity** — write for beginners, explain technical terms
- **Offline-first** — no external dependencies or links
- **Self-contained** — all assets must be in the resource folder

## License

Content is licensed under [CC-BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) unless otherwise specified in individual resource metadata.
