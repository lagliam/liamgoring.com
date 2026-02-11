# Liam Goring - Portfolio Website

A modern, responsive portfolio website built with [Astro](https://astro.build) and deployed on GitHub Pages.

## Getting Started

### Prerequisites
- Node.js 18+ 
- npm or yarn

### Installation

```bash
# Install dependencies
npm install
```

### Development

```bash
# Start the development server
npm run dev
```

The site will be available at `http://localhost:3000`

### Building

```bash
# Build for production
npm run build

# Preview the production build
npm run preview
```

## Deployment

This site is automatically deployed to GitHub Pages using GitHub Actions.

### Initial Setup

1. **Push to GitHub**
   ```bash
   git remote add origin <your-repository-url>
   git push --set-upstream origin main
   ```

2. **Enable GitHub Pages**
   - Go to your repository settings
   - Navigate to "Pages"
   - Under "Build and deployment", select:
     - Source: **Deploy from a branch**
     - Branch: **gh-pages** (this will be created automatically by the workflow)

3. **Configure Custom Domain** (Optional)
   - In Repository Settings > Pages
   - Add your custom domain (e.g., `liamgoring.com`)
   - Update your DNS settings to point to GitHub Pages

### Automatic Deployment

Every push to the `main` branch will:
1. Build the site using the GitHub Actions workflow
2. Deploy to the `gh-pages` branch
3. Update your live site at `https://liamgoring.com`

## Customization

### Update Your Info
Edit `src/pages/index.astro` to customize:
- Your name and title
- Hero subtitle
- Component data

### Edit Sections
- **Hero**: `src/components/Hero.astro`
- **About**: `src/components/About.astro`
- **Projects**: `src/components/Projects.astro`
- **Skills**: `src/components/Skills.astro`
- **Contact**: `src/components/Contact.astro`

### Styling
Global styles and CSS variables are in `src/layouts/Layout.astro`. Update the `:root` CSS variables to change colors.

## Project Structure

```
src/
├── components/          # Reusable components
│   ├── About.astro
│   ├── Contact.astro
│   ├── Hero.astro
│   ├── Projects.astro
│   └── Skills.astro
├── layouts/
│   └── Layout.astro    # Main layout with nav/footer
└── pages/
    └── index.astro     # Home page
```

## Technologies Used

- **Framework**: [Astro](https://astro.build)
- **Styling**: CSS with CSS Variables
- **Deployment**: GitHub Pages + GitHub Actions
- **Hosting**: GitHub

## License

Feel free to use this template for your own portfolio!
