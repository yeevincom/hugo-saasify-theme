# Hugo Saasify Theme

A modern and elegant Hugo theme specifically designed for SaaS websites, built with TailwindCSS. This theme provides a clean, professional look while maintaining excellent performance and customization options.

## Features

- 🎨 Built with TailwindCSS for modern, responsive design
- 🚀 Optimized for performance
- 📱 Fully responsive design
- 🎯 Perfect for SaaS and business websites
- 💡 Clean and modern UI components
- 🛠 Easy to customize and extend

## Requirements

- Hugo version 0.80.0 or higher
- Node.js and npm for TailwindCSS processing

## Installation

1. Initialize a new Hugo site if you haven't already:
   ```bash
   hugo new site your-site-name
   cd your-site-name
   ```

2. Add the theme as a submodule:
   ```bash
   git submodule add https://github.com/yourusername/hugo-saasify-theme themes/hugo-saasify-theme
   ```

3. Configure your `hugo.toml`:
   ```toml
   baseURL = "/"
   languageCode = "en-us"
   title = "Your Site Title"
   theme = "hugo-saasify-theme"
   ```

## Development

1. Install dependencies:
   ```bash
   cd themes/hugo-saasify-theme
   npm install
   ```

2. Start development server:
   ```bash
   npm run dev
   ```

## Customization

The theme can be customized through:
- Hugo configuration in `hugo.toml`
- TailwindCSS configuration in `tailwind.config.js`
- Custom CSS in `assets/css/main.css`

## License

MIT
