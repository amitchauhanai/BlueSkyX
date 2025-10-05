# BlueSkyX

Ocean Visualization Studio — single-page prototype demonstrating an immersive, data-driven concept using NASA assets and local media.

## What's included
- `index.html` — single-page website with background video, header, sections (About, Project, Lab, Launch VR, Login, Data Explorer).
- `style.css` — styles and animations.
- `lakeice-measurements.xlsx` — example dataset parsed by the Data Explorer.
- `NASA-Logo-Large.png` — logo image.

Note: Large MP4 files were intentionally excluded from this repo copy. Host videos separately or use Git LFS if you wish to include them.

## Local development
Serve the folder over HTTP (recommended):

  python3 -m http.server 8000

Open http://localhost:8000 in your browser.

## Features
- Background video with autoplay handling and fallback overlay.
- Responsive navigation with mobile menu.
- Lab section with NASA SVS embed + fallback link.
- Launch VR section with video previews and fullscreen controls.
- Data Explorer that parses `lakeice-measurements.xlsx` and plots a chart using Chart.js.

## Pushing large media
To add videos with Git LFS:

  git lfs install
  git lfs track "*.mp4"
  git add .gitattributes
  git add path/to/video.mp4
  git commit -m "Add video via LFS"
  git push

## License
Check source terms for NASA assets and any included media. Code provided as-is.

Generated on 2025-10-06.
