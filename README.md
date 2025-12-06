# 🎮 Call of Duty Website Clone

<div align="center">

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

**A stunning, pixel-perfect clone of the Call of Duty website featuring a dark gaming aesthetic, custom cursor system, and immersive video hero section.**

[Features](#-features) • [Demo](#-demo) • [Installation](#-installation) • [Project Structure](#-project-structure) • [Technologies](#-technologies-used)

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [Technologies Used](#-technologies-used)
- [Project Structure](#-project-structure)
- [Installation](#-installation)
- [Key Features Breakdown](#-key-features-breakdown)
- [Custom Cursor System](#-custom-cursor-system)
- [Design Highlights](#-design-highlights)
- [Browser Support](#-browser-support)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🎯 Overview

This project is a meticulously crafted clone of the Call of Duty official website, featuring:

- **Immersive Hero Section** with full-screen video background
- **Custom Cursor System** with white glow for visibility on dark backgrounds
- **Responsive Design** that works seamlessly across all devices
- **Modern UI/UX** with smooth animations and hover effects
- **Gaming Aesthetic** with dark theme and futuristic typography

---

## ✨ Features

### 🎨 Visual Features
- ✅ **Full-screen video hero** with gradient overlays
- ✅ **Custom cursor** with white glow effect for dark backgrounds
- ✅ **Smooth animations** and transitions throughout
- ✅ **Responsive navigation** with dropdown menu
- ✅ **Game showcase grid** with hover effects
- ✅ **News feature cards** with modern design
- ✅ **Dark theme** optimized for gaming aesthetic

### 🚀 Technical Features
- ✅ **Zero horizontal scroll** - perfectly optimized layout
- ✅ **Mobile-first responsive** design
- ✅ **Performance optimized** with efficient CSS
- ✅ **Accessibility features** with proper ARIA labels
- ✅ **SEO friendly** structure
- ✅ **Cross-browser compatible**

### 🎯 Interactive Elements
- ✅ **Hover effects** on all interactive elements
- ✅ **Custom cursor tracking** with glow highlight
- ✅ **Smooth scrolling** navigation
- ✅ **Icon integration** (FontAwesome & Bootstrap Icons)
- ✅ **Button animations** with lift effects

---

## 🛠 Technologies Used

### Core Technologies
- **HTML5** - Semantic markup structure
- **CSS3** - Advanced styling with:
  - Flexbox & CSS Grid
  - Custom properties
  - Advanced selectors
  - Pseudo-elements
  - Transform & transitions
  - Mix-blend-mode
  - Filter effects

### External Libraries
- **Google Fonts**
  - Orbitron (Headings, buttons)
  - Rajdhani (Body text)
- **FontAwesome 6.5.1** - Icon library
- **Bootstrap Icons 1.11.2** - Additional icon set

### JavaScript
- **Vanilla JavaScript** - Minimal cursor tracking script

---

## 📁 Project Structure

```
GameWebClone/
├── index.html              # Main HTML file
├── README.md              # Project documentation
└── assets/
    ├── css/
    │   └── main.css       # All styles (976 lines)
    ├── images/
    │   ├── cursor.png     # Custom cursor image
    │   └── logo.svg       # Call of Duty logo
    ├── videos/
    │   └── hero-video.mp4 # Hero section video
    └── favicon.svg        # Site favicon
```

---

## 🚀 Installation

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- A local web server (optional, for video playback)

### Quick Start

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd GameWebClone
   ```

2. **Open the project**
   - Simply open `index.html` in your web browser
   - Or use a local server:
     ```bash
     # Using Python
     python -m http.server 8000
     
     # Using Node.js (http-server)
     npx http-server
     
     # Using PHP
     php -S localhost:8000
     ```

3. **View the site**
   - Navigate to `http://localhost:8000` (if using a server)
   - Or open `index.html` directly in your browser

### No Build Process Required!
This is a pure HTML/CSS/JS project with no dependencies or build steps needed.

---

## 🔍 Key Features Breakdown

### 1. Hero Section
- **Full-screen video background** with autoplay and loop
- **Gradient overlays** on left, right, and bottom edges
- **Centered navigation bar** with glassmorphism effect
- **Responsive height** adjustments for different screen sizes

### 2. Navigation System
- **Three-section layout**: Menu, Main nav, Action buttons
- **Dropdown menu** with hover activation
- **Responsive behavior** - adapts to mobile screens
- **Icon integration** for better visual communication

### 3. Game Showcase
- **Responsive grid layout** using CSS Grid
- **Auto-fit columns** that adapt to screen size
- **Hover effects** with image zoom and shadow
- **Game cards** featuring Call of Duty titles

### 4. News Section
- **Feature card** with large article preview
- **Side cards** for additional news items
- **Tag system** with color coding
- **Read more links** with arrow icons

### 5. Custom Cursor System
- **Custom cursor image** replaces default pointer
- **White glow highlight** follows mouse movement
- **Enhanced visibility** on dark backgrounds
- **Interactive element highlighting** on hover

---

## 🖱 Custom Cursor System

The project features an advanced cursor visibility system designed for dark backgrounds:

### Features
- **Custom cursor image** (`cursor.png`) replaces default pointer
- **White glow highlight** that tracks mouse movement
- **Multiple shadow layers** for maximum visibility
- **Mix-blend-mode** for better contrast
- **Smooth transitions** for professional feel

### Implementation
```css
/* Custom cursor */
cursor: url("../images/cursor.png"), auto;

/* Glow highlight */
.cursor-highlight {
  position: fixed;
  background: radial-gradient(...);
  filter: blur(12px);
  box-shadow: 0 0 40px rgba(255, 255, 255, 0.9), ...;
  mix-blend-mode: screen;
}
```

### JavaScript Tracking
```javascript
document.addEventListener("mousemove", (e) => {
  cursorHighlight.style.left = e.clientX + "px";
  cursorHighlight.style.top = e.clientY + "px";
  cursorHighlight.style.opacity = "1";
});
```

---

## 🎨 Design Highlights

### Color Palette
- **Background**: `#050505` (Deep black)
- **Cards**: `#111214`, `#0c0d0f` (Dark grays)
- **Accents**: `#b2ffba` (Green glow)
- **Text**: `#ffffff`, `#f5f5f5` (White/light gray)
- **Gradients**: Multiple dark-to-light transitions

### Typography
- **Headings**: Orbitron (Futuristic, gaming font)
- **Body**: Rajdhani (Clean, modern sans-serif)
- **Weights**: 300-900 for various emphasis levels

### Spacing & Layout
- **Container max-width**: 1040px - 1400px
- **Responsive breakpoints**: 480px, 768px, 1024px
- **Consistent padding**: 20px - 46px based on screen size
- **Grid gaps**: 16px - 32px for card spacing

### Effects
- **Box shadows**: Multiple layers for depth
- **Text shadows**: White glow on hover
- **Transforms**: Scale, translate for animations
- **Transitions**: 0.2s - 0.3s for smooth feel

---

## 📱 Responsive Design

The site is fully responsive with breakpoints at:

- **Mobile**: < 480px
  - Single column layout
  - Hidden navigation text
  - Reduced padding
  - Stacked elements

- **Tablet**: 481px - 768px
  - 2-column game grid
  - Adjusted navigation
  - Medium padding

- **Desktop**: > 768px
  - 4-column game grid
  - Full navigation
  - Optimal spacing

---

## 🌐 Browser Support

| Browser | Version | Status |
|---------|---------|--------|
| Chrome  | Latest  | ✅ Fully Supported |
| Firefox | Latest  | ✅ Fully Supported |
| Safari  | Latest  | ✅ Fully Supported |
| Edge    | Latest  | ✅ Fully Supported |
| Opera   | Latest  | ✅ Fully Supported |

**Note**: Some advanced CSS features (mix-blend-mode, filter) may have limited support in older browsers.

---

## 🎯 Performance

- **No external dependencies** (except CDN fonts/icons)
- **Optimized CSS** with efficient selectors
- **Minimal JavaScript** (only cursor tracking)
- **Efficient animations** using transform/opacity
- **Lazy loading ready** for images/videos

---

## 🔧 Customization

### Changing Colors
Edit the CSS variables and color values in `assets/css/main.css`:
```css
background-color: #050505; /* Main background */
color: #ffffff; /* Text color */
```

### Modifying Cursor
Replace `assets/images/cursor.png` with your custom cursor image.

### Adding Content
Edit `index.html` to add new sections or modify existing content.

### Styling Adjustments
All styles are in `assets/css/main.css` - modify as needed.

---

## 📝 Code Quality

- ✅ **Semantic HTML5** structure
- ✅ **Organized CSS** with clear sections
- ✅ **Clean JavaScript** with comments
- ✅ **No linter errors**
- ✅ **Accessibility considerations**
- ✅ **Mobile-first approach**

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

This project is created for educational purposes as a clone/recreation of the Call of Duty website. 

**Note**: This is a fan-made project and is not affiliated with or endorsed by Activision Publishing, Inc. or Call of Duty.

---

## 👨‍💻 Author

Created with ❤️ for the gaming community

---

## 🙏 Acknowledgments

- **Activision Publishing, Inc.** - For the original Call of Duty website design inspiration
- **Google Fonts** - For the amazing typography
- **FontAwesome & Bootstrap Icons** - For the icon libraries
- **The gaming community** - For the inspiration

---

## 📞 Support

If you have any questions or suggestions, please feel free to open an issue or contact the maintainers.

---

<div align="center">

**Made with 🎮 passion for gaming**

⭐ Star this repo if you found it helpful!

</div>

