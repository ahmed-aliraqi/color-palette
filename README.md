# SCSS Color Palette Plugin

A powerful SCSS plugin that automatically generates comprehensive color utility classes with customizable shade variations. Perfect for design systems and utility-first CSS frameworks.

## Features

- 🎨 **Automatic shade generation** - Creates 11 shades (50-900) for any base color
- 🎯 **Comprehensive coverage** - Background, text, border, SVG, UI, and shadow utilities
- 🌐 **CDN Ready** - Pre-built CSS files available for direct use

## Installation

### CDN (Easiest)
Include the CSS directly in your HTML:

```html
<!-- Latest version -->
<link rel="stylesheet" href="https://unpkg.com/@ahmed-aliraqi/color-palette@latest/dist/color-palette.min.css">

<!-- Or specific version -->
<link rel="stylesheet" href="https://unpkg.com/@ahmed-aliraqi/color-palette@1.0.3/dist/color-palette.min.css">

<!-- Via jsDelivr -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@ahmed-aliraqi/color-palette@latest/dist/color-palette.min.css">
```

### NPM
```bash
npm install @ahmed-aliraqi/color-palette
```

### Yarn
```bash
yarn add @ahmed-aliraqi/color-palette
```

### Manual
Download and include the `dist/color-palette.css` or `scss/index.scss` file in your project.

## Quick Start

### Using Pre-built CSS (No Build Process Required)
```html
<!DOCTYPE html>
<html>
<head>
    <link rel="stylesheet" href="https://unpkg.com/@ahmed-aliraqi/color-palette@latest/dist/color-palette.min.css">
</head>
<body>
    <div class="bg-blue-500 text-white">Blue background with white text</div>
    <p class="text-red-700 border-red-300">Red text with red border</p>
</body>
</html>
```

### Using SCSS Source
```scss
// Import the plugin
@use '@ahmed-aliraqi/color-palette';

// The plugin automatically generates utilities for the default color palette
// You can now use classes like:
// .bg-red-500, .text-blue-300, .border-green-700, etc.
```

## Available Classes

With the pre-built CSS, you get **over 3,000 utility classes** for 11 colors across 11 shade levels:

### Colors Available
- `red`, `green`, `blue`, `yellow`, `purple`, `pink`, `indigo`, `orange`, `teal`, `cyan`, `gray`

### Shade Levels
- `50` (lightest), `100`, `200`, `300`, `400`, `500` (base), `600`, `700`, `800`, `900`, `1000` (darkest)

### Property Types
- **Backgrounds**: `.bg-red-500`
- **Text**: `.text-blue-300`
- **Borders**: `.border-green-700`
- **Outlines**: `.outline-purple-400`
- **SVG Fill**: `.fill-orange-600`
- **SVG Stroke**: `.stroke-teal-500`
- **Text Decoration**: `.text-decoration-pink-300`
- **Caret**: `.caret-indigo-500`
- **Emphasis**: `.emphasis-cyan-400`
- **Accent**: `.accent-yellow-600`
- **Column Rule**: `.column-rule-gray-500`

## Default Color Palette

The plugin includes these colors by default:

- `red`: #ef4444
- `green`: #22c55e
- `blue`: #3b82f6
- `yellow`: #f59e0b
- `purple`: #8b5cf6
- `pink`: #ec4899
- `indigo`: #6366f1
- `orange`: #f97316
- `teal`: #14b8a6
- `cyan`: #06b6d4
- `gray`: #6b7280

## Default Shade Scale

| Shade | Lightness | Description |
|-------|-----------|-------------|
| 50 | +90% | Lightest |
| 100 | +80% | Very light |
| 200 | +70% | Light |
| 300 | +60% | Light medium |
| 400 | +50% | Medium light |
| 500 | 0% | Base color |
| 600 | -10% | Medium dark |
| 700 | -20% | Dark |
| 800 | -30% | Very dark |
| 900 | -40% | Darkest |
| 1000 | -50% | Ultra dark |

## Generated Class Examples

For a color named `blue`, the plugin generates:

### Background Classes
```css
.bg-blue-50 { background-color: #eff6ff !important; }
.bg-blue-500 { background-color: #3b82f6 !important; }
.bg-blue-900 { background-color: #1e3a8a !important; }
```

### Text Classes
```css
.text-blue-50 { color: #eff6ff !important; }
.text-blue-500 { color: #3b82f6 !important; }
.text-blue-900 { color: #1e3a8a !important; }
```

### Border Classes
```css
.border-blue-500 { border-color: #3b82f6 !important; }
.outline-blue-500 { outline-color: #3b82f6 !important; }
```

### SVG Classes
```css
.fill-blue-500 { fill: #3b82f6 !important; }
.stroke-blue-500 { stroke: #3b82f6 !important; }
```

## Browser Support

This plugin works with any modern SCSS compiler and the generated CSS works in all modern browsers. Some advanced properties like `accent-color` may have limited browser support.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

MIT License - see LICENSE file for details.
