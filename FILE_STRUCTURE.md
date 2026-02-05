# Jekyll Resume - File Structure

## 📁 Directory Structure

```
jekyll-resume/
├── _layouts/
│   └── default.html          # Base HTML template with header/footer
│
├── assets/
│   └── css/
│       └── style.css         # All styling (responsive + print)
│
├── _config.yml               # Site configuration & resume data (EDIT THIS!)
├── index.html                # Main resume page template
├── README.md                 # Documentation and instructions
├── Gemfile                   # Ruby dependencies for local development
├── .gitignore                # Files to exclude from git
└── deploy.sh                 # Quick deployment script

```

## 📝 File Descriptions

### Core Files (Required)

**_config.yml**
- Contains ALL your resume data (name, skills, experience, etc.)
- Edit this file to customize your resume
- Uses YAML format for easy editing

**index.html**
- Main resume template
- Pulls data from _config.yml
- Uses Liquid templating syntax
- Generally, you don't need to edit this unless changing layout

**_layouts/default.html**
- Base HTML structure
- Contains <head>, <body>, and footer
- Includes print button and metadata

**assets/css/style.css**
- All styling for the resume
- Responsive design (mobile, tablet, desktop)
- Print-optimized styles
- Customizable colors and fonts

### Supporting Files

**README.md**
- Complete setup and deployment instructions
- Customization tips
- Troubleshooting guide

**Gemfile**
- Ruby gem dependencies
- Only needed for local development
- GitHub Pages handles this automatically

**.gitignore**
- Excludes build files and caches
- Keeps repository clean

**deploy.sh**
- Optional automated deployment script
- Commits and pushes changes
- Makes updates easier

## 🎯 What to Edit

### For Most Users

**Only edit `_config.yml`** - this contains all your personal information:

```yaml
name: "Your Name"              # Your full name
email: "your@email.com"        # Your email
phone: "+1 (555) 123-4567"    # Your phone
linkedin: "https://..."        # Your LinkedIn URL
github: "https://..."          # Your GitHub URL
summary: "Your bio..."         # Professional summary

technical_skills:              # Your skills
  - category: "Languages"
    items: "Python, Java..."
  
experience:                    # Your work history
  - title: "Senior Engineer"
    company: "Company Name"
    # ... etc

# Continue editing all sections
```

### For Advanced Users

**Customize Layout** - Edit `index.html` to:
- Change section order
- Add new sections
- Modify structure

**Customize Styling** - Edit `assets/css/style.css` to:
- Change colors
- Modify fonts
- Adjust spacing
- Customize responsive breakpoints

**Customize Template** - Edit `_layouts/default.html` to:
- Add custom meta tags
- Include analytics
- Modify header/footer

## 🚀 Deployment Methods

### Method 1: Using deploy.sh (Easiest)

```bash
# Make changes to _config.yml
./deploy.sh
```

### Method 2: Manual Git Commands

```bash
git add .
git commit -m "Update resume"
git push origin main
```

### Method 3: GitHub Web Interface

1. Edit files directly on GitHub
2. Commit changes
3. Changes deploy automatically

## 🔧 Local Development

To preview locally before deploying:

```bash
# Install dependencies
bundle install

# Serve locally
bundle exec jekyll serve

# Visit http://localhost:4000
```

## 📱 Key Features

### Responsive Design
- Mobile: < 480px
- Tablet: 480px - 768px
- Desktop: > 768px

### Print Styles
- Optimized for PDF export
- Removes navigation/footer
- Adjusts font sizes
- Ensures content fits on pages

### Color Scheme
- Primary: #2563eb (blue)
- Text: #2c3e50 (dark gray)
- Links: #2563eb (blue)
- Backgrounds: #f8f9fa (light gray)

## 💡 Tips

1. **Keep it Updated**: Regularly update _config.yml with new experience
2. **Test Locally**: Preview changes before deploying
3. **Check Print**: Always verify PDF output looks good
4. **Mobile Test**: View on phone before deploying
5. **Backup**: Keep a local copy of your resume data

## 🆘 Troubleshooting

**Resume not showing:**
- Check GitHub Pages settings (Settings → Pages)
- Ensure source is set to main/master branch
- Wait 2-3 minutes for deployment

**Styling looks broken:**
- Verify file paths in default.html
- Check assets/css/style.css exists
- Clear browser cache

**Changes not appearing:**
- Wait a few minutes for GitHub Pages to rebuild
- Clear browser cache (Ctrl/Cmd + Shift + R)
- Check git push was successful

## 📞 Need Help?

Refer to the main README.md for detailed instructions and tips.
