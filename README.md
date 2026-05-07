# TechGadget Price Matrix 

A CSS fundamentals project that styles a product comparison page using **combinators**, **structural selectors**, and **CSS units** — without adding extra classes to the HTML.

---

##  Project Structure

```
techgadget-price-matrix/

* index.html       # Main HTML file (starter code provided)
* style.css        # All CSS styling (the assignment deliverable)
* README.md        # This file
```

---

## Objective

Style a product grid where visual design changes are driven entirely by CSS selectors and combinators — relying on the **relationship between elements** rather than adding a class to every single element.

---

##  Requirements Covered

### 1. Layout — CSS Units

| Unit | Where Used | Why |
|------|-----------|-----|
| `rem` | `max-width` on `.container` | Relative to root font size — scales with browser accessibility settings |
| `vh` | `height` on the hero section | Proportional to viewport height on any screen size |
| `%` | `width` on article columns | Relative to parent — makes columns responsive |
| `em` | Padding & margins inside components | Scales relative to the element's own font size |

---

### 2. Selective Styling — Selectors & Combinators

| Rule | Selector | Effect |
|------|----------|--------|
| Premium Tag | `article:first-of-type` | Gold border on the first article only — no extra class needed |
| Nested Links | `footer a` | Styles all links inside `<footer>` (descendant combinator — **space**) |
| Direct Price Label | `.price-tag > span` | Targets only the `<span>` that is a direct child of `.price-tag` (child combinator — `>`) |
| Discount Notice | `h2 + p` | Styles a `<p>` that comes immediately after an `<h2>` (adjacent sibling combinator — `+`) |
| Hover State | `button:hover` | Changes button background on mouse hover |

---

### 3. Structural Targeting

| Rule | Selector | Effect |
|------|----------|--------|
| Even row highlight | `.features li:nth-child(even)` | Alternating background on every 2nd, 4th, 6th `<li>` — zebra stripe effect |
| Global box sizing | `* { box-sizing: border-box }` | Universal selector — applies to every element on the page |

---

##  Key Concepts Demonstrated

- **Combinator types:** descendant (space), child (`>`), adjacent sibling (`+`)
- **Pseudo-classes:** `:first-of-type`, `:nth-child(even)`, `:hover`
- **Universal selector** (`*`) for document-wide rules
- **Unit strategy:** `rem` for layout, `vh` for viewport, `%` for columns, `em` for component spacing
- **Avoiding class bloat:** structural selectors replace manual class assignments on HTML elements

---

##  How to Run

No build tools or dependencies required.

1. Clone or download the project folder
2. Open `index.html` in any browser
3. That's it — pure HTML and CSS, no frameworks

---

##  About

**Course:** Software Engineering — Zindua School  
**Cohort:** April 2026  
**Assignment:** CSS Selection Challenge (The TechGadget Price Matrix)  
**Topics:** CSS Units · Combinators · Pseudo-classes · Structural Selectors