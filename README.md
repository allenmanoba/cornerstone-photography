# Cornerstone Photography Website

A modern, professional real estate photography website built with vanilla HTML, CSS, and JavaScript. Designed with a dark, warm aesthetic inspired by the LOGE Camps brand.

## 📁 Project Structure

```
cornerstone-photography/
├── index.html                 # Homepage
├── services.html              # Services page
├── pricing.html               # Pricing page
├── gallery.html               # Portfolio gallery
├── contact.html               # Contact form
├── css/
│   └── styles.css            # Main stylesheet (all page styles)
├── js/
│   └── script.js             # Interactive features (mobile menu, animations, filtering)
├── .gitignore
└── README.md
```

## 🎨 Design System

### Color Palette
- **Background Primary**: #1a1a1a (Deep charcoal)
- **Background Secondary**: #2a2a2a (Lighter charcoal)
- **Accent Primary**: #c9954c (Warm gold/amber)
- **Accent Secondary**: #2d6a6a (Deep teal)
- **Text Primary**: #f5f0eb (Warm white)
- **Text Secondary**: #a8a29e (Muted grey)

### Typography
- **Headlines**: DM Serif Display (serif, warm & editorial)
- **Body**: DM Sans (clean, modern sans-serif)

## 🚀 Features

- ✅ Fully responsive design (mobile, tablet, desktop)
- ✅ Sticky navigation with scroll detection
- ✅ Scroll-triggered fade animations
- ✅ Mobile menu toggle
- ✅ Parallax hero background
- ✅ Gallery filtering by category
- ✅ Contact form with validation
- ✅ Dark theme with warm accents
- ✅ Accessibility features (ARIA labels, semantic HTML)
- ✅ Fast loading with lazy-loaded images

## 📱 Pages

### Homepage (index.html)
- Hero section with large property image
- 6 service cards grid
- "Why Cornerstone" section highlighting key benefits
- Call-to-action buttons throughout

### Services (services.html)
- Detailed breakdown of each service
- Split-layout design alternating image/content
- Individual service anchors for deep linking

### Pricing (pricing.html)
- 5 package tiers with pricing
- Feature lists for each package
- Pricing disclaimer (subject to change)

### Gallery (gallery.html)
- Filterable portfolio with 9 sample images
- Filter buttons: All, Interior, Exterior, Drone, Virtual Staging
- Responsive masonry-style grid

### Contact (contact.html)
- Contact form with validation
- Service selection dropdown
- Contact information card
- Business hours
- Map placeholder

## 🔧 Quick Start

1. Clone or download this repository
2. Open `index.html` in your browser to preview
3. All files are self-contained (no build process needed)

## ✏️ Customization

### Update Contact Information
Find and replace these placeholders:
- `[PHONE NUMBER]` → Your actual phone number
- `info@cornerstonephotography.com.au` → Your email address
- Business hours and location details in contact.html

### Update Images
Replace Unsplash placeholder images with your own:
- **Hero image** in index.html: Large property exterior shot
- **Service cards** in index.html: 6 images representing each service
- **Gallery images** in gallery.html: Your portfolio samples

### Update Brand Details
- Logo text "Cornerstone." in navbar
- Company name in footer
- Service descriptions
- Pricing packages

## 🎯 Performance

- All CSS inlined for critical styles
- Lazy loading on all images (`loading="lazy"`)
- Smooth scroll behavior
- CSS custom properties for easy theme adjustments
- Mobile-optimized with touch-friendly buttons

## 📋 Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📝 Notes

- Contact form currently shows an alert on submit. To make it functional, connect to a backend service (Formspree, Netlify Forms, etc.)
- Google Maps embed placeholder in contact page needs to be replaced with actual map iframe
- All prices shown are indicative (as of January 2023) and marked as subject to change

## 📄 License

This website template is provided for Cornerstone Photography's use.

---

**Last Updated**: April 2026  
**Status**: Ready for GitHub Pages deployment
