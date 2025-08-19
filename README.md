# Terminal Portfolio Template

A modern developer portfolio template with a unique retro terminal aesthetic. Built with Astro 5.0 and Tailwind CSS, featuring customizable themes, smooth animations, and a cyberpunk-inspired design.

## ✨ Features

- **🖥️ Retro Terminal Design**: Authentic 80s computer terminal aesthetic
- **🎨 Dual Color Themes**: Toggle between green phosphor and amber CRT modes
- **⚡ Built with Astro 5.0**: Fast, modern, and SEO-friendly
- **🎯 Responsive Design**: Optimized for all device sizes
- **🔧 Customizable Animations**: Control panel for enabling/disabling effects
- **📝 Blog & Projects**: Built-in content management for showcasing work
- **🚀 Performance Optimized**: Lighthouse-perfect scores
- **♿ Accessible**: WCAG compliant with proper semantic markup

## 🚀 Quick Start

### Prerequisites
- Node.js (v18.17.1 or higher)
- pnpm (recommended) or npm

### Installation

1. **Clone or download this template**
   ```bash
   git clone <your-repo-url>
   cd terminal-portfolio-template
   ```

2. **Install dependencies**
   ```bash
   pnpm install
   ```

3. **Start development server**
   ```bash
   pnpm run dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:4321`

## 🛠️ Customization Guide

### 1. Basic Information

**Update site configuration** in `src/config.yaml`:
```yaml
site:
  name: Your Portfolio Name
  site: 'https://yourdomain.com'

metadata:
  title:
    default: Your Name - Developer Portfolio
  description: "Your description here"
  twitter:
    handle: '@yourhandle'
```

**Update package.json**:
```json
{
  "name": "your-portfolio-name",
  "description": "Your portfolio description"
}
```

### 2. Personal Content

**Home Hero Section** (`src/components/ContentComponents/HomeHero.astro`):
- Replace `[Your Name]` with your actual name
- Update the tagline and description
- Modify skillsets and tech stack
- Update project links

**About Section** (`src/components/ContentComponents/PersonalFacts.astro`):
- Customize the facts array with your background, interests, philosophy, and mission
- Modify section titles and content to match your experience

**Contact Information** (`src/pages/contact.astro`):
- Update the email address from `your.email@domain.com`
- Modify contact form behavior if needed

**Footer** (`src/components/Footer.astro`):
- Replace `[Your Name]` in the copyright notice

### 3. Content Management

**Blog Posts** (in `src/data/post/`):
- Remove sample posts and add your own
- Follow the frontmatter format in existing samples
- Add featured images to `/public/images/blog/`

**Projects** (in `src/data/projects/`):
- Replace sample projects with your actual work
- Update project images in `/public/images/projects/`
- Modify the MDX components to showcase your projects

### 4. Styling & Themes

**Theme Colors** (`tailwind.config.js`):
```javascript
colors: {
  terminal: {
    bg: {
      primary: '#0a0a0a',
      secondary: '#1a1a1a',
    },
    // Customize your color palette
  }
}
```

**Custom Fonts**: The template uses retro fonts like VT323 and Share Tech Mono. Update font imports in `src/assets/styles/base.css`.

**Animation Controls**: Users can toggle animations via the built-in control panel. Customize animation settings in the respective components.

### 5. Navigation

Update navigation links in `src/navigation.ts` (if using custom navigation) or modify the footer links in `src/components/Footer.astro`.

## 📁 Project Structure

```
/
├── public/                 # Static assets
│   ├── images/            # Image assets
│   └── fonts/             # Custom fonts
├── src/
│   ├── assets/            # Styles and assets
│   ├── components/        # Reusable components
│   │   ├── AnimationComponents/  # Terminal animations
│   │   ├── ContentComponents/    # Homepage sections
│   │   ├── TerminalComponents/   # Terminal UI elements
│   │   └── ProjectComponents/    # Project showcase
│   ├── content/           # Content collections (if using)
│   ├── data/              # Blog posts and projects
│   │   ├── post/          # Blog posts (.md)
│   │   └── projects/      # Project files (.mdx)
│   ├── layouts/           # Page layouts
│   ├── pages/             # File-based routing
│   ├── styles/            # Global styles
│   ├── utils/             # Utility functions
│   ├── config.yaml        # Site configuration
│   └── navigation.ts      # Navigation structure
├── astro.config.ts        # Astro configuration
├── tailwind.config.js     # Tailwind CSS config
└── package.json
```

## 🎨 Theme System

The template features a sophisticated theme system with two primary modes:

- **Green Phosphor**: Classic green-on-black terminal look
- **Amber CRT**: Warm amber retro computer aesthetic

Users can toggle between themes using the theme switcher component. The system uses CSS custom properties for easy customization.

## 🔧 Development Commands

```bash
# Development
pnpm run dev              # Start dev server
pnpm run dev-host        # Start dev server with external access

# Building
pnpm run build           # Build for production
pnpm run preview         # Preview production build

# Code Quality
pnpm run check           # Run all checks (Astro + ESLint + Prettier)
pnpm run check:astro     # Check Astro files
pnpm run check:eslint    # Run ESLint
pnpm run check:prettier  # Check Prettier formatting

# Fixing
pnpm run fix             # Fix all issues (ESLint + Prettier)
pnpm run fix:eslint      # Fix ESLint issues
pnpm run fix:prettier    # Fix Prettier formatting
```

## 🚀 Deployment

The template is optimized for deployment on:
- **Netlify** (recommended)
- **Vercel**
- **GitHub Pages**
- Any static hosting service

For Netlify, the `netlify.toml` configuration is already included.

## 🎯 Performance

The template is optimized for:
- ⚡ **Lighthouse Score**: 100/100 across all metrics
- 🔍 **SEO**: Comprehensive meta tags and structured data
- ♿ **Accessibility**: WCAG 2.1 AA compliant
- 📱 **Mobile-First**: Responsive design for all devices

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## 📄 License

This project is open source and available under the [MIT License](LICENSE.md).

## 🙏 Credits

- Built on top of the [AstroWind](https://github.com/onwidget/astrowind) template
- Terminal fonts and aesthetic inspired by retro computing
- Cyberpunk design elements from classic sci-fi media

## 🆘 Support

If you encounter any issues or have questions:
1. Check the existing issues on GitHub
2. Create a new issue with a detailed description
3. Include your environment details and steps to reproduce

---

**Made with ❤️ and lots of caffeine**

Transform your developer portfolio with this unique terminal-inspired template!