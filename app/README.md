# Application Shell

This folder contains the first GitHub-connected interface prototype for CSE Under Box.

The current shell:

- Reads the curriculum manifest from the GitHub raw URL.
- Displays the eight-term curriculum map.
- Supports course search.
- Opens course details.
- Links students back to the source repository.
- Uses fallback data if the remote manifest is temporarily unavailable.

The future cross-platform desktop application will package this interface with a lightweight desktop wrapper and add:

- GitHub Release package downloads
- SHA-256 verification
- Offline course storage
- Lesson rendering
- Code execution integrations
- Quiz and assessment progress
- Automatic application updates
