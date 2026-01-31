# Contributing to OfflineOwl Content

Thank you for contributing original content to OfflineOwl!

## Two Repositories

| Repository | Purpose |
|------------|---------|
| **This repo** (`content`) | Actual content files |
| [offlineowl/registry](https://github.com/offlineowl/registry) | JSON metadata index |

**When adding content, submit PRs to both repos.**

---

## Structure

Every piece of content is a folder at the root:

```
content/
├── water-purification-wkdx/
│   ├── index.mdx
│   └── assets/
├── survival-quiz-a7x9/
│   ├── index.html
│   └── game.js
└── first-aid-video-k2m3/
    └── video.mp4
```

**Flat structure** - No nested categories. One folder per content item.

## Folder Naming

Use format: `{slug}-{id}`

1. Generate an ID using the [ID Generator](https://offlineowl.app/tools/id-generator)
2. Create folder: `my-content-a7x9/`

---

## Supported Formats

| Type | Example Files |
|------|---------------|
| Guide | `index.mdx`, `index.md`, `guide.txt` |
| Interactive | `index.html`, `game.js`, `app.ts` |
| Video | `video.mp4`, `tutorial.webm` |
| Audio | `audio.mp3`, `podcast.ogg` |
| Document | `manual.pdf` |
| Data | `data.json`, `reference.csv` |

## Optional Metadata

Add `meta.json` to your folder for extra config:

```json
{
  "entryPoint": "index.mdx",
  "assets": ["diagram.png", "video.mp4"],
  "buildCommand": "npm run build"
}
```

---

## Adding Content

### Step 1: Generate an ID

Use the [ID Generator](https://offlineowl.app/tools/id-generator) to get a unique 4-char ID.

### Step 2: Create Folder

```bash
mkdir my-guide-a7x9
```

### Step 3: Add Content

**For a guide:**
```
my-guide-a7x9/
├── index.mdx
└── assets/
    └── diagram.png
```

**For interactive content:**
```
my-quiz-k2m3/
├── index.html
├── game.js
└── styles.css
```

**For media:**
```
tutorial-video-p9q2/
└── video.mp4
```

### Step 4: Submit PR to This Repo

### Step 5: Submit PR to Registry

Create `{slug}-{id}.json` at registry root:

```json
{
  "id": "a7x9",
  "version": "1.0.0",
  "title": "My Guide Title",
  "description": "Description for search...",
  "type": "guide",
  "category": "survival",
  "tags": ["water", "purification"],
  "localContent": {
    "repo": "https://github.com/offlineowl/content",
    "path": "my-guide-a7x9"
  },
  "license": "cc-by-sa",
  "author": "Your Name",
  "language": "en",
  "createdAt": "2026-01-31T00:00:00.000Z",
  "updatedAt": "2026-01-31T00:00:00.000Z"
}
```

---

## Content Guidelines

### Accuracy
- Information must be factually correct
- Survival/medical content could be life-saving - verify everything

### Clarity
- Write for beginners
- Define technical terms
- Use tables for quick reference

### Offline-First
- No external dependencies
- All assets in the folder
- No iframes or external embeds

---

## Content Types

- `guide` - MDX/Markdown guides
- `document` - PDF, text files
- `video` - MP4, WebM
- `audio` - MP3, OGG
- `game` - Interactive HTML/JS
- `tool` - Calculators, utilities
- `dataset` - Data files

---

## License

All contributions are licensed under [CC-BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) unless specified otherwise.

---

## Questions?

Open an issue if you have questions about contributing!
