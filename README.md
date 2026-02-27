# Short Stories

A GitHub Pages project for publishing short stories using markdown files, automatically deployed with GitHub Actions.

## Features

- 📝 Write stories in simple Markdown format
- 🚀 Automatic deployment via GitHub Actions
- 🎨 Clean, readable layout using Jekyll
- 📚 Easy to maintain and version control

## Project Structure

```
.
├── .github/
│   └── workflows/
│       └── pages.yml          # GitHub Actions workflow for deployment
├── stories/
│   ├── first-story.md         # Sample story 1
│   └── adventure.md           # Sample story 2
├── _config.yml                # Jekyll configuration
├── index.md                   # Homepage
└── README.md                  # This file
```

## How It Works

1. Write your stories in Markdown format in the `stories/` directory
2. Update `index.md` to add links to new stories
3. Push changes to the main/master branch
4. GitHub Actions automatically deploys the site to GitHub Pages

## Setup

To enable GitHub Pages for this repository:

1. Go to Repository Settings → Pages
2. Under "Build and deployment", select "GitHub Actions" as the source
3. The workflow will automatically deploy on push to main/master branch

## Adding New Stories

1. Create a new `.md` file in the `stories/` directory
2. Add front matter at the top:
   ```yaml
   ---
   layout: default
   title: Your Story Title
   ---
   ```
3. Write your story content in Markdown
4. Update `index.md` to add a link to your new story

## Local Development

To preview the site locally:

```bash
# Install Jekyll
gem install bundler jekyll

# Run the server
jekyll serve
```

Visit `http://localhost:4000` to see your site.

## License

This project is open source and available for anyone to use and modify.