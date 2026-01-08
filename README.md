# Academic Portfolio Website

A modern, professional academic portfolio website with a refined editorial aesthetic. This template is inspired by professional academic websites and features smooth animations, responsive design, and an elegant layout.

## Features

- 🎨 **Distinctive Design**: Editorial aesthetic with Cormorant Garamond serif font for headings and Work Sans for body text
- 📱 **Fully Responsive**: Works beautifully on desktop, tablet, and mobile devices
- ✨ **Smooth Animations**: Parallax effects, scroll animations, and smooth transitions
- 🧭 **Fixed Navigation**: Sticky navigation bar with active section highlighting
- 📄 **Multiple Sections**: Home, Research, Teaching, Experience, and Contact sections
- 🎯 **SEO Ready**: Semantic HTML structure for better search engine optimization
- ⚡ **Fast Loading**: Minimal dependencies, optimized performance

## File Structure

```
portfolio-website/
│
├── index.html          # Main HTML file
├── styles.css          # CSS styling
├── script.js           # JavaScript for interactions
└── README.md           # This file
```

## Getting Started

### 1. Prerequisites

You have already downloaded VS Code. Make sure you also have:
- A modern web browser (Chrome, Firefox, Safari, or Edge)
- Basic understanding of HTML/CSS (helpful but not required)

### 2. Setup

1. **Open VS Code**
2. **Open Folder**: File → Open Folder → Select the folder containing these files
3. **Install Live Server Extension** (recommended):
   - Click Extensions icon in left sidebar (or press Ctrl+Shift+X)
   - Search for "Live Server" by Ritwick Dey
   - Click Install

4. **View Your Website**:
   - Right-click on `index.html`
   - Select "Open with Live Server"
   - Your website will open in your default browser
   - Changes will auto-reload as you edit files

   **Alternative (without Live Server)**:
   - Simply double-click `index.html` to open in your browser
   - Refresh the page manually after making changes

## Customization Guide

### 1. Personal Information

Open `index.html` and replace:

- **Line 31**: `<a href="#" class="logo">Your Name</a>` → Your name
- **Lines 49-51**: Your name and title
- **Line 52**: Your position and university
- **Lines 65-88**: Your biography and research interests
- **All placeholder text**: Replace with your actual content

### 2. Profile Photo

Replace the placeholder in the hero section:

```html
<!-- Find this section around line 48 -->
<div class="image-placeholder">
    <!-- Replace the SVG with: -->
    <img src="your-photo.jpg" alt="Your Name" style="width: 100%; height: 100%; object-fit: cover;">
</div>
```

Add your photo file to the same folder as index.html.

### 3. Colors & Theme

Edit `styles.css` at the top (lines 2-10):

```css
:root {
    --color-primary: #1a1a2e;      /* Main dark color */
    --color-accent: #c7956d;        /* Accent color (links, highlights) */
    --color-background: #fdfcfb;    /* Page background */
    /* Adjust these to match your preference */
}
```

**Color Scheme Suggestions**:
- Academic Blue: `--color-accent: #2563eb;`
- Professional Green: `--color-accent: #059669;`
- Warm Burgundy: `--color-accent: #991b1b;`
- Modern Purple: `--color-accent: #7c3aed;`

### 4. Typography

To change fonts, edit the Google Fonts link in `index.html` (line 9):

```html
<link href="https://fonts.googleapis.com/css2?family=YOUR-FONT:wght@300;400;600;700&display=swap" rel="stylesheet">
```

Then update `styles.css` (lines 11-12):

```css
--font-display: 'YOUR-FONT', serif;
--font-body: 'YOUR-FONT', sans-serif;
```

**Font Recommendations**:
- Display fonts: Playfair Display, Crimson Pro, Lora, Merriweather
- Body fonts: Source Sans Pro, Open Sans, Roboto, Lato

### 5. Add Research Projects

In `index.html`, find the Research section (around line 99) and duplicate this block:

```html
<div class="research-card">
    <div class="card-number">04</div>
    <h3 class="card-title">Your Research Title</h3>
    <p class="card-description">
        Description of your research
    </p>
    <a href="#" class="card-link">Learn more →</a>
</div>
```

### 6. Add Teaching Experience

Find the Teaching section (around line 136):

```html
<div class="teaching-item">
    <div class="teaching-header">
        <h3 class="teaching-course">Course Name</h3>
        <span class="teaching-term">Semester Year</span>
    </div>
    <p class="teaching-description">
        Course description
    </p>
</div>
```

### 7. Update Contact Information

Find the Contact section (around line 177):

```html
<div class="contact-item">
    <span class="contact-label">Email</span>
    <a href="mailto:your.email@university.edu" class="contact-value">
        your.email@university.edu
    </a>
</div>
```

Update:
- Email address
- Office location
- Phone number
- Social media links (LinkedIn, Google Scholar, etc.)

## Advanced Customization

### Add New Sections

1. Add a navigation link in the `<nav>` section:
```html
<li><a href="#newsection" class="nav-link">New Section</a></li>
```

2. Create the section:
```html
<section id="newsection" class="new-section">
    <div class="container">
        <h2 class="section-title">New Section</h2>
        <!-- Your content here -->
    </div>
</section>
```

3. Add CSS styling in `styles.css`:
```css
.new-section {
    padding: 6rem 2rem;
    background: var(--color-white);
}
```

### Animations

The website includes several animations:
- **Disable animations**: Remove animation properties from CSS
- **Adjust speed**: Change animation duration (e.g., `0.8s` → `1.2s`)
- **Add more animations**: Use CSS `@keyframes` or JavaScript

### Mobile Menu

The mobile menu automatically appears on screens smaller than 768px. Customize the breakpoint in `styles.css`:

```css
@media (max-width: 768px) {
    /* Change 768px to your preferred breakpoint */
}
```

## Tips for Success

1. **Content First**: Write your content before worrying about design
2. **Professional Photo**: Use a high-quality, professional headshot
3. **Proofread**: Check for typos and grammatical errors
4. **Test Responsiveness**: View on different devices
5. **Keep It Updated**: Regularly update your research and publications
6. **Optimize Images**: Compress images for faster loading
7. **Backup**: Keep backups of your files

## Publishing Your Website

### Option 1: GitHub Pages (Free)
1. Create a GitHub account
2. Create a new repository named `yourusername.github.io`
3. Upload your files
4. Your site will be live at `https://yourusername.github.io`

### Option 2: University Hosting
Many universities provide web hosting for students/faculty. Check with your IT department.

### Option 3: Custom Domain
- Purchase a domain (e.g., yourname.com)
- Use services like Netlify, Vercel, or traditional hosting
- Point your domain to your hosting service

## Browser Compatibility

Tested and working on:
- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)

## Common Issues

**Q: Live Server not working?**
A: Make sure you've installed the Live Server extension and right-clicked on index.html

**Q: Animations not showing?**
A: Clear your browser cache (Ctrl+Shift+Delete)

**Q: Mobile menu not opening?**
A: Check that script.js is properly linked in index.html

**Q: Fonts not loading?**
A: Check your internet connection (Google Fonts requires internet)

## Need Help?

- **VS Code Tips**: Press Ctrl+Shift+P to open command palette
- **HTML/CSS Reference**: [MDN Web Docs](https://developer.mozilla.org)
- **Color Picker**: Use VS Code's built-in color picker (click on color codes)

## License

Free to use for personal and academic purposes. Please customize it to make it your own!

## Credits

Created with inspiration from professional academic portfolio websites. Designed with attention to typography, spacing, and user experience.

---

Good luck with your website! 🚀
