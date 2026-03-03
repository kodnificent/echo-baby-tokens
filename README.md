# Echo Baby Design Tokens

Shared design tokens for Echo Baby products. Material Design 3 colors, typography, spacing, elevation, shape, and motion — all as CSS custom properties.

## Usage

### Install

```bash
bun add github:kodnificent/echo-baby-tokens
```

### Plain HTML/CSS

```html
<!-- Tokens (typography, spacing, elevation, shape, motion) -->
<link rel="stylesheet" href="node_modules/echo-baby-tokens/css/tokens.css">

<!-- Theme (pick one, or include both for dark mode support) -->
<link rel="stylesheet" href="node_modules/echo-baby-tokens/css/themes/light.css">
<link rel="stylesheet" href="node_modules/echo-baby-tokens/css/themes/dark.css">

<!-- Typography utility classes (optional) -->
<link rel="stylesheet" href="node_modules/echo-baby-tokens/css/typography.css">

<!-- Font -->
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap">
```

Then use CSS custom properties in your styles:

```css
body {
  font-family: var(--font-sans);
  background: var(--md-sys-color-background);
  color: var(--md-sys-color-on-background);
}

.card {
  background: var(--md-sys-color-surface-container);
  border-radius: var(--radius-xl);
  box-shadow: var(--elevation-2);
  padding: var(--spacing-6);
}
```

### Dark mode

Add `class="dark"` to `<html>` to switch to dark theme:

```html
<html class="dark">
```

### Bundler / CSS import

```css
@import 'echo-baby-tokens/css/tokens.css';
@import 'echo-baby-tokens/css/themes/light.css';
@import 'echo-baby-tokens/css/themes/dark.css';
@import 'echo-baby-tokens/css/typography.css';
```

## What's Included

| File | Contents |
|------|----------|
| `css/tokens.css` | Typography scale, spacing (4px grid), elevation (shadows), shape (border radius), motion (durations & easings) |
| `css/themes/light.css` | Default light theme — MD3 semantic colors, activity colors, event colors, tracker colors |
| `css/themes/dark.css` | Dark theme variant |
| `css/themes/light-mc.css` | Light medium contrast |
| `css/themes/light-hc.css` | Light high contrast (WCAG AA) |
| `css/themes/dark-mc.css` | Dark medium contrast |
| `css/themes/dark-hc.css` | Dark high contrast (WCAG AAA) |
| `css/typography.css` | Plain CSS utility classes (`.text-display-lg`, `.text-body-md`, etc.) |
| `assets/logo.svg` | Echo Baby logo |

## Test Page

Open `index.html` in a browser to see all tokens rendered with a dark mode toggle.

## License

MIT
