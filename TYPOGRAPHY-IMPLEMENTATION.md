# Pitt County Typography Implementation Guide

## Quick Reference for Developers

### 1. Approved Font Stack (in order of preference):

```css
font-family: 'Myriad Pro', 'Noto Sans', 'Open Sans', -apple-system, BlinkMacSystemFont,
    'Segoe UI', 'Roboto', 'Helvetica Neue', Arial, sans-serif;
```

### 2. CSS Classes to Use Instead of Inline Styles:

#### Font Families:

-   `.font-primary` - Uses complete Pitt County font stack
-   `.canva-fallback` - For Canva-compatible designs
-   `.font-script` - Great Vibes (APPROVAL REQUIRED)

#### Font Weights:

-   `.font-light` (300)
-   `.font-regular` (400)
-   `.font-semibold` (600)
-   `.font-bold` (700)

#### Text Sizes:

-   `.text-xs` through `.text-5xl`
-   Use `.h1` through `.h6` for semantic headings

#### Typography Best Practices:

-   `.text-left` - Left alignment (preferred)
-   `.optimal-line-length` - 50-75 character limit
-   `.tracking-normal` - Consistent letter spacing
-   `.leading-normal` - Adequate line spacing
-   `.title-case` - For headlines
-   `.no-orphans` - Prevents text widows/orphans

### 3. Converting Inline CSS:

#### Instead of:

```html
<h1 style="font-family: Arial; font-size: 48px; font-weight: bold;"></h1>
```

#### Use:

```html
<h1 class="h1 font-bold title-case"></h1>
```

### 4. Responsive Typography:

All font sizes use `clamp()` for automatic scaling across devices.

### 5. Accessibility:

-   Respects user font size preferences
-   Includes proper fallbacks
-   Optimized for screen readers

### 6. Special Cases:

#### For Canva Designs:

Add class `canva-fallback` to use Noto Sans/Open Sans

#### For Script Elements (APPROVAL REQUIRED):

```html
<span class="font-script">Special Signature</span>
```

#### For Optimal Readability:

```html
<p class="optimal-line-length leading-relaxed">Long content here...</p>
```

## Migration Strategy:

1. **Replace inline font-family declarations** with CSS custom properties
2. **Use semantic HTML** (h1-h6) with typography classes
3. **Apply utility classes** instead of inline styles
4. **Test across devices** to ensure responsive behavior
5. **Validate accessibility** with screen readers

## Development Workflow:

1. **Always use external CSS** instead of inline styles
2. **Link typography.css** in every HTML file
3. **Use CSS custom properties** for consistency
4. **Follow mobile-first** responsive approach
5. **Test font loading** across different connection speeds
