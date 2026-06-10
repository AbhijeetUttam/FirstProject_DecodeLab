# FirstProject_DecodeLab
# DecodeLabs - Frontend Project 1 (Static Webpage Design)

This repository contains the source code for **Frontend Project 1** from the DecodeLabs Batch 2026 Industrial Training Kit. The project serves as a showcase and educational blueprint for masterclass frontend engineering, prioritizing semantic markup integrity, modern CSS layouts (CSS Grid & Flexbox), accessibility (A11Y), and responsive visual architecture.

---

## 🚀 Project Overview

The project is a premium, developer-focused static landing page designed using a "blueprint" and dark-mode aesthetic. It highlights the transition from visual structure plans to clean, scalable, and semantically perfect HTML & CSS.

### Key Objectives
*   **Semantic Integrity:** Strictly using correct HTML5 elements (`<header>`, `<main>`, `<section>`, `<article>`, `<address>`, `<footer>`) with a single `<h1>` tag to achieve a perfect sitemap structure.
*   **CSS Engineering (DRY):** Implementing modular, reusable CSS styles without inline declarations.
*   **Modern Layout Systems:** Utilizing CSS Grid for macro-layout (2D grids like cards and columns) and Flexbox for micro-layout (1D alignments like navigation and inline flows).
*   **Performance & Web Auditing:** Adhering to standards aligned with W3C validation and Lighthouse optimization parameters (WebP/AVIF media tags, proper dimensions, accessibility contrast ratios).

---

## 📁 File Structure

The project has a clean and minimalist structure:

```bash
d:/AbhijeetProject/
├── index.html   # Main structural sitemap and content markup
└── style.css    # Master stylesheet (External styles & Design tokens)
```

---

## 🛠️ Codebase Deep-Dive

### 1. Structure (`index.html`)

The markup is organized into distinct logical sections:
*   **Header / Nav:** Contains the brand logo (`DecodeLabs`) and utility anchor links mapped directly to on-page section IDs.
*   **Hero Section (`#hero`):** A high-impact opening fold featuring a background grid texture, typography headings, and an absolute-positioned badge (`P1 Static Webpage`) that scales down on smaller screens.
*   **About Section (`#about`):** Introduces the core project requirements paired with a simulated **CSS Blueprint Card** visual detailing structural sitemaps.
*   **Skills Section (`#skills`):** A responsive 3-column grid composed of semantic `<article>` cards covering core engineering principles (Information Architecture, Semantic HTML, CSS Engineering, Layout Systems, A11Y, and QA).
*   **IPO Model Section:** A structural flowchart representing the engineering workflow: **Input** (Assets) $\rightarrow$ **Process** (CSS Logic) $\rightarrow$ **Output** (Rendered View).
*   **Footer (`#contact`):** Includes brand information, copyright text, and an `<address>` block providing physical/digital contact details.

### 2. Styling (`style.css`)

The style system uses a custom design system based on CSS variables and responsive media breakpoints:

#### **Design Tokens (CSS Variables)**
```css
:root {
  --color-bg: #0a0a0f;           /* Deep dark background */
  --color-surface: #12121a;      /* Card / Section surface background */
  --color-surface-2: #1a1a28;    /* Footer / Inner element background */
  --color-primary: #ff6b35;      /* Vibrant orange accent */
  --color-accent: #4ecdc4;       /* Teal color accent */
  --color-text: #e8e8f0;         /* Primary text light tone */
  --color-text-muted: #8888aa;   /* Secondary/muted text tone */
  --color-border: #2a2a40;       /* Border / separator color */
  --color-blueprint: #1a3a6b;    /* Blueprint card background */
  --font-display: 'Syne', sans-serif;
  --font-mono: 'Space Mono', monospace;
  --radius: 6px;
  --radius-lg: 12px;
  --max-width: 1200px;
  --transition: 0.25s ease;
}
```

#### **Core Design & Interaction Highlights**
*   **Typography:** The page combines the modern, bold geometric typeface `Syne` for headings with `Space Mono` for technical labels, code snippets, and structured items.
*   **Grid Layouts:** 
    *   `.skills-grid` uses `grid-template-columns: repeat(3, 1fr)` for a multi-column desktop layout.
    *   `.about-grid` splits content evenly into two parts on desktop screens.
*   **Visual Polish:** Includes micro-animations (like hover shifts `translateY(-4px)` on cards, smooth transitions, and box-shadow glows) and a custom CSS-engineered grid background utilizing repeating gradients.

#### **Responsiveness (Media Queries)**
*   **`@media (max-width: 900px)` (Tablets):** Switches the layout to single column for the About and Footer sections, scales the Skills grid to 2 columns, and hides the decorative hero badge to preserve screen space.
*   **`@media (max-width: 600px)` (Mobiles):** Adapts the Skills Grid to a single column, rotates the IPO model arrows to point downwards, hides the navigation menu links to clean up visual clutter, and rescales the large hero typography.

---

## 🏷️ Standards and Guidelines

This codebase follows professional development standards:
1.  **CSS Variable Utilization:** All color, spacing, fonts, and animation properties refer back to design variables.
2.  **No Inline Styling:** Structural layout and styling layers are completely decoupled.
3.  **BEM Styling Method:** Selectors follow standard CSS architecture practices for maintainability.
4.  **A11Y Best Practices:** High text-to-background contrast and responsive viewport configurations are built-in.
