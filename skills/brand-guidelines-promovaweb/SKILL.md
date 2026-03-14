---
name: brand-guidelines-promovaweb
description: Applies PromovaWeb's official brand colors and typography to any sort of artifact that may benefit from having PromovaWeb's look-and-feel. Use it when brand colors or style guidelines, visual formatting, or company design standards apply. PromovaWeb is a Brazilian digital marketing and LowCode education platform.
license: Complete terms in LICENSE.txt
---

# PromovaWeb Brand Styling

## Overview

To access PromovaWeb's official brand identity and style resources, use this skill.

**Keywords**: branding, promovaweb, corporate identity, visual identity, post-processing, styling, brand colors, typography, PromovaWeb brand, visual formatting, visual design, teal, lowcode, marketing digital

## Brand Guidelines

### Colors

**Main Colors:**

- Dark Navy: `#1A3A5C` - Primary CTA buttons and strong contrasts
- Heading Dark: `#111827` - H1/H2 titles and primary text
- Body Gray: `#6B7280` - Paragraphs, descriptions, secondary text
- Light Background: `#F9FAFB` - Page and section backgrounds
- White: `#FFFFFF` - Card surfaces and hero backgrounds

**Accent Colors:**

- Brand Teal: `#00C9A7` - Primary brand accent, logo "web" highlight, display headlines
- Teal Dark: `#00957A` - Hover states, borders, secondary teal elements

**Supporting Colors:**

- Nav / Subtext: `#374151` - Navigation links, tertiary text
- Icon Background: `#EEF2FF` - Icon container fills and subtle highlights
- Borders: `#E5E7EB` - Dividers, card borders, separators

### Typography

- **Display (H1)**: Inter ExtraBold 800 (with Arial Black fallback)
- **Headings (H2/H3)**: Inter Bold 700 (with Arial Bold fallback)
- **Body Text**: Inter Regular 400 (with Arial fallback)
- **UI Labels / Nav**: Inter Medium 500 (with Arial fallback)
- **Note**: Inter should be pre-installed in your environment for best results. Google Fonts CDN available at https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700;800

### Logo Usage

- **"Promova"** portion: rendered in `#111827` (dark heading color)
- **"web"** portion: rendered in `#00C9A7` (brand teal)
- Minimum clear space: equal to the height of the "P" on all sides
- Never recolor or distort the logo mark

### Decorative Elements

- **Dot grid pattern**: subtle grid of small circles in `#D1D5DB` — used in hero backgrounds, top-left positioning
- **Border radius**: 8px for buttons and inputs, 12px for cards, 20px+ for large containers
- **Button style**: filled navy `#1A3A5C` for primary; ghost with `#1A3A5C` border and text for secondary

## Features

### Smart Font Application

- Applies Inter ExtraBold 800 to display headings (H1, 28pt and larger)
- Applies Inter Bold 700 to section headings (H2/H3, 16–24pt)
- Applies Inter Regular 400 to body text
- Applies Inter Medium 500 to nav items, labels, and UI elements
- Automatically falls back to Arial if Inter unavailable
- Preserves readability across all systems

### Text Styling

- Display headings (28pt+): Inter 800, color `#111827`, teal accent `#00C9A7` on key phrases
- Section headings (16–24pt): Inter 700, color `#111827`
- Body text: Inter 400, color `#6B7280`, line-height 1.6
- Navigation / UI: Inter 500, color `#374151`
- Smart color selection based on background brightness
- Preserves text hierarchy and formatting

### Shape and Accent Colors

- Primary CTA shapes and buttons use Navy `#1A3A5C`
- Accent highlights and underlines use Brand Teal `#00C9A7`
- Icon backgrounds use `#EEF2FF`
- Card surfaces use White `#FFFFFF` with `#E5E7EB` borders
- Section backgrounds alternate between `#FFFFFF` and `#F9FAFB`
- Maintains visual interest while staying on-brand

## Technical Details

### Font Management

- Uses system-installed Inter font when available
- Google Fonts CDN: `https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700;800&display=swap`
- Provides automatic fallback to Arial (all weights)
- No font installation required — works with existing system fonts
- For best results, pre-install Inter or load via Google Fonts CDN

### Color Application

- Uses RGB/HEX color values for precise brand matching
- Applied via python-pptx's RGBColor class for .pptx artifacts
- Applied via CSS custom properties for HTML/React artifacts:

```css
--pw-teal:       #00C9A7;
--pw-teal-dark:  #00957A;
--pw-navy:       #1A3A5C;
--pw-heading:    #111827;
--pw-nav:        #374151;
--pw-body:       #6B7280;
--pw-bg:         #F9FAFB;
--pw-icon-bg:    #EEF2FF;
--pw-border:     #E5E7EB;
--pw-white:      #FFFFFF;
```

- Maintains color fidelity across different systems and formats
