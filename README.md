# Technical Writing Portfolio - Docs-as-Code Samples

A professional portfolio site showcasing technical writing samples following docs-as-code best practices. Built with clean HTML, CSS, and JavaScript—ready to deploy to GitHub Pages.

## 🚀 Quick Deploy to GitHub Pages

### Option 1: New Repository

1. Create a new repository on GitHub (e.g., `docs-portfolio`)
2. Clone it locally:
   ```bash
   git clone https://github.com/YOUR-USERNAME/docs-portfolio.git
   cd docs-portfolio
   ```
3. Copy the `index.html` file to the repository root
4. Commit and push:
   ```bash
   git add index.html
   git commit -m "Initial commit: Add docs-as-code portfolio site"
   git push origin main
   ```
5. Enable GitHub Pages:
   - Go to your repository settings
   - Navigate to **Pages** (in the left sidebar)
   - Under **Source**, select `main` branch and `/root` folder
   - Click **Save**
   - Your site will be live at `https://YOUR-USERNAME.github.io/docs-portfolio/`

### Option 2: Using GitHub Username Site

1. Create a repository named `YOUR-USERNAME.github.io`
2. Follow steps 2-4 from Option 1
3. Your site will automatically be published at `https://YOUR-USERNAME.github.io/`

## ✨ Features

### Design Elements
- **Editorial Typography**: Instrument Serif for headings, Crimson Pro for body text, IBM Plex Mono for code
- **Warm Color Palette**: Refined earth tones with strategic accent colors
- **Smooth Animations**: Fade-ins, slide-ups, and hover effects
- **Responsive Layout**: Optimized for desktop, tablet, and mobile
- **Interactive Filtering**: Filter samples by category (All, API Docs, User Guides, Reference)

### Content Samples Included

The site includes 12 diverse technical writing samples across three categories:

#### API Documentation (4 samples)
- REST API Reference (OpenAPI, Redoc)
- GraphQL Schema Docs (Docusaurus, Schema SDL)
- Webhook Event Catalog (AsyncAPI)
- Swagger UI Implementation (OpenAPI, Interactive)

#### User Guides (4 samples)
- Getting Started Guide (MDX, Next.js)
- Architecture Decision Records (MADR, Markdown)
- Troubleshooting Runbook (MkDocs)
- MkDocs Material Theme (Python-based)

#### Reference Documentation (4 samples)
- CLI Command Reference (Cobra, Go)
- SDK Reference Library (Multi-language)
- Configuration Reference (YAML, JSON Schema)
- Docusaurus Documentation (React, MDX)

## 🎨 Customization

### Adding New Samples

Add new sample cards to the `samples-grid` section:

```html
<article class="sample-card" data-category="api">
    <div class="sample-category">API Documentation</div>
    <h3 class="sample-title">Your Sample Title</h3>
    <p class="sample-description">
        Brief description of your documentation sample.
    </p>
    <div class="sample-tags">
        <span class="tag">Technology 1</span>
        <span class="tag">Technology 2</span>
    </div>
    <a href="#" class="sample-link">View Documentation →</a>
</article>
```

### Updating Links

Replace `#` placeholders with actual URLs to your documentation:
- GitHub repository links
- Published documentation sites
- Blog posts
- Case studies

### Customizing Colors

Edit CSS variables in the `:root` selector:

```css
:root {
    --bg-primary: #fdfcfb;
    --text-primary: #1a1814;
    --accent-warm: #c77545;
    /* ... more variables */
}
```

### Adding Categories

To add a new category filter:

1. Add a new tab button in the `<nav>` section:
   ```html
   <button class="nav-tab" data-category="tutorials">Tutorials</button>
   ```

2. Add cards with matching `data-category` attribute:
   ```html
   <article class="sample-card" data-category="tutorials">
   ```

## 📁 File Structure

```
docs-portfolio/
├── index.html          # Main portfolio page
└── README.md          # This file
```

## 🛠️ Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: Custom properties, Grid, Flexbox, animations
- **Vanilla JavaScript**: Filtering and scroll animations
- **Google Fonts**: Instrument Serif, Crimson Pro, IBM Plex Mono

## 🌐 Live Site Features

- **Tab Filtering**: Click category tabs to filter samples
- **Hover Effects**: Cards lift and show accent border on hover
- **Scroll Animations**: Content slides up as you scroll
- **Responsive Design**: Adapts seamlessly to all screen sizes
- **Fast Performance**: No frameworks, just optimized vanilla code

## 💡 Docs-as-Code Best Practices Demonstrated

This portfolio showcases modern documentation practices:

1. **Version Control**: All docs stored in Git
2. **CI/CD Integration**: Automated builds and deployments
3. **Code as Documentation**: Generated from source code
4. **Multiple Formats**: API specs, Markdown, MDX, YAML
5. **Toolchain Diversity**: MkDocs, Docusaurus, Sphinx, Hugo
6. **Automation**: Auto-generated from OpenAPI, JSDoc, godoc

## 📝 Customizing Content

### Update Header
Edit the header section in `index.html`:
```html
<h1>Your Name<br>Technical Writer</h1>
<p class="intro">Your personal introduction here...</p>
```

### Update Footer
Modify footer links:
```html
<a href="https://github.com/YOUR-USERNAME" class="footer-link">GitHub</a>
<a href="https://linkedin.com/in/YOUR-PROFILE" class="footer-link">LinkedIn</a>
```

## 🎯 SEO Optimization

The site includes:
- Semantic HTML5 markup
- Descriptive meta tags
- Proper heading hierarchy
- Alt text for images (when added)

To further optimize:
1. Add a `meta description` tag
2. Include Open Graph tags for social sharing
3. Add `sitemap.xml` for better indexing
4. Use descriptive, keyword-rich URLs for linked docs

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 🤝 Contributing

Feel free to fork this template and customize it for your own portfolio!

## 📄 License

Free to use and modify for your personal portfolio site.

---

**Pro Tip**: To make this portfolio truly shine, link each sample card to actual documentation you've written. Host them on GitHub Pages, ReadTheDocs, or other documentation platforms, then update the `sample-link` href attributes with the real URLs.
