# OfflineOwl Content

First-party content for [OfflineOwl](https://offlineowl.app) - your offline survival and preparedness companion.

This repository contains original guides, interactive tools, games, and media created by the OfflineOwl team and contributors.

## Structure

```
content/
├── water-purification-wkdx/   # One folder per content item
│   ├── index.mdx              # Main content file
│   ├── meta.json              # Optional metadata
│   └── assets/                # Images, etc.
│
├── fire-starting-zugk/
│   └── index.mdx
│
├── survival-quiz-a7x9/
│   ├── index.html
│   ├── game.js
│   └── styles.css
│
└── README.md
```

**Flat structure** - Every content item is a folder at root level. No nested categories.

## Folder Naming

Folders use the same naming as registry files: `{slug}-{id}`

- `water-purification-wkdx/`
- `first-aid-basics-nc4i/`
- `radio-guide-je8k/`

## Supported Formats

Content can be any format:
- **Text**: `.txt`, `.md`, `.mdx`
- **Documents**: `.pdf`
- **Audio**: `.mp3`, `.ogg`
- **Video**: `.mp4`, `.webm`
- **Interactive**: `.html`, `.js`, `.ts`
- **Data**: `.json`, `.csv`

## Optional Metadata

Each folder can include a `meta.json` for additional info:

```json
{
  "entryPoint": "index.mdx",
  "assets": ["diagram.png", "video.mp4"],
  "buildCommand": "npm run build"
}
```

## How Content is Referenced

Content is indexed in the [OfflineOwl Registry](https://github.com/offlineowl/registry):

```json
{
  "id": "wkdx",
  "title": "Water Purification Guide",
  "localContent": {
    "repo": "https://github.com/offlineowl/content",
    "path": "water-purification-wkdx"
  }
}
```

## Contributing

1. Generate an ID using the [ID Generator](https://offlineowl.app/tools/id-generator)
2. Create folder: `{slug}-{id}/`
3. Add your content files
4. Submit PR to this repo
5. Submit PR to registry repo with metadata JSON

## Content Guidelines

- **Accuracy** - Information must be factually correct
- **Clarity** - Write for beginners, explain technical terms
- **Offline-first** - No external dependencies
- **Self-contained** - All assets in the folder

## License

Content is licensed under [CC-BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) unless otherwise specified.
