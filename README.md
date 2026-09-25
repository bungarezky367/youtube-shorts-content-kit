# YouTube Shorts Content Kit

A lightweight project generator for creating structured, repeatable YouTube Shorts production projects.

Designed for short-form workflows targeting USA + Global audiences, with a focus on clear scene planning, short voice-over segments, visual direction, SEO metadata, and final publishing checks.

## Features

- Creates a complete Shorts project folder automatically.
- Uses a 9:16 production format.
- Defaults to a maximum planned scene duration of 5 seconds.
- Generates scene-by-scene voice-over and visual placeholders.
- Generates an SEO metadata section.
- Generates a publishing checklist.
- Stores structured project information in JSON.
- Uses only Python's standard library.

## Requirements

- Python 3.9 or newer
- No third-party packages required

## Quick Start

Run:

~~~bash
python shorts_builder.py "Algeria vs Jordan World Cup" --scenes 8
~~~

This creates:

~~~text
projects/
└── algeria-vs-jordan-world-cup/
    ├── project.json
    ├── SCRIPT.md
    ├── CHECKLIST.md
    ├── README.md
    ├── scenes/
    ├── assets/
    └── export/
~~~

## Command Options

~~~text
python shorts_builder.py TITLE [--scenes N] [--output DIRECTORY]
~~~

- TITLE: Shorts project title.
- --scenes: Number of scenes. Default: 8.
- --output: Output directory. Default: projects.

Example:

~~~bash
python shorts_builder.py "NBA Trending Update" --scenes 7 --output projects
~~~

## Recommended Workflow

1. Create a project with shorts_builder.py.
2. Write and verify the voice-over in SCRIPT.md.
3. Keep each planned scene within the selected duration.
4. Add visual prompts and on-screen text for every scene.
5. Verify factual claims before publishing.
6. Complete the SEO section.
7. Follow CHECKLIST.md before final export.

## Project Structure

~~~text
youtube-shorts-content-kit/
├── shorts_builder.py
├── README.md
├── LICENSE
├── .gitignore
├── templates/
│   ├── project-template.json
│   └── scene-template.md
└── projects/
    └── .gitkeep
~~~

## Content Accuracy

The generator creates templates; it does not verify facts, copyright ownership, or platform policies. Claims, statistics, names, dates, images, clips, music, and other assets should be independently verified and properly licensed before publication.

## License

MIT License. See LICENSE.
