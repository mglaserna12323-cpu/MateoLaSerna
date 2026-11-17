# Mateo La Serna — Filmmaker Portfolio

A cinematic, dark-themed portfolio website designed for Mateo La Serna (Filmmaker, Est. 2023).

## Directory Structure

```text
mateo-portfolio/
├── index.html                 # Complete portfolio website (HTML, Tailwind CSS, JavaScript)
├── README.md                  # Project documentation & instructions
└── assets/
    ├── logo.svg               # Aperture emblem fallback (place your logo.png here)
    ├── logo.png               # (Optional) Custom aperture / film-reel emblem
    ├── hero-bg.jpg            # (Optional) Moody mountain backdrop (falls back to cinematic Unsplash mountain)
    ├── mateo-portrait.jpg     # (Optional) Professional portrait photo (falls back to cinematic photographer)
    ├── resume.pdf             # Production resume with Hollywood PA credits
    ├── previews/              # Drop your 10–15s silent MP4 preview clips here
    └── scripts/               # Drop your screenplay and treatment PDFs here
        ├── feature-script.pdf
        └── short-script.pdf
```

## Adding Films & Screenplays

All projects and screenplays are defined in `index.html` inside the `<script>` tag:

### To add a new film:
Add an entry to the `PROJECTS` array in `index.html`:
```js
{
  title: "FILM TITLE",
  role: "Director / Cinematographer",
  year: "2026",
  category: "NARRATIVE", // or "DOCUMENTARY" or "COMMERCIAL"
  description: "One or two sentence logline / synopsis.",
  poster: "assets/posters/your-poster.jpg", // or web URL
  previewVideo: "assets/previews/your-clip.mp4",
  fullVideoEmbed: "https://www.youtube.com/embed/VIDEO_ID?autoplay=1"
}
```

### To add a new screenplay:
Add an entry to the `SCREENPLAYS` array in `index.html`:
```js
{
  title: "SCRIPT TITLE",
  format: "Feature Film • 98 Pages",
  genre: "Drama / Thriller",
  logline: "Your logline describing the core conflict and protagonist journey.",
  pdfUrl: "assets/scripts/your-script.pdf"
}
```

## Connecting to GitHub

When you're ready to deploy or push to GitHub:
1. Initialize git in this directory (`git init`)
2. Commit your files (`git add . && git commit -m "Initial commit"`)
3. Connect your GitHub remote repository and push (`git remote add origin ... && git push -u origin main`)
4. You can also host it for free via GitHub Pages!
