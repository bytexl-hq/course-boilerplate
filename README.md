# Course Template

This repository serves as a template for structuring course content. Each course consists of multiple modules, and each module contains multiple topics. Topics can be either written content (in Markdown) or videos (linked or embedded).

## Repository Structure
```
course-repo/
│── modules/
│   ├── module-1/
│   │   ├── topic-1.md
│   │   ├── topic-2.md
│   │   ├── video-topic-3/
│   │   │   ├── video.md
│   │   │   ├── video.mp4 (optional, can be hosted externally)
│   ├── module-2/
│   │   ├── topic-1.md
│   │   ├── topic-2.md
│   │   ├── video-topic-3/
│   │   │   ├── video.md
│   │   │   ├── video.mp4
│── README.md
│── .gitignore
│── config.json (optional, metadata for course settings)
```

## Instructions for Content Creation

### 1. Creating Modules and Topics
- Each **module** is a directory inside `modules/`.
- Each **topic** is either a Markdown (`.md`) file or a subdirectory (if it's a video topic).
- Markdown files should follow the format described below.

### 2. Markdown Format for Topics
Each Markdown topic should follow this format:

```markdown
# Topic Title

## Learning Objectives
- Objective 1
- Objective 2
- Objective 3

## Content
(Content goes here in markdown format)

## Summary
(Summarize the key takeaways)
```

### 3. Adding Videos
- For video topics, create a folder with a `video.md` file inside.
- Videos should be stored externally (YouTube, Vimeo, or cloud storage) and linked inside `video.md`.
- Example `video.md` format:

```markdown
# Topic Title (Video)

## Video Link
[Watch Video Here](https://example.com/video-link)

## Summary
(Summary of the video content)
```

### 4. Course Metadata
A `config.json` file can be used to store metadata about the course, such as title, description, and module structure.

```json
{
  "title": "Course Title",
  "description": "A brief description of the course.",
  "modules": [
    {
      "title": "Module 1",
      "topics": ["Topic 1", "Topic 2", "Video Topic 3"]
    }
  ]
}
```

## Contribution Guidelines
- Follow the structure strictly.
- Use clear, concise language in markdown content.
- Ensure all video links are accessible.
- Commit changes with meaningful messages.

---
This structure ensures consistency and allows easy navigation for learners.
