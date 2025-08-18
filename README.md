# RevealJS Slides with Tailwind CSS

A modern presentation framework built with RevealJS, Tailwind CSS, and shadcn design tokens.

## Features

- 🎯 **RevealJS** - Powerful HTML presentation framework
- 🎨 **Tailwind CSS** - Utility-first CSS framework
- 🌙 **shadcn Themes** - Beautiful color system with light/dark mode support
- ⚡ **Fast Development** - Hot reload and build scripts included

## Quick Start

1. **Install dependencies:**
   ```bash
   npm install
   ```

2. **Start development server:**
   ```bash
   npm run serve
   ```

3. **Open your browser:**
   Navigate to `http://localhost:8010`

## Development

### Available Scripts

- `npm run dev` - Watch and rebuild CSS on changes
- `npm run build` - Build minified CSS for production
- `npm run serve` - Start local development server

### Project Structure

```
slides/
├── index.html          # Main presentation file
├── styles.css          # Source Tailwind CSS
├── dist/
│   └── styles.css      # Compiled CSS output
├── tailwind.config.js  # Tailwind configuration
└── postcss.config.js   # PostCSS configuration
```

## Customization

### Theme Colors

The project uses shadcn color variables. Customize colors in `styles.css`:

```css
:root {
    --background: 0 0% 100%;
    --foreground: 0 0% 3.9%;
    --primary: 0 0% 9%;
    /* ... more variables */
}
```

### Adding New Slides

Edit the `index.html` file and add new `<section>` elements:

```html
<section>
    <h2 class="text-4xl font-semibold mb-6">Your Title</h2>
    <p class="text-xl">Your content with Tailwind classes</p>
</section>
```

### Tailwind Classes

Use any Tailwind utility classes with shadcn color tokens:

- `bg-primary` - Primary background color
- `text-muted-foreground` - Muted text color
- `border-border` - Border color
- `bg-card` - Card background

## RevealJS Configuration

Modify presentation settings in the `<script>` section of `index.html`:

```javascript
Reveal.initialize({
    hash: true,
    transition: 'slide',
    transitionSpeed: 'default',
    backgroundTransition: 'fade'
});
```

## Building for Production

1. Build optimized CSS:
   ```bash
   npm run build
   ```

2. Deploy the entire project folder to your hosting provider

## License

ISC