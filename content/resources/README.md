# External Resource Curation

External resources supplement the original CSE Under Box lessons.

## Approved resource types

- YouTube lecture
- YouTube concept explanation
- University open-course lecture
- Documentation
- Open textbook
- Research paper
- GitHub reference implementation
- Interactive simulator

## YouTube resource record

Each resource should include:

```json
{
  "id": "youtube-mit-6006-lecture-1",
  "title": "Algorithms and Computation",
  "url": "https://www.youtube.com/watch?v=ZA-tUyM_y7s",
  "platform": "YouTube",
  "channel": "MIT OpenCourseWare",
  "courseIds": ["CSE-2201"],
  "topicIds": ["algorithms", "data-structures"],
  "language": "English",
  "level": "undergraduate",
  "type": "university-lecture",
  "reviewStatus": "reviewed",
  "lastVerified": "YYYY-MM-DD",
  "note": "Use after the introductory visual lesson."
}
```

## Review checklist

Before a resource is marked `reviewed`:

- It directly matches one or more syllabus concepts.
- The explanation is technically accurate.
- The intended level is clear.
- The language and audio are understandable.
- The link is publicly available.
- The video is supplementary, not the only explanation.
- A replacement resource is identified for important topics.

Do not download or rehost third-party videos. Store metadata and links, and let the application open or embed the original resource.
