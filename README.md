# Course Template

This repository serves as a template for structuring course content. Each course consists of multiple modules, and each module contains multiple topics. Topics can be either written content (in Markdown) or videos (linked or embedded).

## Repository Structure
```
course-repo/
│── modules/
│   ├── module-1/
│   │   ├── topic-1.md
│   │   ├── topic-2.md
│   │   ├── topic-3.md
│   ├── module-2/
│   │   ├── topic-1.md
│   │   ├── topic-2.md
│   │   ├── topic-3.md
│── README.md
│── .gitignore
│── config.json (optional, metadata for course settings)
```

## Instructions for Content Creation

### 1. Creating Modules and Topics
- Each **module** is a directory inside `modules/`.
- Each **topic** is either a Markdown (`.md`) file.

Each Markdown topic should follow the below instructions for the content

1. Content should be in Markdown format
2. Content can have images, gifs, videos
3. Content can be multi paragraph


### 2. Videos in Topics
Content markdown support Video embedding, YouTube/ Vimeo embedding code can be placed. 

### 3. Course Metadata
A `config.json` file is used to store metadata about the course, such as title, description, and respective .md file.

```json
{
  "title": "Course Title",
  "description": "A brief description of the course.",
  "modules": [
    {
      "title": "Title of the module",
      "description" : "Description of the module",
      "folder": "folder name of the module. ex. module-1",
      "topics": [{
        {
          "title": "Title of the topic",
          "description": "Description of the topic",
          "file": "file name of the topic ex. module-1/topic-1.md"
        },
      }]
    }
  ]
}
```

## Contribution Guidelines
- Follow the structure strictly.
- Use clear, concise language in markdown content.
- Ensure all video links are accessible (made public/ unlisted).

---
This structure ensures consistency and allows easy navigation for learners.
