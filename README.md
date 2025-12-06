# PromptMaster: Interactive Engineering Guide

An interactive study guide for mastering generative AI prompt engineering, featuring mobile-first simulators for building, testing, and securing prompts.

## Features

- **Prompt Lab**: Drag-and-drop prompt builder with instant AI simulation
- **Logic & RAG**: Visualize Chain-of-Thought and retrieval pipelines
- **Red Team Sim**: Test defenses against prompt injection attacks
- **Certification Quiz**: Test your knowledge with interactive assessments

## Setup Instructions

### 1. Create GitHub Repository

Using GitHub CLI, create a new public repository:

```bash
gh repo create prompt-master --public --source=. --remote=origin --push
```

If you don't have GitHub CLI installed, you can:
1. Go to [GitHub](https://github.com/new)
2. Create a new repository named `prompt-master`
3. Make it public
4. Initialize and push your code:

```bash
git init
git add .
git commit -m "Initial commit: PromptMaster interactive guide"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/prompt-master.git
git push -u origin main
```

### 2. Enable GitHub Pages

1. Go to your repository on GitHub
2. Navigate to **Settings** → **Pages**
3. Under **Source**, select **GitHub Actions** (not "Deploy from a branch")
4. The GitHub Actions workflow will automatically deploy your site when you push to the `main` branch

### 3. Access Your Site

After the first deployment completes (usually takes 1-2 minutes), your site will be available at:

```
https://YOUR_USERNAME.github.io/prompt-master/
```

You can find the exact URL in:
- Repository **Settings** → **Pages**
- The workflow run output under the "Deploy to GitHub Pages" step

## Local Development

Simply open `index.html` in your web browser, or use a local server:

```bash
# Using Python
python3 -m http.server 8000

# Using Node.js (if you have http-server installed)
npx http-server

# Using PHP
php -S localhost:8000
```

Then visit `http://localhost:8000` in your browser.

## Project Structure

```
prompt-master/
├── index.html              # Main application file
├── .github/
│   └── workflows/
│       └── deploy.yml      # GitHub Actions deployment workflow
└── README.md              # This file
```

## Technologies Used

- HTML5
- Tailwind CSS (via CDN)
- Material Symbols Icons
- Tone.js (for audio features)
- Vanilla JavaScript

## License

This project is open source and available for educational purposes.

