# Copilot Instructions for amike-portfolio

## Project Overview
This is a **personal portfolio website** for Jonathan Doe (template). It's a single-page HTML application with planned expandable sections for showcasing professional work, services, and contact information.

## Architecture & Structure

### Current Layout
- **`index.html`** - Main entry point with semantic HTML5 sections:
  - Header: Navigation menu with 7 nav items (links currently empty)
  - Main: Contains 6 planned sections (`#home`, `#about`, `#services`, `#portfolio`, `#skills`, `#contact`, `#blog`)
  - Services section has 6 card-based items with FontAwesome icons
  - Footer: Currently empty
- **`images/`** - Asset folder containing logo, profile images
- **`pages/`** - Empty folder, reserved for potential additional pages

### Technology Stack
- **HTML5** with semantic structure and OpenGraph-ready metadata
- **FontAwesome Icons** (v6 - CDN: `kit.fontawesome.com/824082b16c.js`)
- **Responsive Design** - Uses `<meta viewport>` tag
- **No styling/JS** - Currently unstyled; CSS and JavaScript files not yet created

## Key Patterns & Conventions

### HTML Structure Pattern
All page sections follow a similar pattern - top descriptive part, bottom content grid:
```html
<section id="sectionName">
    <div><!-- Header/description --></div>
    <div><!-- Content --></div>
</section>
```

### Social Media Icons
Located in home section using FontAwesome brands: Facebook, Twitter, Pinterest, Instagram, Behance

### Image Assets
- Store in `images/` folder with descriptive names (logo.png, profile-img.png, mansmiling.png)
- Always use relative paths: `src="./images/filename.png"`
- Include meaningful alt text for accessibility

### Navigation
- Nav items in header should link to corresponding section IDs
- Current nav items: Home, About, Service, Portfolio, Skills, Contact, Blog
- Update href attributes when adding new pages or sections

## Development Notes

### Incomplete Sections
These sections have HTML structure but no content:
- `#portfolio` - Needs portfolio grid/showcase
- `#skills` - Needs skill bars or list
- `#contact` - Needs contact form
- `#blog` - Needs blog grid
- Footer - Empty, needs content

### Next Steps (Common Tasks)
1. **Add CSS styling** - Create `style.css`, link in `<head>`
2. **Create contact form** - Build in `#contact` section with validation
3. **Add animations** - Smooth scrolling, fade-in effects when content added
4. **Implement responsive design** - Mobile-first approach for small screens
5. **Update navigation links** - Connect nav items to section IDs

### Asset Additions
When adding images:
- Place in `images/` directory
- Use lowercase filenames with hyphens: `profile-pic.png` (not `profilePic.png`)
- Keep file sizes optimized for web (< 100KB for thumbnails)
