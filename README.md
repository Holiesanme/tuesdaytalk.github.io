# Tuesday Talk

A simple static website for Tuesday Talk — a recurring session exploring ideas and tools in software development.

Live at: **https://tuesdaytalk.github.io**

## Structure

```
tuesdaytalk.github.io/
├── index.html        # Home page
├── claude-talk.html  # Session page: Claude Code & MCP
├── style.css         # Shared stylesheet
└── .github/
    └── workflows/
        └── static.yml  # GitHub Actions deployment workflow
```

## Deployment

The site is deployed automatically to GitHub Pages via GitHub Actions on every push to `main`. No build step — files are served as-is from the repository root.

To publish changes:

```bash
git add .
git commit -m "your message"
git push
```

## Adding a new session page

1. Create a new `.html` file in the root directory.
2. Add the standard `<head>` links for Inter font and `style.css`.
3. Link to it from `index.html`.
