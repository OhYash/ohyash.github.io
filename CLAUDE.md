# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a personal portfolio website for Yash Yadav, built as a static HTML site using the Strata template from HTML5 UP. The website showcases personal projects, work experience, education, and contact information.

## Architecture

- **Static HTML Site**: Single-page application with no build process required
- **Template**: Based on Strata by HTML5 UP with CCA 3.0 license
- **Styling**: SCSS-based styling system with modular structure
- **Layout**: Fixed sidebar header with scrollable main content area
- **Responsive**: Mobile-first design with breakpoint-based responsive behavior

## File Structure

### Core Files
- `index.html` - Main HTML file containing all content sections
- `assets/css/main.css` - Compiled CSS (do not edit directly)
- `assets/sass/main.scss` - Main SCSS entry point
- `assets/sass/libs/` - SCSS utility libraries (_vars.scss, _mixins.scss, etc.)

### Content Assets
- `images/` - Portfolio images, thumbnails, and personal photos
- `assets/Documents/` - Resume PDFs
- `assets/js/` - JavaScript libraries and custom scripts

### Key Sections in index.html
1. **Header (#header)** - Fixed sidebar with avatar and introduction
2. **About (#one)** - Personal introduction and links
3. **Projects (#two)** - Portfolio grid with project thumbnails
4. **Work Experience (#three)** - Professional experience timeline
5. **Education (#four)** - Education and certifications
6. **Contact (#five)** - Contact form and information
7. **Footer** - Social links and copyright

## Styling System

The SCSS follows a modular architecture:
- `_vars.scss` - Color palette, typography, and size variables
- `_mixins.scss` - Reusable SCSS mixins
- `_breakpoints.scss` - Responsive breakpoint definitions
- `main.scss` - Main styles importing all modules

### Key Design Elements
- **Responsive breakpoints**: xlarge (1281px+), large (981-1280px), medium (737-980px), small (481-736px), xsmall (<481px)
- **Fixed header width**: 35% on desktop, full width on mobile
- **Image overlays**: Hover effects on portfolio thumbnails
- **Form styling**: Custom styled form elements with focus states

## Development Workflow

### Making Style Changes
1. Edit SCSS files in `assets/sass/`
2. Compile SCSS to CSS (requires Sass compiler)
3. Test responsive behavior across breakpoints

### Adding Portfolio Items
1. Add images to `images/fulls/` and `images/thumbs/`
2. Update the project grid in index.html section #two
3. Follow existing article structure with image, title, and description

### Content Updates
- **Resume**: Replace `Yash_Resume.pdf` and update links
- **Contact**: Update form action URL and contact details
- **Social Links**: Update footer and header social media links

## External Dependencies

- **Fonts**: Source Sans Pro from Google Fonts
- **Icons**: Font Awesome (included locally)
- **JavaScript Libraries**: jQuery, Poptrox (image gallery), breakpoints detection
- **Form Handling**: Formspree (https://formspree.io/mdopnppj)
- **Analytics**: Google Analytics with custom implementation

## Browser Support

Designed for modern browsers with vendor prefixes for:
- CSS transitions and animations
- Flexbox layout
- CSS Grid (html-grid mixin)
- Background-attachment and other modern properties

## Mobile Considerations

- Touch-optimized image gallery behavior
- Collapsible navigation on small screens
- Responsive typography scaling
- Mobile-optimized form layouts