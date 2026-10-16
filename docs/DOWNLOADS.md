# Course Download and Release Flow

The launcher will not ship the entire degree content inside the installer.

## States

- planned: mapped in the curriculum, content not started
- source-preview: content exists in GitHub but has not passed package validation
- downloadable: a validated package is available as a GitHub Release asset
- update-available: a newer package version exists
- installed: the student has a verified local copy

## Release flow

1. Author lesson files in the course folder.
2. Add diagrams, animations, code, labs, quizzes, and resource metadata.
3. Validate the course manifest through GitHub Actions.
4. Build a versioned ZIP package.
5. Publish the package as a GitHub Release asset.
6. Record the release tag, asset URL, and SHA-256 hash in content/catalog.json.
7. The application displays Download Course.
8. The launcher downloads the archive and verifies the hash.
9. The course is unpacked into the user's application data directory.
10. Future launches check for catalog updates.

## Integrity

Every downloadable course should have a SHA-256 hash. The launcher must reject a package when the downloaded hash does not match the catalog.

## Platform behavior

The package format is shared across Windows, macOS, and Linux. Only the local application-data directory and native installer behavior differ.
