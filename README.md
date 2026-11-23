# Microsoft Ignite NYC 2025 - Conference Website

A professional, responsive HTML/CSS/JavaScript website for the Microsoft Ignite NYC 2025 one-day technology conference (November 13, 2025).

## Overview

Static website for Ignite NYC 2025. Edit `index.html` and add plain CSS, JavaScript, and other public assets in the repository root. No compilation or dependency installation is required. Use relative asset URLs so they work under the `/2025/` project path.

This website serves as the main hub for Microsoft Ignite NYC 2025, featuring:
- **Global Ignite Sessions** - Latest cloud, AI, and enterprise innovations
- **.NET Conf 2025 Content** - Modern .NET development and ecosystem updates
- **NYC Location** - Heart of Manhattan, combining Ignite branding with NYC imagery
- **One-Day Event** - November 13, 2025

## Features

✨ **Modern Design**
- Responsive design (mobile-first approach)
- Professional card-based layouts
- Smooth animations and transitions
- Ignite brand colors (Blue #0078D4, Purple #7928CA)
- NYC-inspired visual elements

🎯 **Core Sections**
1. **Navigation** - Sticky navbar with mobile toggle
2. **Hero** - Eye-catching event announcement with NYC + Ignite branding
3. **About** - Event details and key features
4. **Stats** - Quick event highlights with NYC skyline SVG
5. **Sessions** - Four conference tracks (Global Ignite, .NET Conf, AI, Cloud)
6. **Speakers** - Featured speaker profiles and presentation decks
7. **Schedule** - Full-day timeline (8 AM - 7 PM)
8. **Location** - Venue details, transit, accessibility info
9. **Registration** - Contact form with validation
10. **Footer** - Links, social media, branding

🔧 **Technology Stack**
- Pure HTML5 (no frameworks)
- CSS3 with CSS variables for theming
- Vanilla JavaScript for interactivity
- Font Awesome icons (CDN)
- No build tools or compilation needed

## File Structure

```
project-root/
├── index.html           # Main HTML file
├── styles.css          # All styling
├── script.js           # All JavaScript functionality
├── README.md           # This file
└── presentations/      # Directory for presentation decks (PDFs)
    ├── presentation1.pdf
    ├── presentation2.pdf
    └── ...
```

## Getting Started

### 1. Local Preview
Run a local web server from the repository root:

```bash
python3 -m http.server 8000
```

Then open <http://localhost:8000/> in your browser.

### 2. GitHub Pages Deployment

1. In **Settings → Pages → Build and deployment**, select **GitHub Actions**
   as the source (requires repository administrator access).
2. Merge site changes into `main`. The **Deploy static site to GitHub Pages**
   workflow publishes the repository directly, with no build step.
3. Visit <https://ignitenyc.github.io/2025/> after the deployment succeeds.

The workflow also supports manual runs from the **Actions** tab on `main`.
Pull requests do not deploy. Everything in the repository root except hidden
files and directories is included in the published artifact, so keep private
files out of the repository.

## Customization

### Colors
Edit CSS variables in `styles.css`:
```css
:root {
    --primary-color: #0078D4;      /* Microsoft Blue */
    --secondary-color: #7928CA;    /* Tech Purple */
    --accent-color: #FFD700;       /* NYC Yellow */
    --dark-color: #1F2937;
    --light-color: #F8F9FA;
}
```

### Event Details
Update these in `index.html`:
- Event date: "November 13, 2025"
- Venue address
- Session titles and descriptions
- Speaker names and titles
- Timeline/schedule items

### Links
- Global Ignite: https://ignite.microsoft.com
- .NET Conf: https://www.dotnetconf.net
- Social media links in footer

## JavaScript Features

✅ **Mobile Menu Toggle** - Responsive hamburger navigation
✅ **Smooth Scrolling** - Anchor link navigation
✅ **Form Validation** - Registration form with email validation
✅ **Notifications** - Toast-style alert system
✅ **Animations** - Intersection Observer for scroll animations
✅ **Parallax** - Subtle background parallax effect
✅ **Keyboard Navigation** - ESC to close menu
✅ **Performance** - Optimized animations with debouncing

## Accessibility

✓ Semantic HTML5 structure
✓ Proper heading hierarchy (h1, h2, h3)
✓ Alt text on all images
✓ ARIA labels where needed
✓ Keyboard navigation support
✓ Focus management
✓ Color contrast compliance
✓ Respects `prefers-reduced-motion`

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Android)
- IE 11 not supported (uses modern CSS/JS features)

## Performance

- No external CSS frameworks (lightweight)
- Minimal JavaScript (vanilla, no jQuery by default)
- Optimized images (compress before deploy)
- CSS Grid and Flexbox for layouts
- Lazy loading ready for images
- Page load typically < 2 seconds

## Registration Form

The registration form collects:
- Full Name (required)
- Email (required, validated)
- Phone (optional)
- Primary Interest (required) - dropdown selection

Form data can be:
1. Sent to your backend API (modify form submission in `script.js`)
2. Stored locally (modify form handler)
3. Integrated with services like Formspree, Netlify Forms, etc.

Currently logs to browser console for demo purposes.

## SEO

Meta tags included:
- Title: "Microsoft Ignite 2025 NYC Community Summit"
- Description: Event overview
- Viewport: Responsive design
- Theme color: Brand blue
- Open Graph tags for social media
- Twitter Card tags

## Social Media

Footer includes links to:
- Twitter (@microsoft)
- LinkedIn (Microsoft company page)
- YouTube (Microsoft channel)
- Instagram (@microsoft)

Update links as needed for your event accounts.

## Presentation Decks

Place PDF presentation files in the `presentations/` directory. These will be linked from the Decks section of the website.

## Troubleshooting

### Content not showing
- Ensure files are saved in the correct location
- Check browser console for errors
- Verify file paths are correct

### Mobile menu not working
- Check browser console for JavaScript errors
- Ensure `script.js` is loaded
- Test in different browser

### Form not submitting
- Check browser console for errors
- Verify email format validation
- Ensure all required fields are filled

### Styling issues
- Clear browser cache (Ctrl+Shift+Del)
- Check for CSS syntax errors
- Verify `styles.css` is loaded

## License

Microsoft Ignite NYC 2025 - Event website
© 2025 Microsoft Corporation

## Support

For questions or issues with this website:
1. Review browser console for error messages
2. Verify all files are present in correct locations
3. Test in different browser/device

---

**Version:** 1.0
**Last Updated:** November 23, 2025
**Created for:** Microsoft Ignite NYC 2025