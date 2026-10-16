# CSE Under Box

CSE Under Box is a GitHub-first undergraduate Computer Science and Engineering learning system.

The goal is to cover the complete Khulna University B.Sc. Engg. in CSE curriculum inside one lightweight cross-platform desktop application. The application will provide structured lessons, diagrams, animations, code examples, laboratories, quizzes, projects, thesis guidance, and curated external resources such as YouTube lectures.

## Core principles

- Curriculum-first: every course and prerequisite is explicitly mapped.
- Concept-first: each lesson explains the idea before asking students to copy code.
- Visual and practical: concepts are shown through diagrams, animations, simulations, code, and projects.
- GitHub-native: source code, curriculum data, lesson content, resource metadata, and release packages live in GitHub.
- Modular downloads: the launcher stays small; courses are downloaded as versioned packages.
- Offline-friendly: downloaded courses remain available without an internet connection.
- Original learning content: external videos supplement our lessons; they do not replace them.

## Planned repositories and package boundaries

The initial project is a monorepo so the system can begin simply:

- `app/` — desktop launcher and learning interface
- `content/curriculum/` — curriculum and prerequisite graph
- `content/courses/` — lesson packages
- `content/resources/` — reviewed YouTube and web resources
- `docs/` — architecture, authoring, and contribution guides
- `.github/workflows/` — validation and release automation

As the content grows, large courses can be split into dedicated repositories without changing the application contract.

## Download model

1. The application downloads `content/catalog.json`.
2. A student selects a course.
3. The application reads the course package URL and version.
4. A versioned archive is downloaded from GitHub Releases.
5. The course is unpacked into the application data directory.
6. The launcher checks the manifest for updates.
7. Only changed course packages are downloaded.

## Curriculum source

The initial curriculum map follows the Khulna University B.Sc. Engg. (CSE) curriculum published in December 2016:

https://ku.ac.bd/discipline/uploads/courses/Curriculum%20for%20B.Sc.%20Engg.%28CSE%29%20-Main.pdf

This repository is an independent educational project and is not an official Khulna University product.

## Current status

- [x] Repository created
- [x] Initial architecture documented
- [x] Full term-wise curriculum catalog mapped
- [ ] Cross-platform desktop launcher
- [ ] Course package downloader
- [ ] First complete course: Structured Programming I
- [ ] YouTube resource review workflow
- [ ] Cross-platform release pipeline (Windows, macOS, Linux)
