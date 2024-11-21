# Hugo Saasify Theme

A modern and elegant Hugo theme specifically designed for SaaS websites. Built with TailwindCSS, this theme provides a clean, professional look while maintaining excellent performance and customization options.

![Hugo Saasify Theme Screenshot](https://raw.githubusercontent.com/chaoming/hugo-saasify-theme/main/images/screenshot.png)

![Hugo Saasify Theme Screenshot 2](https://raw.githubusercontent.com/chaoming/hugo-saasify-theme/main/screenshots/screenshot2.png)

![Hugo Saasify Theme Screenshot 3](https://raw.githubusercontent.com/chaoming/hugo-saasify-theme/main/screenshots/screenshot3.png)

[Demo Site](https://saasify-demo.chaoming.li)

## Features

- 🎨 Modern design with TailwindCSS
- 📱 Fully responsive layout
- 🚀 Performance optimized
- 💅 Clean typography with Inter & Plus Jakarta Sans fonts
- 🎯 Perfect for SaaS and business websites
- 🛠 Easy to customize
- 📦 No jQuery, minimal JavaScript

## Requirements

- Hugo Extended Version (>= 0.80.0)
- Node.js (>= 14.x)
- npm or yarn

## Installation

### 1. Create a new Hugo site (skip if you have an existing site)

```bash
hugo new site your-site-name
cd your-site-name
```

### 2. Add the theme as a submodule

```bash
git init
git submodule add https://github.com/chaoming/hugo-saasify-theme themes/hugo-saasify-theme
```

### 3. Install dependencies

```bash
# Copy package.json and other config files to your site root
cp themes/hugo-saasify-theme/package.json .
cp themes/hugo-saasify-theme/postcss.config.js .
cp themes/hugo-saasify-theme/tailwind.config.js .

# Install dependencies
npm install
```

### 4. Configure your Hugo site

Create or update your `hugo.toml` with the following configuration:

```toml
baseURL = "/"
languageCode = "en-us"
title = "Your Site Title"
theme = "hugo-saasify-theme"

[params]
  description = "Your site description"
  author = "Your Name"

[module]
  [module.hugoVersion]
    extended = true
    min = "0.80.0"
```

## Development

To start the development server with live reload:

```bash
npm run start
```

This will:
- Watch for changes in your TailwindCSS styles
- Run the Hugo development server
- Automatically rebuild when changes are detected

## Customization

### Colors

The theme uses a primary and secondary color scheme that can be customized in `tailwind.config.js`:

```js
colors: {
  primary: {
    // Your primary color palette
  },
  secondary: {
    // Your secondary color palette
  }
}
```

### Typography

The theme uses Inter for body text and Plus Jakarta Sans for headings. You can modify this in `tailwind.config.js`:

```js
fontFamily: {
  sans: ['Inter', 'system-ui', 'sans-serif'],
  heading: ['Plus Jakarta Sans', 'sans-serif'],
}
```

### Layout Components

Common components like buttons, cards, and sections can be customized in `assets/css/main.css`.

## Content Structure

```
content/
├── _index.md          # Homepage content
├── blog/              # Blog posts
├── features/          # Feature pages
└── docs/              # Documentation pages
```

## License

This theme is released under the [MIT license](https://github.com/chaoming/hugo-saasify-theme/blob/main/LICENSE).

## Support

If you have any questions or need help, please [open an issue](https://github.com/chaoming/hugo-saasify-theme/issues).
