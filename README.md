# Jekyll Resume for GitHub Pages

A clean, modern, and responsive resume built with Jekyll for GitHub Pages.

## 🚀 Quick Start

### 1. Repository Setup

Create a new repository named `yourusername.github.io` (replace `yourusername` with your GitHub username).

### 2. File Structure

Create the following directory structure in your repository:

```
yourusername.github.io/
├── _layouts/
│   └── default.html
├── assets/
│   └── css/
│       └── style.css
├── _config.yml
└── resume.html (or index.html)
```

### 3. Add Files

Copy the files to your repository:

- `default.html` → `_layouts/default.html`
- `style.css` → `assets/css/style.css`
- `_config.yml` → `_config.yml` (root directory)
- `resume.html` → `resume.html` or `index.html` (root directory)

### 4. Customize Your Resume

Edit `_config.yml` to add your information:

```yaml
# Personal Information
name: "Your Name"
email: "your.email@example.com"
phone: "+1 (555) 123-4567"
linkedin: "https://linkedin.com/in/yourprofile"
github: "https://github.com/yourusername"

# Professional Summary
summary: "Your professional summary here..."

# Technical Skills
technical_skills:
  - category: "Languages"
    items: "Python, JavaScript, etc."
  # Add more categories...

# Experience, Projects, Education, Certifications
# Update each section with your details
```

### 5. Deploy to GitHub Pages

1. Push all files to your repository
2. Go to repository Settings → Pages
3. Under "Source", select the branch (usually `main` or `master`)
4. Click Save
5. Your resume will be available at `https://yourusername.github.io/resume.html`

## 📋 Features

- ✅ Clean, professional design
- ✅ Fully responsive (mobile, tablet, desktop)
- ✅ Print-friendly with dedicated print styles
- ✅ One-click PDF download via print function
- ✅ ATS-friendly structure
- ✅ Easy to customize via YAML configuration
- ✅ No build process needed - works directly on GitHub Pages
- ✅ SEO optimized

## 🎨 Customization

### Change Colors

Edit `assets/css/style.css` to modify the color scheme:

```css
/* Primary color (links, accents) */
color: #2563eb;  /* Change this */

/* Headers */
color: #1a1a1a;  /* Change this */
```

### Add Sections

To add new sections, edit `resume.html` and add:

```html
<section class="section">
  <h2>New Section</h2>
  <!-- Your content here -->
</section>
```

### Using as Main Page

To make this your landing page, rename `resume.html` to `index.html`.

## 📱 Mobile & Print

The resume automatically adapts to:
- Mobile devices (responsive design)
- Tablets
- Desktop screens
- Print layout (PDF-ready)

Use the "Print / Download PDF" button to save as PDF or use your browser's print function (Ctrl/Cmd + P).

## 🔧 Local Development

To test locally before deploying:

```bash
# Install Jekyll
gem install bundler jekyll

# Create Gemfile
bundle init
bundle add jekyll

# Serve locally
bundle exec jekyll serve

# Visit http://localhost:4000/resume.html
```

## 📝 Tips

1. **Keep it concise**: Aim for 1-2 pages when printed
2. **Use metrics**: Quantify achievements with numbers
3. **Update regularly**: Keep your resume current
4. **Test printing**: Always check the print preview
5. **Mobile test**: View on different screen sizes
6. **Proofread**: Check for typos and formatting

## 🎯 SEO & Metadata

Add to `_config.yml` for better SEO:

```yaml
description: "Senior Software Engineer specializing in cloud infrastructure"
keywords: "software engineer, python, aws, kubernetes"
url: "https://yourusername.github.io"
```

## 📄 License

Feel free to use this template for your own resume!

## 🤝 Support

Issues or questions? Create an issue in the repository.
