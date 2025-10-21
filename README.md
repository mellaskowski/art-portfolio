# Art Portfolio Website

A modern, responsive art portfolio website showcasing artwork with interactive features and professional presentation.

## 🌐 Live Site
View the live website: **[https://mellaskowski.github.io/art-portfolio/](https://mellaskowski.github.io/art-portfolio/)**

## 📋 Table of Contents
- [Features](#features)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Pages Overview](#pages-overview)
- [Animation Controls](#animation-controls)
- [Customization](#customization)
- [Deployment](#deployment)
- [Contributing](#contributing)

## ✨ Features

### 🎨 Portfolio Showcase
- **Interactive Gallery** with filtering and modal view
- **Featured Artwork** sections on the homepage
- **Professional About Page** with artist biography and quote
- **Recommendations Page** showcasing favorite art spaces and organizations
- **Contact Form** for inquiries and commissions

### 🎭 Animation Controls
- **Pause/Resume GIFs** - User-friendly animation control system
- **Accessibility Focus** - Reduces motion for users who prefer it
- **Visual Feedback** - Clear indicators for paused states

### 📱 Responsive Design
- **Mobile-First Approach** - Optimized for all screen sizes
- **Modern UI/UX** - Clean, professional design with smooth transitions
- **Cross-Browser Compatible** - Works across all major browsers

### 🔧 Technical Features
- **Pure HTML/CSS/JavaScript** - No frameworks required
- **Semantic HTML** for accessibility
- **CSS Grid & Flexbox** for responsive layouts
- **Modern CSS** with custom properties and animations

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- A code editor (VS Code, Sublime Text, etc.)
- Optional: A local web server for development

### Clone and Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/mellaskowski/art-portfolio.git
   cd art-portfolio
   ```

2. **Open in your preferred editor**
   ```bash
   # For VS Code users
   code .
   
   # Or open the folder in any code editor
   ```

3. **View the website**
   
   **Option A: Direct File Opening**
   - Simply open `index.html` in your web browser
   - Double-click the file or right-click → "Open with" → Browser
   
   **Option B: Local Server (Recommended)**
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Python 2
   python -m SimpleHTTPServer 8000
   
   # Using Node.js (if you have http-server installed)
   npx http-server
   
   # Using PHP
   php -S localhost:8000
   ```
   
   Then open `http://localhost:8000` in your browser.

### Why Use a Local Server?
While the site works when opening files directly, a local server provides:
- Better handling of relative paths
- Proper MIME types for all assets
- More accurate testing environment
- Better performance for image loading

## 📁 Project Structure

```
art-portfolio/
├── index.html              # Homepage with featured artwork
├── gallery.html            # Full gallery with filtering
├── about.html              # Artist biography and information
├── recommendations.html     # Art spaces and organizations
├── contact.html            # Contact form and information
├── style.css              # Main stylesheet
├── images/                # Artwork and media files
│   ├── *.png             # Static artwork images
│   ├── *.gif             # Animated GIFs
│   ├── animated/         # Animated GIFs subfolder
│   └── photography/      # Photography subfolder
└── README.md             # This file
```

## 📄 Pages Overview

### 🏠 Homepage (`index.html`)
- Hero section with artist introduction
- Featured artwork showcase
- Animation control toggle
- Quick navigation to other sections

### 🖼️ Gallery (`gallery.html`)
- Complete artwork collection
- Filter by category (All, Photography, Digital Art, etc.)
- Modal lightbox view for detailed viewing
- Animation controls for GIFs

### 👤 About (`about.html`)
- Artist biography and background
- Inspirational quote from Yuri Kochiyama
- Professional presentation
- Links to other portfolio sections

### 🎯 Recommendations (`recommendations.html`)
- **Art Organizations**: National Coalition Against Censorship, Don't Delete Art
- **Local DC Galleries**: Rhizome (Queer art gallery), Folger Shakespeare Library, Brookland Arts Walk
- **Online Resources**: Artists' Rights Society and educational platforms
- Categorized with visual tags and direct links

### 📧 Contact (`contact.html`)
- Contact form for inquiries
- Professional contact information
- Social media links (placeholder)
- Commission inquiry options

## 🎮 Animation Controls

The website features a sophisticated animation control system:

### How It Works
1. **Pause Button**: Located in the top-right corner of each page
2. **Static Generation**: Creates high-quality static versions of GIFs
3. **Visual Feedback**: Paused animations show subtle desaturation
4. **Accessibility**: Helps users who prefer reduced motion

### Technical Implementation
- Canvas-based frame capture for static versions
- CSS fallback for browsers with restrictions
- Maintains image quality and aspect ratios
- Preserves user preferences across page navigation

## 🎨 Customization

### Adding New Artwork
1. Place images in the `images/` folder (organize in subfolders as needed)
2. Update the gallery in `gallery.html`:
   ```html
   <div class="artwork-item" data-category="your-category">
       <img src="images/your-artwork.jpg" alt="Description" class="artwork-image">
   </div>
   ```

### Updating Content
- **Artist Bio**: Edit the content in `about.html`
- **Featured Work**: Update the homepage sections in `index.html`
- **Recommendations**: Add new galleries/organizations in `recommendations.html`
- **Contact Info**: Update details in `contact.html`

### Styling Changes
- Main styles are in `style.css`
- CSS custom properties for easy color scheme changes
- Responsive breakpoints clearly marked
- Component-based organization

## 🚀 Deployment

### GitHub Pages (Current Setup)
The site is currently deployed using GitHub Pages:

1. **Automatic Deployment**: Pushes to `main` branch automatically deploy
2. **Custom Domain**: Can be configured in repository settings
3. **HTTPS**: Automatically enabled for security

### Alternative Deployment Options

**Netlify**
1. Connect your GitHub repository to Netlify
2. Deploy automatically on every push
3. Custom domain and form handling available

**Vercel**
1. Import project from GitHub
2. Automatic deployments and preview branches
3. Edge network for fast loading

**Traditional Hosting**
1. Upload all files to your web server
2. Ensure proper MIME types for all file extensions
3. Configure redirects if needed

## 🛠️ Development Tips

### Local Development
- Use a local server to avoid CORS issues
- Test on multiple devices and browsers
- Check console for any JavaScript errors

### Performance Optimization
- **Images**: Already optimized, but consider WebP format for better compression
- **CSS**: Minify for production deployment
- **JavaScript**: Consider bundling if adding more features

### Browser Support
- **Modern Browsers**: Full feature support
- **Older Browsers**: Graceful degradation for advanced features
- **Mobile**: Fully responsive and touch-friendly

## 📸 Image Guidelines

### Supported Formats
- **Static Images**: JPG, PNG, WebP
- **Animations**: GIF (with pause/play controls)
- **Photography**: High-resolution recommended

### Organization Tips
- Use descriptive filenames
- Organize by category in subfolders
- Keep file sizes reasonable for web loading
- Maintain consistent aspect ratios when possible

## 🤝 Contributing

### Making Changes
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-artwork`)
3. Make your changes
4. Test thoroughly in multiple browsers
5. Submit a pull request

### Reporting Issues
- Use GitHub Issues for bug reports
- Include browser and device information
- Provide steps to reproduce any problems

## 📝 License

This project is open source. Feel free to use it as inspiration for your own portfolio website.

## 🙏 Acknowledgments

- **National Coalition Against Censorship** - For defending artistic freedom
- **Rhizome DC** - Supporting queer artists in Washington, DC
- **Folger Shakespeare Library** - Combining literature, performance, and visual arts
- **Brookland Arts Walk** - Building community through public art
- **Yuri Kochiyama** - For the inspiring quote about bridging communities

---

**Live Site**: [https://mellaskowski.github.io/art-portfolio/](https://mellaskowski.github.io/art-portfolio/)

**Repository**: [https://github.com/mellaskowski/art-portfolio](https://github.com/mellaskowski/art-portfolio)
