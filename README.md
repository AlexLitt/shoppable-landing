# Webflow Export Package

This package contains all the files needed to recreate the hero section and trusted brands section in Webflow.

## Files Included

### HTML
- `index.html` - Complete HTML structure for the hero and trusted brands sections

### CSS
- `styles.css` - All styling for the sections with responsive design

### Assets
- `assets/hero_video.mp4` - Main hero video
- `assets/logo-flag.svg` - Vidalytics logo
- `assets/images/hero_video_card.png` - Video poster image
- `assets/images/editor_sidebar.png` - Dashboard screenshot
- `assets/images/seamlessly integrated-min-1.webp` - Integration image
- `assets/images/clients-logo/` - All client logo images (logo1.jpeg through logo6.png)

## How to Use in Webflow

### Option 1: Custom Code (Recommended)
1. **Upload Assets**: Upload all files from the `assets/` folder to your Webflow project assets
2. **Add Custom Code**: 
   - Go to Project Settings > Custom Code
   - Copy the entire contents of `styles.css` and paste it in the Head Code section wrapped in `<style>` tags:
     ```html
     <style>
     /* Paste all CSS content here */
     </style>
     ```
3. **Add HTML Structure**:
   - Create a new page or section
   - Add an Embed element
   - Copy the HTML content from `index.html` (everything inside the `<body>` tags)
   - Update asset paths to match your Webflow asset URLs

### Option 2: Native Webflow Elements
1. **Upload Assets**: Upload all files from the `assets/` folder to your Webflow project
2. **Recreate Structure**:
   - Create sections with the classes from the HTML
   - Add div blocks with the appropriate class names
   - Style each element using the Webflow Designer, referencing the CSS file for values
3. **Update Asset References**: Replace asset paths with your Webflow asset URLs

## Key Features

### Hero Section
- Responsive grid layout (60/40 split on desktop)
- Maximum height constraint (75vh)
- Auto-playing background video
- Call-to-action buttons with hover effects

### Trusted Brands Section
- Infinite scrolling logo carousel
- Responsive logo cards
- Conversion-focused content section
- Mobile-optimized layout

## CSS Variables Used
- `--sv-container: 1280px` - Maximum container width
- `--sv-gutter: 32px` - Side padding
- `--sv-py: 96px` - Vertical section padding
- `--sv-yellow: #FFD24A` - Primary accent color
- `--sv-ink: #0B0F1A` - Dark background color

## Responsive Breakpoints
- Mobile: max-width 767px
- Tablet: 768px - 1023px
- Desktop: 1024px+
- Large Desktop: 1280px+

## Notes
- All animations are CSS-only (no JavaScript required)
- Video autoplay is set with appropriate fallbacks
- All images are optimized for web
- Color scheme uses CSS custom properties for easy theming
- Accessibility features included (ARIA labels, focus states)

## Customization
- Update colors by changing CSS custom properties
- Adjust spacing by modifying the `--sv-py` and `--sv-gap` variables
- Replace logos by swapping image files in the clients-logo folder
- Modify text content directly in the HTML

## Browser Support
- Modern browsers (Chrome, Firefox, Safari, Edge)
- CSS Grid and Flexbox support required
- CSS custom properties support required
