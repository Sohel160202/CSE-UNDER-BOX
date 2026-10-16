# CSE Under Box Architecture

## Product layers

### 1. Desktop launcher

The Windows application is the student's entry point. It owns:

- Curriculum browsing
- Search and filtering
- Download and update management
- Local course availability
- Progress tracking
- Lesson rendering
- Code and quiz launch points

The launcher must not contain the complete curriculum media. It should remain small and updateable.

### 2. Curriculum catalog

The catalog is structured data, not hardcoded UI. It defines:

- Years and terms
- Course codes and titles
- Theory or sessional classification
- Credit hours
- Prerequisites
- Course package status
- Course package version
- Release URL
- Learning outcomes

### 3. Course packages

A course package is a versioned, downloadable unit.

Recommended package layout:

```text
course-cse-1103/
├── course.json
├── lessons/
│   ├── 01-computer-and-programming/
│   │   ├── lesson.md
│   │   ├── media.json
│   │   ├── resources.json
│   │   └── quiz.json
│   └── 02-algorithms-and-flowcharts/
├── labs/
├── projects/
├── code/
└── assets/
```

Every package must contain a machine-readable `course.json` with its ID, version, manifest URL, prerequisites, and license information.

### 4. External resources

External resources are references, not copied course assets.

Each reviewed resource should record:

- URL
- Platform
- Channel or author
- Topic mapping
- Language
- Difficulty
- Resource type
- Last verified date
- Reviewer note
- Fallback resource when available

The application should gracefully handle removed or unavailable videos.

## GitHub release strategy

- Source and small text assets: normal Git history
- Course packages: GitHub Release assets
- Windows installer: GitHub Release asset
- Large media: package archives, not thousands of individual Git blobs
- Manifest: small JSON file fetched from the default branch or a tagged release

Use semantic versions:

```text
Application: 0.1.0
Course package: CSE-1103@0.1.0
Catalog schema: 1.0.0
```

## Content authoring rules

A lesson should normally include:

1. Learning objective
2. Prerequisite concepts
3. Problem or motivating example
4. Plain-language explanation
5. Visual representation
6. Code or worked example
7. Common mistakes
8. Practice activity
9. Assessment
10. Further resources

Our preferred teaching loop is:

```text
Build → Explain → Break → Debug → Improve
```

## Validation requirements

GitHub Actions should validate:

- JSON schema
- Duplicate course IDs
- Broken internal lesson links
- Missing prerequisites
- Invalid YouTube URLs
- Missing required lesson fields
- Package version consistency
- Release manifest integrity
