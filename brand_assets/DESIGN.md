# Design System Specification: Contract Intelligence Refined

## 1. Overview & Creative North Star: "The Digital Polymath"

The digital landscape for finance and procurement is often cluttered with rigid grids and aggressive borders that mirror the spreadsheets they seek to replace. This design system breaks that cycle. Our Creative North Star is **"The Digital Polymath"**—an interface that feels as intelligent as the AI powering it, characterized by editorial precision, breathless whitespace, and organic depth.

We move beyond "software" into "experience" by employing **Intentional Asymmetry**. By offsetting high-contrast typography against expansive `surface` areas, we guide the eye through complex contract data with the ease of a premium broadsheet. We reject the "boxed-in" look of legacy ERPs, opting instead for a layered, translucent aesthetic that suggests a platform that is lightweight yet authoritative.

---

## 2. Color & Tonal Architecture

This system utilizes a sophisticated Material 3-based palette, anchored by deep indigos and crisp neutrals to establish a sense of institutional trust.

### The "No-Line" Rule
**Explicit Instruction:** 1px solid borders are prohibited for sectioning. Structural boundaries must be defined solely through background color shifts. Use `surface-container-low` for secondary navigation areas against a `surface` background. The eye should perceive change through tonal transitions, not "fences."

### Surface Hierarchy & Nesting
Treat the UI as a physical stack of semi-translucent sheets. 
- **Layer 0 (Base):** `surface` (#f9f9fb)
- **Layer 1 (Sectioning):** `surface-container-low` (#f3f3f5)
- **Layer 2 (Interactive Elements):** `surface-container-highest` (#e2e2e4)
- **Layer 3 (Floating Actions):** `surface-container-lowest` (#ffffff)

### The Glass & Gradient Rule
To signal "AI-First" sophistication, use **Glassmorphism** for floating panels (e.g., AI chat drawers or context menus). Combine `surface-container-lowest` at 80% opacity with a `backdrop-filter: blur(12px)`. 

**Signature Texture:** Primary actions should never be flat. Use a linear gradient (45°) transitioning from `primary` (#6e00c1) to `primary_container` (#8a2be2) to provide a tactile, "lit-from-within" quality to high-value buttons.

---

## 3. Typography: Editorial Authority

We use a duo-font approach to balance technical precision with human-centric readability.

*   **Display & Headlines (Manrope):** Chosen for its geometric stability and modern "tech-forward" feel. Use `display-lg` (3.5rem) with tighter letter-spacing (-0.02em) to create a bold, editorial statement in hero sections.
*   **Title & Body (Inter/Geist):** These are the workhorses. `title-md` (1.125rem) serves as the standard for card headers, while `body-md` (0.875rem) ensures high information density remains legible for long-form contract text.
*   **Labels (Inter):** All-caps `label-sm` (0.6875rem) with increased letter-spacing (0.05em) should be used for metadata and tags, providing a "blueprint" aesthetic that feels engineered.

---

## 4. Elevation & Depth: Tonal Layering

Traditional shadows are too heavy for a lightweight procurement tool. We convey hierarchy through ambient light and material stacking.

*   **The Layering Principle:** Instead of shadows, stack `surface-container-lowest` cards on top of a `surface-container-low` background. The subtle 2% difference in luminosity creates a sophisticated, "flat-depth" look.
*   **Ambient Shadows:** For high-elevation elements (Modals, Tooltips), use an ultra-diffused shadow: `box-shadow: 0 16px 32px rgba(110, 0, 193, 0.06)`. Note the tint: we use a fraction of the `primary` color, not black, to simulate natural light refraction.
*   **The Ghost Border:** If accessibility requires a stroke, use `outline-variant` (#cfc2d7) at **20% opacity**. It should be felt, not seen.

---

## 5. Component Philosophy

### Buttons & Chips
*   **Primary:** Gradient fill (`primary` to `primary_container`) with `on_primary` text. `round-md` (0.375rem) corner radius.
*   **Secondary:** `surface-container-highest` background. No border.
*   **Chips:** Use `secondary_container` (#e4e2e1) with `label-md` text. For AI-generated tags, use a subtle `tertiary_fixed` (#ffd8e6) background to highlight "intelligence."

### Input Fields & Controls
*   **Inputs:** Background set to `surface-container-low`. On focus, transition background to `surface-container-lowest` and add a 1px "Ghost Border" using `primary`.
*   **Checkboxes/Radios:** Use `primary` (#6e00c1) for selected states. The high contrast against the `f9f9fb` surface ensures rapid scanning.

### Cards & Intelligence Lists
*   **Strict Prohibition:** No divider lines between list items. Use `spacing-4` (1rem) of vertical white space or alternating tonal shifts (`surface` to `surface-container-low`).
*   **The "Insight" Card:** Cards containing AI contract insights should use a `tertiary` (#93075d) left-accent bar (4px) to draw the eye without boxing the content.

### Signature Component: The "Contextual Glass" Drawer
For contract deep-dives, use a right-aligned drawer with `surface-container-lowest` and 70% opacity. This allows the user to maintain visual context of the main document while reviewing AI-extracted clauses.

---

## 6. Do’s and Don’ts

### Do
*   **Do** use asymmetrical layouts. A heavy left-aligned headline with a wide right margin creates a premium, airy feel.
*   **Do** lean on `spacing-12` and `spacing-16` for section breathing room. 
*   **Do** use the `tertiary` (pink/magenta) palette sparingly—only for AI highlights or critical errors.

### Don't
*   **Don't** use pure black (#000000) for text. Always use `on_surface` (#1a1c1d) to maintain a soft, high-end feel.
*   **Don't** use "Card-in-Card" layouts with borders. Use nested tonal shifts (Darker surface inside Lighter surface).
*   **Don't** use standard 1px grey dividers. If a separator is required, use a `spacing-px` height box filled with `outline-variant` at 10% opacity.

---

## 7. Spacing & Rhythm

All spacing must adhere to the 4px baseline grid.
- **Section Padding:** `spacing-12` (3rem) to `spacing-20` (5rem).
- **Component Internal Padding:** `spacing-4` (1rem).
- **Icon-to-Text Gap:** `spacing-2` (0.5rem).

By adhering to this system, Nissa will transcend the utilitarian nature of procurement software, offering a workspace that feels like a high-performance, intelligent extension of the professional user.