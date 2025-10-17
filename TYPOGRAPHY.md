# Pitt County Typography System

## Overview

The Pitt County website uses **Myriad Pro** as the official brand font to ensure readability, consistency, and accessibility across all platforms—including websites, social media, print materials, and official communications.

## Font Implementation

### Primary Font

-   **Myriad Pro** - Official Pitt County brand font
-   Includes weights: Light (300), Regular (400), Semibold (600), Bold (700)

### Fallback Fonts

For accessibility and cross-platform compatibility, the following fallback fonts are used:

-   `-apple-system` (iOS/macOS)
-   `BlinkMacSystemFont` (macOS)
-   `'Segoe UI'` (Windows)
-   `'Roboto'` (Android)
-   `'Helvetica Neue'` (General)
-   `Arial` (Universal fallback)
-   `sans-serif` (Generic fallback)

## Typography Scale

### Headings

-   **H1**: 3rem - 4rem (responsive) - Bold weight
-   **H2**: 2.25rem - 3rem (responsive) - Bold weight
-   **H3**: 1.875rem - 2.25rem (responsive) - Semibold weight
-   **H4**: 1.5rem - 1.875rem (responsive) - Semibold weight
-   **H5**: 1.25rem - 1.5rem (responsive) - Semibold weight
-   **H6**: 1.125rem - 1.25rem (responsive) - Semibold weight

### Body Text

-   **Base**: 1rem - 1.125rem (responsive) - Regular weight
-   **Lead**: 1.125rem - 1.25rem (responsive) - Regular weight
-   **Small**: 0.875rem - 1rem (responsive) - Regular weight
-   **Caption**: 0.75rem - 0.875rem (responsive) - Regular weight

## CSS Classes Available

### Font Weights

-   `.font-light` - 300 weight
-   `.font-regular` - 400 weight
-   `.font-semibold` - 600 weight
-   `.font-bold` - 700 weight

### Font Sizes

-   `.text-xs` - Extra small text
-   `.text-sm` - Small text
-   `.text-base` - Base text size
-   `.text-lg` - Large text
-   `.text-xl` - Extra large text
-   `.text-2xl` through `.text-5xl` - Larger heading sizes

### Line Heights

-   `.leading-tight` - 1.25 line height
-   `.leading-normal` - 1.5 line height
-   `.leading-relaxed` - 1.625 line height
-   `.leading-loose` - 2.0 line height

### Special Purpose Classes

-   `.nav-text` - For navigation elements
-   `.btn-text` - For button text (uppercase, letter-spaced)
-   `.lead` - For lead paragraphs
-   `.caption` - For captions and small text

## Usage Examples

### HTML Structure

```html
<h1>Page Title</h1>
<p class="lead">This is a lead paragraph with larger text.</p>
<p>This is regular body text using Myriad Pro.</p>

<nav>
    <a href="#" class="nav-text">Navigation Link</a>
</nav>

<button class="btn-text">Button Text</button>
```

### Custom Font Weights

```html
<h2 class="font-light">Light Heading</h2>
<p class="font-semibold">Semibold Paragraph</p>
```

## Accessibility Features

1. **Font Display**: Uses `font-display: swap` for better loading performance
2. **Responsive Sizing**: All text scales appropriately across devices
3. **Fallback Support**: Comprehensive fallback font stack
4. **Motion Preferences**: Respects `prefers-reduced-motion` settings
5. **Print Optimization**: Specific styles for print media

## File Structure

-   `css/typography.css` - Main typography system
-   `css/global.css` - Updated to integrate with typography
-   `index.html` - Updated with typography classes

## Browser Support

The typography system supports all modern browsers and gracefully degrades for older browsers through the fallback font system.

## Maintenance

When updating typography:

1. Maintain the Myriad Pro font as primary
2. Ensure all responsive scaling continues to work
3. Test across different devices and browsers
4. Verify accessibility compliance
5. Update this documentation as needed
