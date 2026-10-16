# Platform Support

CSE Under Box is planned as one desktop application for:

| Platform | Planned package | Release source |
|---|---|---|
| Windows | Setup executable and optional MSI | GitHub Releases |
| macOS | DMG and app bundle | GitHub Releases |
| Linux | AppImage first; Debian/RPM later | GitHub Releases |

## Shared across platforms

- Curriculum manifest
- Course catalog
- Downloaded course packages
- Lesson format
- YouTube and external-resource metadata
- Progress model
- Search and navigation
- GitHub update protocol

## Platform-specific concerns

Only these areas should contain platform-specific behavior:

- Installer and application bundle creation
- User data directory resolution
- Native update installation
- File associations
- Optional system notifications
- Code-signing and notarization

The goal is to keep course content and the learning experience identical on every platform.
