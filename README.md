# Behind The Science Static Website

This is a static science news website called "Behind The Science" built with HTML, CSS, and JavaScript.

## Files Included

- `index.html` - Main HTML file with the website structure
- `styles.css` - CSS stylesheet with all styling and responsive design
- `script.js` - JavaScript for interactive features
- `README.md` - This file with instructions

## Features

✅ Responsive design (mobile, tablet, desktop)
✅ Mobile-friendly navigation menu
✅ Article card layout with category badges
✅ Sidebar widgets (Newsletter, Trending, Social)
✅ Pagination
✅ Smooth scrolling
✅ Animation on scroll
✅ Newsletter subscription form
✅ Social media integration
✅ Footer with multiple sections

## How to Use

1. **Simple Method**: Just open `index.html` in any web browser

2. **Local Server Method** (recommended):
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Python 2
   python -m SimpleHTTPServer 8000
   
   # Using Node.js
   npx serve
   ```
   Then open http://localhost:8000 in your browser

## Structure

```
.
├── index.html       # Main page
├── styles.css       # Styling
├── script.js        # Functionality
└── README.md        # Documentation
```

## Customization

### Colors
The color scheme is defined in CSS variables at the top of `styles.css`:
- `--primary-color`: Main brand color
- `--biology-color`, `--chemistry-color`, etc.: Category colors
- Modify these to change the entire color scheme

### Content
All articles and content are in `index.html`. You can:
- Add/remove article cards
- Modify trending news items
- Update footer links
- Change navigation items

### Features
The `script.js` file contains:
- Mobile menu toggle
- Newsletter form handling
- Smooth scrolling
- Scroll animations
- Social sharing functions

## Browser Compatibility

✅ Chrome/Edge (latest)
✅ Firefox (latest)
✅ Safari (latest)
✅ Mobile browsers (iOS Safari, Chrome Mobile)

## Notes

- This is a static version and doesn't include backend functionality
- Links are placeholders (use # anchors)
- Newsletter form shows an alert instead of actual subscription
- No actual search functionality (placeholder)
- Images would need to be added separately
- For a production site, you would need:
  - A backend for newsletter subscriptions
  - A CMS for article management
  - Image hosting
  - Search functionality
  - Analytics integration

## License

This is the Behind The Science website. All content and branding belong to Behind The Science.

## Credits

Behind The Science - Science, Space and Technology News
YouTube: https://www.youtube.com/@BehindTheScience_YT
Created as a modern science news platform
