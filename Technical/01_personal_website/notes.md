

### [Next steps]()

- Upload your past projects

### 🔧 Fundamental Objects (HTML Semantic Primitives)

These are not just tags—they're **semantic roles** you must map to user intent and content hierarchy:

#### 1. **`<header>`**

* Purpose: Contains the site's branding, nav bar, or intro tagline.
* Strategy: Optimize for fast scan, identity recognition, and primary nav routes.

#### 2. **`<nav>`**

* Purpose: Navigation links to sections or other pages.
* Strategy: Should not be an unordered list unless there's real hierarchical structure. Inline links are often more semantically efficient.

#### 3. **`<main>`**

* Purpose: Core content of your portfolio (e.g. About, Projects, Skills).
* Strategy: This is your conversion zone. Make it information-dense and value-concentrated.

#### 4. **`<section>`**

* Purpose: Logical grouping within `<main>` (e.g., a “Projects” section).
* Strategy: Each section should be self-contained, address a specific user intent, and serve a conversion path (e.g., recruiter, client, collaborator).

#### 5. **`<article>`**

* Purpose: Individual project showcases or blog entries.
* Strategy: Treat as atomic units—project cards or writeups that can be reused or filtered.

#### 6. **`<footer>`**

* Purpose: Contact info, social links, copyright.
* Strategy: Think of it as your last-ditch call to action. Avoid decorative clutter.

---

### 🎨 Fundamental Objects (CSS Layout + Style Constructs)

Avoid ad hoc styling. Think in terms of **layout primitives** that give you composable control over space and hierarchy:

#### 1. **CSS Grid / Flexbox Containers**

* Use `display: grid` or `display: flex` to create layout scaffolds.
* Grid for macro layout (whole page or sections); Flex for micro layout (navbars, cards).

#### 2. **Box Model Units**

* Use rem/em for scalable spacing.
* Avoid fixed px unless for borders or pixel-perfect visual constraints.

#### 3. **Utility Classes (Optional)**

* You can build minimal utility classes for spacing, alignment, and font sizing to enforce consistency without a full framework.

#### 4. **Custom Properties (`--var`)**

* Centralize color, spacing, and font systems.
* Avoid hard-coded values unless optimizing for performance.

#### 5. **Responsive Breakpoints**

* Use `@media` queries to target:
  * mobile-first (≤768px)
  * tablets (~1024px)
  * desktops (≥1280px)

---

### 🧱 Minimal Object Set Summary

| **Object** | **Purpose**         | **CSS Strategy**        |
| ---------------- | ------------------------- | ----------------------------- |
| `<header>`     | Identity + primary nav    | Flexbox/Sticky positioning    |
| `<nav>`        | Section/page routing      | Inline-flex + hover styles    |
| `<main>`       | Core content zones        | Grid/flex layout              |
| `<section>`    | Thematic content grouping | Padding + border delineation  |
| `<article>`    | Project or post instances | Card-like UI using box shadow |
| `<footer>`     | Contact/action closure    | Contrasting background        |
