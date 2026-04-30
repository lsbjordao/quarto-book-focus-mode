# Quarto Book Focus Mode

A lightweight Quarto extension that adds a floating **Focus Mode** toggle button to Quarto Book HTML outputs.

The button hides the left sidebar and page table of contents, recenters the main content for distraction-free reading, and can be toggled back to restore navigation. The selected mode is remembered across pages during navigation.

Compatible with **Quarto ≥ 1.4**.

## Installation

From within a Quarto project:

```bash
quarto add lsbjordao/quarto-book-focus-mode
```

## Usage

After installation, the focus-mode toggle button is automatically enabled in **Quarto Book HTML output**.

No additional configuration is required.

Click the button to switch between:

- **Focus mode** → hides sidebar and margin TOC
- **TOC mode** → restores navigation panels

The selected mode is preserved while browsing the book.

## Custom content width

You can adjust the reading width in focus mode by defining:

```css
:root {
  --book-focus-content-width: 960px;
}
```

Add this rule to your project stylesheet.

## Features

- Floating toggle button
- Responsive pill-style hover animation
- Sidebar + margin TOC hide/show
- Reading-optimized layout width
- Local state persistence (per browser session)
- Automatically activates only for Quarto Book layout
- Zero configuration required

## Compatibility

This extension is designed specifically for **Quarto Book HTML output**.

The button automatically hides itself on pages that do not use the Quarto Book sidebar structure.