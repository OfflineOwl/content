# Contributing Resources to OfflineOwl

OfflineOwl is built on community-contributed preparedness knowledge. This guide walks you through creating and sharing your own resources — from writing a survival guide to submitting an interactive tool.

---

## How It Works

OfflineOwl resources live across two repositories:

| Repository | What Goes Here |
|---|---|
| **`resource/`** (this repo) | The actual content files — markdown, HTML, PDFs, etc. |
| **`registry/`** | A JSON metadata file for each resource (title, category, tags, etc.) |

When you contribute, you submit a PR to **both** repos: one with your content files, one with the metadata JSON that tells OfflineOwl how to index and display it.

---

## Quick Start

Here's the fastest path to contributing a resource:

```bash
# 1. Generate a unique 4-character ID
#    Go to https://offlineowl.app/tools/id-generator
#    Example: a7x9

# 2. Create your resource folder
mkdir water-filter-diy-a7x9

# 3. Add your content
echo "# How to Build a DIY Water Filter" > water-filter-diy-a7x9/index.md

# 4. Submit PRs to both repos (see detailed steps below)
```

---

## Step-by-Step Guide

### Step 1: Generate a Resource ID

Every resource needs a unique 4-character alphanumeric ID. Use the [ID Generator](https://offlineowl.app/tools/id-generator) to create one.

Example IDs: `k2m8`, `a7x9`, `n8f2`

### Step 2: Create Your Folder

Create a folder at the root of this repo using the format `{slug}-{id}`:

```
my-guide-title-a7x9/
```

**Naming rules:**
- Use lowercase kebab-case for the slug
- Keep it descriptive but concise
- End with your generated ID
- No nested folders — everything is flat at the root level

### Step 3: Add Your Content

Add your content files to the folder. At minimum, you need one entry point file.

**For a simple guide (most common):**
```
my-guide-a7x9/
└── index.md          # Your guide in Markdown
```

**For a guide with images:**
```
water-purification-a7x9/
├── index.md
├── filter-diagram.svg
└── boiling-chart.png
```

**For an interactive resource:**
```
survival-quiz-a7x9/
├── index.html
├── game.js
└── styles.css
```

**For media:**
```
knot-tying-tutorial-a7x9/
└── video.mp4
```

### Step 4: Provide Multiple Formats (Optional)

You can provide the same content in multiple formats so OfflineOwl can pick the best one for each device. If you do, add a `manifest.json`:

```json
{
  "id": "a7x9",
  "title": "My Guide",
  "description": "A brief description of this resource",
  "version": "1.0.0",
  "formats": {
    "mdx": {
      "file": "index.mdx",
      "description": "Interactive version with React components",
      "features": ["interactive", "animated"],
      "priority": 1
    },
    "md": {
      "file": "index.md",
      "description": "Standard markdown version",
      "features": ["offline"],
      "priority": 2
    },
    "pdf": {
      "file": "print-version.pdf",
      "description": "Designed PDF for printing",
      "features": ["printable", "designed"],
      "priority": 2
    },
    "txt": {
      "file": "index.txt",
      "description": "Plain text for any device",
      "features": ["universal", "offline"],
      "priority": 3
    }
  },
  "assets": {
    "images": [
      { "file": "diagram.svg", "alt": "Description of the diagram" }
    ]
  }
}
```

**Format priority** (1 = highest): The app serves the highest-priority format the device supports. A smartphone might get markdown while a desktop browser gets the interactive MDX version.

### Step 5: Create the Registry Entry

Create a JSON file in the `registry/` repo named `{slug}-{id}.json`:

```json
{
  "id": "a7x9",
  "version": "1.0.0",
  "title": "Your Resource Title",
  "description": "A detailed description for search and display. Mention what it covers and who it's for.",
  "shortDescription": "One-line summary for cards and lists",
  "type": "guide",
  "category": "survival",
  "tags": ["water", "purification", "diy"],
  "localContent": {
    "repo": "https://github.com/offlineowl/content",
    "path": "resource/my-guide-a7x9",
    "ref": "main",
    "entryPoint": "index.md",
    "format": "md"
  },
  "license": "cc-by-sa",
  "author": "Your Name",
  "language": "en",
  "createdAt": "2026-03-16T00:00:00.000Z",
  "updatedAt": "2026-03-16T00:00:00.000Z",
  "verified": false,
  "featured": false,
  "priority": 50
}
```

### Step 6: Submit Pull Requests

1. **PR #1** — to this repo (`resource/`) with your content folder
2. **PR #2** — to the `registry/` repo with your JSON metadata file

Both PRs will be reviewed together. Once merged, your resource appears in the OfflineOwl library.

---

## Registry Field Reference

| Field | Required | Description |
|---|---|---|
| `id` | Yes | Unique 4-character alphanumeric ID |
| `version` | Yes | Semantic version (e.g., `"1.0.0"`) |
| `title` | Yes | Display title |
| `description` | Yes | Full description for search and detail views |
| `shortDescription` | No | One-line summary for cards |
| `type` | Yes | Content type (see below) |
| `category` | Yes | Primary category (see below) |
| `tags` | Yes | Array of lowercase keyword tags |
| `localContent` | Yes | Object pointing to the content files |
| `license` | Yes | License identifier (see below) |
| `author` | No | Creator name or "OfflineOwl Contributors" |
| `language` | Yes | ISO 639-1 code (e.g., `"en"`) |
| `createdAt` | Yes | ISO 8601 timestamp |
| `updatedAt` | Yes | ISO 8601 timestamp |
| `verified` | Yes | `false` for community submissions (team sets to `true`) |
| `featured` | Yes | `false` for community submissions |
| `priority` | Yes | Sort weight, `50` is default |

### Content Types

| Type | Use For |
|---|---|
| `guide` | Written guides, tutorials, how-tos |
| `document` | Reference documents, PDFs, manuals |
| `video` | Video tutorials, demonstrations |
| `audio` | Audio guides, podcasts |
| `image` | Infographics, diagrams, charts |
| `game` | Interactive quizzes, learning games |
| `tool` | Calculators, utilities, interactive tools |
| `dataset` | Data files, reference tables |
| `archive` | Bundled collections |
| `ai-model` | Offline AI models |

### Categories

| Category | Description |
|---|---|
| `survival` | General survival skills, emergency response |
| `medical` | First aid, health, medical procedures |
| `food-water` | Food preservation, water purification, foraging |
| `shelter` | Shelter building, home fortification |
| `communication` | Radio, signals, emergency communication |
| `entertainment` | Games, activities, morale-boosting content |
| `education` | Learning resources, skill development |
| `reference` | Reference materials, field manuals |

### Licenses

| License | Description |
|---|---|
| `cc-by-sa` | Creative Commons Attribution-ShareAlike (recommended) |
| `cc-by` | Creative Commons Attribution |
| `cc-by-nc` | Creative Commons Attribution-NonCommercial |
| `cc-by-nc-sa` | Creative Commons Attribution-NonCommercial-ShareAlike |
| `cc0` | Creative Commons Zero (public domain dedication) |
| `public-domain` | Public domain |
| `mit` | MIT License |
| `apache-2.0` | Apache License 2.0 |
| `gpl-3.0` | GNU GPL v3 |

---

## Content Guidelines

### Accuracy

- **Verify everything.** Survival and medical content can be life-saving — or life-threatening if wrong.
- Cite authoritative sources (military field manuals, Red Cross guidelines, WHO recommendations, etc.)
- If you're not an expert, note that and suggest professional consultation

### Clarity

- Write for beginners. Assume the reader has zero prior knowledge.
- Define technical terms on first use
- Use numbered steps for procedures
- Use tables for quick-reference data
- Break long guides into clear sections with descriptive headings

### Offline-First

This is critical — OfflineOwl is designed for situations where there's no internet.

- **No external links or embeds** — don't link to YouTube, external images, or CDNs
- **No external dependencies** — no scripts loaded from URLs
- **Self-contained assets** — all images, diagrams, and media must be in your resource folder
- **Text-first** — ensure critical information is in text, not only in images

### Printability

Many users will print resources. Help them:

- Use clear headings that work as a table of contents
- Include quick-reference checklists
- Avoid relying on color alone to convey meaning
- Consider including a print-ready PDF alongside your markdown

### File Size

- Keep resource folders under **50 MB** total
- Optimize images (SVG for diagrams, compressed PNG/JPEG for photos)
- Compress video and audio files
- PDFs should be under 5 MB when possible

---

## Writing in Markdown

Most resources are written in Markdown (`.md`). Here's a template to get started:

```markdown
# Your Resource Title

> **One-Line Summary** — A brief hook explaining what this guide covers and why it matters.

## Overview

Brief introduction. Who is this for? What will they learn?

---

## Section 1: Getting Started

Step-by-step content here.

1. **First step** — Explanation
2. **Second step** — Explanation
3. **Third step** — Explanation

---

## Section 2: Key Techniques

### Technique A

Details...

### Technique B

Details...

---

## Quick Reference

| Item | Details |
|------|---------|
| Key fact 1 | Value |
| Key fact 2 | Value |

---

## What to Do If...

Common scenarios and troubleshooting.

---

## Sources & Further Reading

- Source 1
- Source 2
```

---

## Writing in MDX

MDX lets you embed React components for interactive content. Use `.mdx` files:

```mdx
# Interactive Water Purification Guide

<Callout type="warning">
  Always purify water from unknown sources before drinking.
</Callout>

## Boiling Method

Bring water to a **rolling boil** for at least 1 minute (3 minutes above 6,500 ft elevation).

<Checklist items={[
  "Container that can withstand heat",
  "Heat source (fire, stove)",
  "Way to handle hot container"
]} />
```

**Note:** MDX resources should always have a plain `.md` or `.txt` fallback for devices that don't support React rendering.

---

## Print-Ready PDFs

If you want to include a professionally designed print version:

1. Add the PDF to your resource folder (e.g., `print-version.pdf`)
2. Include a `pdf` entry in your `manifest.json` formats
3. The PDF will show as a "Print PDF" button in the app

**PDF best practices:**
- Include page numbers
- Use clear headings for scanning
- Add quick-reference cards or checklists
- Keep file size under 5 MB
- Ensure text is searchable (not scanned images)

---

## Updating an Existing Resource

1. Make your changes in the resource folder
2. Bump the `version` in the registry JSON (e.g., `"1.0.0"` to `"1.1.0"`)
3. Update the `updatedAt` timestamp
4. Submit PRs to both repos

---

## Questions?

- Open an [issue](https://github.com/offlineowl/content/issues) if you need help
- Check the [docs](https://offlineowl.app/docs/contributing) for the latest version of this guide
