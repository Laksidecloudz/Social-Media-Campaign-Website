# Social Media Campaigns Ltd. - Website Documentation

A modern, professional website for online safety education targeting teenagers, parents, and educators.

## 🎨 Design System

### Color Palette
The website uses a vibrant gradient color scheme:
- **Primary Purple**: `#8b5cf6` (violet-500)
- **Pink**: `#ec4899` (pink-500)
- **Teal**: `#14b8a6` (teal-500)
- **Blue**: `#3b82f6` (blue-500)
- **Cyan**: `#06b6d4` (cyan-500)

### Typography
- **Font Family**: [Outfit](https://fonts.google.com/specimen/Outfit) from Google Fonts
- **Weights**: 300, 400, 500, 600, 700, 800
- **Style**: Modern, geometric sans-serif perfect for teen audiences

### Gradients
- **Primary**: `linear-gradient(135deg, #8b5cf6 0%, #ec4899 50%, #14b8a6 100%)`
- **Secondary**: `linear-gradient(135deg, #3b82f6 0%, #06b6d4 100%)`
- **Hero**: Multi-color gradient for hero sections

## 📁 File Structure

```
Web_Files/
├── css/
│   └── styles.css          # Main stylesheet (28KB+) - Complete design system
├── js/
│   └── main.js             # Interactive features & animations
├── icons/
│   ├── facebook.png
│   ├── twitter.png
│   ├── instagram.png
│   ├── youtube.png
│   ├── rss.png
│   ├── Twitch.png
│   ├── Facebook Gaming.png
│   ├── YouTube Gaming.png
│   └── cursor-1.png
├── images/
│   └── [various images for content]
├── Home.html               # Homepage
├── Information.html        # About & Mission
├── Popular Apps.html       # App safety guides
├── Parents Help.html       # Resources for parents
├── Livestreaming.html      # Livestreaming safety
├── Contact.html            # Contact form & info
├── Legislation.html        # Laws & regulations
├── Privacy Policy.html     # Privacy policy
├── rss.xml                 # RSS feed
└── README.md               # This file
```

## 🚀 Features

### Core Features
- ✅ **Fully Responsive** - Perfect on mobile, tablet, and desktop
- ✅ **No Bootstrap** - Lightweight custom CSS (~28KB)
- ✅ **Modern Gradients** - Purple/Pink/Teal/Blue color scheme
- ✅ **Outfit Font** - Professional, teen-friendly typography
- ✅ **Smooth Animations** - Scroll-triggered animations, hover effects
- ✅ **Sticky Navigation** - Fixed header with scroll effects
- ✅ **Mobile Menu** - Hamburger menu for mobile devices
- ✅ **Scroll to Top** - Floating button for easy navigation
- ✅ **Card-based Layouts** - Modern, organized content presentation
- ✅ **Floating Particles** - Animated background effects

### Interactive Elements
- Mobile menu toggle with smooth animations
- Scroll-triggered fade-in animations
- Hover effects on cards, buttons, and links
- Form validation with real-time feedback
- Search functionality (on Popular Apps page)
- Interactive checklists
- Counter animations for statistics

### Accessibility
- Semantic HTML5 structure
- ARIA labels for interactive elements
- Keyboard navigation support
- Focus-visible styles
- Reduced motion support (`prefers-reduced-motion`)
- High contrast mode support

## 📱 Responsive Breakpoints

| Breakpoint | Width | Description |
|------------|-------|-------------|
| Mobile | < 480px | Single column, stacked layout |
| Mobile Large | < 768px | Adjusted typography, mobile menu |
| Tablet | < 992px | 2-column grids, hamburger menu |
| Desktop | < 1200px | Full layouts |
| Large Desktop | > 1200px | Max-width containers |

## 🎯 Pages Overview

### 1. Home.html
- Hero section with gradient text
- Statistics counter animation
- Feature cards with icons
- Safety tips section
- Campaigns manager CTA

### 2. Information.html
- Aims & Vision sections
- Why Online Safety Matters cards
- Additional resources links

### 3. Popular Apps.html
- App cards for major platforms (Twitter, Facebook, Instagram, Snapchat, WhatsApp, TikTok, YouTube, Twitch)
- Platform-specific safety tips
- Search functionality
- Universal safety tips

### 4. Parents Help.html
- Four key tips for parents
- Warning signs section
- Interactive checklist
- Parent resources

### 5. Livestreaming.html
- Embedded safety video
- Platform links (Twitch, Facebook Gaming, YouTube Gaming)
- Streaming safety tips
- Streamer checklist
- Parent streamer guidance

### 6. Contact.html
- Contact form with validation
- Branch location information
- Embedded map
- FAQ section
- Emergency help section

### 7. Legislation.html
- US legislation (COPPA, CIPA)
- UK/EU legislation (GDPR, Online Safety Bill)
- Best practices cards
- Digital rights & responsibilities

## 🛠️ CSS Architecture

### CSS Variables
All design tokens are stored in CSS custom properties for easy theming:

```css
:root {
  --color-purple: #8b5cf6;
  --color-pink: #ec4899;
  --color-teal: #14b8a6;
  --color-blue: #3b82f6;
  --gradient-primary: linear-gradient(135deg, var(--color-purple) 0%, var(--color-pink) 50%, var(--color-teal) 100%);
  /* ... more variables */
}
```

### Component Classes
- `.btn` - Button variants (primary, secondary, outline)
- `.card` - Card layouts with hover effects
- `.grid` - CSS Grid layouts (2, 3, 4 columns)
- `.section` - Page section containers
- `.nav-link` - Navigation links with hover effects
- `.animate-on-scroll` - Scroll-triggered animations

## 🔧 JavaScript Features

### Main.js Functions
- `initNavigation()` - Sticky header & mobile menu
- `initScrollEffects()` - Scroll-to-top button & smooth scroll
- `initAnimations()` - Intersection Observer for scroll animations
- `initParticles()` - Floating background particles
- `initSearch()` - Search functionality
- `initFormValidation()` - Form validation

### Utilities
- `debounce()` - Performance optimization
- `throttle()` - Scroll performance
- `Cookies` - Cookie management
- `Storage` - LocalStorage wrapper
- `Toast` - Notification system
- `Modal` - Modal dialog handling

## 🌐 Browser Support

- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- iOS Safari 14+
- Chrome Android 90+

## 📋 Usage Guide

### Adding a New Page
1. Copy the header and footer from an existing page
2. Update the page title and meta description
3. Add the active class to the appropriate nav link
4. Include `styles.css` and `main.js`
5. Update the breadcrumb in the footer

### Adding Content Cards
```html
<div class="card animate-on-scroll">
  <div class="card-icon">🎯</div>
  <h3 class="card-title">Card Title</h3>
  <p class="card-text">Card description...</p>
</div>
```

### Adding Animations
Add the `animate-on-scroll` class to any element:
```html
<div class="animate-on-scroll">Content fades in on scroll</div>
<div class="animate-on-scroll stagger-2">Content with delay</div>
```

### Using Buttons
```html
<a href="#" class="btn btn-primary">Primary Button</a>
<a href="#" class="btn btn-secondary">Secondary Button</a>
<a href="#" class="btn btn-outline">Outline Button</a>
```

## 🔐 Security Notes

- Forms include CSRF protection (implement server-side)
- All external links use `rel="noopener"`
- Form validation on client and server sides
- Privacy Policy linked on all forms

## 📝 License

&copy; 2024 Social Media Campaigns Ltd. All rights reserved.

## 🤝 Credits

- **Font**: [Outfit](https://fonts.google.com/specimen/Outfit) by Rodrigo Fuenzalida
- **Design System**: Custom built for SMC Ltd.
- **Icons**: Original icons and emoji-based icons
- **Images**: Original campaign images and assets

## 📞 Support

For questions or support, contact:
- Email: info@smc-ltd.com
- Emergency: help@smc-ltd.com
- Website: [Contact Page](Contact.html)

---

**Built with ❤️ for a safer online world.**
