# Design System Strategy: EAZ Việt Nam Recruitment Portal

## 1. Overview & Creative North Star: "The Kinetic Pulse"
This design system moves away from the static, corporate "template" look of traditional recruitment sites. For EAZ Việt Nam, we are adopting a Creative North Star called **"The Kinetic Pulse."** 

E-commerce is about movement, speed, and energy. Our design reflects this by using the vibrant Orange palette not just as a color, but as a source of light and heat. We break the rigid grid through **intentional asymmetry**: overlapping job cards, "floating" photography of smiling team members that break container bounds, and high-contrast typography scales that feel like a premium digital editorial. The goal is to make a candidate feel like they aren't just applying for a job, but joining a high-velocity movement.

---

## 2. Colors: Tonal Depth & The "No-Line" Rule
We use color to define structure. 

*   **The "No-Line" Rule:** 1px solid borders are strictly prohibited for sectioning. To separate the "Life at EAZ" section from the "Open Positions" section, transition the background from `surface` (#fff4ef) to `surface-container-low` (#ffede4).
*   **Surface Hierarchy:** 
    *   **Level 0 (Base):** `surface` (#fff4ef) - Use for the main page canvas.
    *   **Level 1 (Nesting):** `surface-container` (#ffe3d2) - Use for secondary content areas.
    *   **Level 2 (Interaction):** `surface-container-highest` (#ffd4b9) - Use for hover states or active card backgrounds.
*   **Signature Textures:** For Hero sections and primary CTAs, do not use flat orange. Apply a subtle gradient from `primary` (#9c3f00) to `primary-container` (#ff7a2f) at a 135-degree angle to add "soul" and dimension.
*   **Glassmorphism:** For floating navigation bars or "Quick Apply" widgets, use `surface` with 70% opacity and a `24px` backdrop-blur to allow the vibrant brand colors to bleed through.

---

## 3. Typography: The Editorial Edge
We pair two distinct sans-serifs to balance high-energy headlines with extreme readability.

*   **Display & Headlines (Plus Jakarta Sans):** This is our "vocal" font. Use `display-lg` (3.5rem) for hero statements. Tighten letter-spacing by `-0.02em` to create a compact, high-end "editorial" look.
*   **Body & Labels (Be Vietnam Pro):** Our "functional" font. Designed for the Vietnamese language, it ensures that job descriptions are legible even on small mobile screens.
*   **Hierarchy Tip:** Use `headline-sm` in `primary` (#9c3f00) for section titles to draw the eye, while keeping body text in `on-surface-variant` (#7f512e) for a softer, premium reading experience.

---

## 4. Elevation & Depth: Tonal Layering
Forget drop shadows that look like "fuzz" behind a box. We use light and layering.

*   **The Layering Principle:** Place a `surface-container-lowest` (#ffffff) card on a `surface-container` (#ffe3d2) background. The change in hex value creates a "soft lift" that feels architectural rather than digital.
*   **Ambient Shadows:** If an element must float (like a sticky CTA), use a shadow with a blur of `32px` and an opacity of `6%`, tinted with `on-surface` (#4a2506). This mimics natural sunlight hitting a surface.
*   **The "Ghost Border":** If a boundary is needed for accessibility in input fields, use the `outline-variant` (#dba078) at **15% opacity**. It should be felt, not seen.

---

## 5. Components: Precision & Purpose

### Buttons (The Energy Drivers)
*   **Primary CTA:** Gradient from `primary` to `primary-container`. `xl` roundedness (1.5rem). Text in `on-primary` (#fff0ea). 
*   **Secondary CTA:** `surface-container-highest` background with `primary` text. No border.
*   **States:** On hover, the primary button should scale slightly (1.02x) rather than just changing color, emphasizing the \"Kinetic Pulse.\"

### Job Cards (The Talent Showcase)
*   **Structure:** No dividers. Use `spacing-6` (1.5rem) as the internal padding.
*   **Content:** Job title in `title-lg`, Department in `label-md` (Uppercase, tracked out 5%).
*   **Visual Shift:** Use a `surface-container-low` background. On hover, shift to `surface-container-highest` and apply a `ghost border`.

### Image Containers (The Human Element)
*   **Asymmetric Framing:** Do not use simple rectangles. Use a mix of `xl` (1.5rem) and `full` (pill) corner radii on different corners of the same image to create a custom, modern tech vibe.
*   **Overlays:** Use a `20%` tint of `primary` on decorative background elements to tie professional photography back to the EAZ brand.

### Input Fields
*   **Style:** Flat. Background `surface-container-lowest`. 
*   **Active State:** A 2px bottom-bar using `primary` (#9c3f00) instead of a full bounding box.

---

## 6. Do's and Don'ts

### Do:
*   **Do** use plenty of white space. Refer to `spacing-20` (5rem) for section breathing room.
*   **Do** mix photography with abstract orange \"pulse\" shapes to create depth.
*   **Do** use `tertiary` (#00675b) for success states or \"New\" badges to provide a sophisticated contrast to the orange.

### Don't:
*   **Don't** use black (#000000) for text. Always use `on-surface` (#4a2506) to maintain a warm, high-end feel.
*   **Don't** use standard 4px rounded corners. Stick to the `md` (0.75rem) or `xl` (1.5rem) tokens to keep the \"Modern & Youthful\" promise.
*   **Don't** clutter the Job Cards. If information isn't vital for the first click, hide it. Minimalism is a sign of a premium brand.

---
*End of Design System Document*