# Ibrahim Aromoye - Portfolio Website

A modern, responsive portfolio website for Ibrahim Aromoye, PhD Student in Autonomous Robotics at the University of Glasgow.

## Features

- **Modern Design**: Clean, professional layout with smooth animations
- **Responsive**: Fully responsive design that works on all devices
- **Interactive**: Smooth scrolling, hover effects, and dynamic animations
- **Accessible**: WCAG compliant with proper focus states and semantic HTML
- **Performance Optimized**: Lazy loading, debounced scroll events, and efficient animations

## Sections

1. **Hero Section**: Introduction with animated typing effect
2. **About**: Personal story and research interests
3. **Education**: Academic timeline with visual markers
4. **Experience**: Research and teaching experience cards
5. **Projects**: Featured projects with interactive cards
6. **Publications**: Research publications with status indicators
7. **Awards**: Honors and recognition
8. **Contact**: Contact form and professional links

## Technologies Used

- **HTML5**: Semantic markup structure
- **CSS3**: Modern styling with CSS Grid, Flexbox, and custom properties
- **JavaScript**: Interactive features and animations
- **Font Awesome**: Icons for enhanced visual appeal
- **Google Fonts**: Inter font family for typography

## Getting Started

1. Clone or download the project files
2. Open `index.html` in a web browser
3. No build process required - it's a static website

## File Structure

```
ibrahim-portfolio/
├── index.html          # Main HTML file
├── styles.css          # CSS styles and animations
├── script.js           # JavaScript functionality
└── README.md           # This file
```

## Customization

### Adding Your Photo
Replace the placeholder image in the hero section:
```html
<img src="path/to/your/photo.jpg" alt="Ibrahim Aromoye" id="profile-img">
```

### Updating Contact Information
Modify the contact section in `index.html`:
- Email addresses
- Location
- Social media links

### Adding New Projects
Add new project cards in the projects section:
```html
<div class="project-card">
    <div class="project-image">
        <img src="project-image.jpg" alt="Project Name">
    </div>
    <div class="project-content">
        <h3>Project Title</h3>
        <p>Project description...</p>
        <div class="project-tech">
            <span class="tech-tag">Technology</span>
        </div>
    </div>
</div>
```

### Color Scheme
The website uses CSS custom properties for easy theming. Modify the `:root` variables in `styles.css`:
```css
:root {
    --primary-color: #4f46e5;
    --secondary-color: #10b981;
    --accent-color: #8b5cf6;
    /* ... other variables */
}
```

## Browser Support

- Chrome 60+
- Firefox 60+
- Safari 12+
- Edge 79+

## Performance Features

- **Lazy Loading**: Images load only when needed
- **Debounced Scroll Events**: Optimized scroll performance
- **CSS Animations**: Hardware-accelerated animations
- **Minimal Dependencies**: Only essential external resources

## Accessibility Features

- **Semantic HTML**: Proper heading structure and landmarks
- **Keyboard Navigation**: Full keyboard accessibility
- **Focus Indicators**: Clear focus states for interactive elements
- **Alt Text**: Descriptive alt text for all images
- **Color Contrast**: WCAG AA compliant color combinations

## Deployment

### GitHub Pages
1. Upload files to a GitHub repository
2. Enable GitHub Pages in repository settings
3. Select source branch (usually `main`)

### Netlify
1. Drag and drop the project folder to Netlify
2. Or connect your GitHub repository for automatic deployments

### Vercel
1. Import project from GitHub
2. Deploy with zero configuration

## Contact

For questions about this portfolio template or customization requests, please contact:
- Email: ibrahim.aromoye@postgrad.manchester.ac.uk
- Email: aromoyeibm@gmail.com

## License

This portfolio template is free to use and modify for personal and commercial projects.

---

**Note**: This is a template created for Ibrahim Aromoye. Please customize all personal information, images, and content to match your own profile.
