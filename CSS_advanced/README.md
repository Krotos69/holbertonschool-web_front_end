

---

# Advanced CSS

A complete reference-style README summarizing core CSS concepts, matching the structure of your after-project documentation style.

---

## 🌐 Overview
CSS (Cascading Style Sheets) is the language that controls the **visual presentation** of HTML documents. It defines how elements look — layout, colors, spacing, animations, responsiveness, and more.

This README covers the **fundamental building blocks** of CSS, including selectors, the box model, layout systems, animations, transforms, browser support, and best practices. Each section includes conceptual explanations and practical examples.

---

## 1. Selectors, Properties, and Values
CSS rules follow the MDN structure:

```
selector {
  property: value;
}
```

From MDN:  
> “style-rule ::= selectors-list { properties-list }”  
> “selectors-list ::= selector[:pseudo-class] [::pseudo-element]”

### Selectors
- **Type selectors** (`p`, `div`)
- **Class selectors** (`.btn`)
- **ID selectors** (`#main`)
- **Attribute selectors** (`[type="text"]`)
- **Pseudo-classes** (`:hover`, `:focus`)
- **Pseudo-elements** (`::before`, `::after`)

### Properties & Values
Properties define *what* you change; values define *how*.

```
p { color: red; }
```

---

## 2. Block vs Inline Elements
Block elements:
- **Full width elements**  
- Start on a new line  
- Accept width/height  

Inline elements:
- **Inline flow elements**  
- Only take needed width  
- Ignore width/height  

---

## 3. CSS Reset (Consistency Across Browsers)
A reset removes default browser styles.

Common resets:
```
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
```

- **Normalize.css** is widely used.

---

## 4. CSS Variables (Custom Properties)
```
:root {
  --main-color: #3498db;
}

button {
  background: var(--main-color);
}
```

- **CSS variables** improve maintainability.

---

## 5. Inline vs Embedded vs External CSS
### Inline
```
<p style="color:red;">Hello</p>
```

### Embedded
```
<style>
  p { color: red; }
</style>
```

### External
```
<link rel="stylesheet" href="style.css">
```

- **External CSS** is preferred for scalability.

---

## 6. Grid Systems with Floats
Before Flexbox/Grid:

```
.column {
  float: left;
  width: 33.33%;
}
```

- **Float-based grids** require clearfix.

---

## 7. Icon Webfonts vs SVG Icons
### Webfonts
- Styled with `font-size`, `color`
- Can blur when scaled

### SVG Icons
- Crisp at any size
- Support `fill` and `stroke`

- **SVG icons** are preferred today.

---

## 8. Pseudo-classes vs Pseudo-elements
From MDN:  
> “Pseudo-classes specify a special state of the selected element.”  
> “Pseudo-elements represent entities not included in HTML.”

Examples:
- `a:hover` → pseudo-class  
- `p::first-line` → pseudo-element  

- **Specificity rules** apply differently.

---

## 9. Background Gradients
```
background: linear-gradient(45deg, red, blue);
```

Types:
- **Linear gradients**
- **Radial gradients**
- **Conic gradients**

---

## 10. CSS Animations
```
@keyframes fade {
  from { opacity: 0; }
  to { opacity: 1; }
}

div {
  animation: fade 2s ease-in-out;
}
```

Properties:
- `animation-name`
- `animation-duration`
- `animation-timing-function`
- `animation-iteration-count`

- **CSS animations** enable dynamic UI.

---

## 11. CSS Transforms (2D & 3D)
2D:
- `translate(x, y)`
- `rotate(45deg)`
- `scale(1.5)`

3D:
- `rotateX(45deg)`
- `rotateY(45deg)`
- `translateZ(50px)`

- **CSS transforms** enhance interactivity.

---

## 12. Vendor Prefixes
Used for experimental features:

```
.box {
  -webkit-transform: rotate(45deg);
  transform: rotate(45deg);
}
```

- **Vendor prefixes** ensure compatibility.

---

## 13. Box Sizing
From CSS-Tricks:  
> “width + padding + border = actual visible width”

Use:
```
* { box-sizing: border-box; }
```

- **Box sizing** simplifies layout math.

---

## 14. Specificity
From MDN:  
> “Specificity is the weight browsers use to determine which declaration applies.”

Order:
1. Inline styles  
2. IDs  
3. Classes, attributes, pseudo-classes  
4. Type selectors  
5. Universal selector  

Avoid `!important`.

- **Specificity calculator** helps visualize conflicts.

---

## 15. Browser Support (Can I Use)
Use caniuse.com to check support for:
- Flexbox  
- Grid  
- View transitions  
- New CSS functions (`if()`, `dvh`, etc.)

Example from the document:  
> “Lazy loading via attribute for video & audio – March 5, 2026”

- **Browser support** is essential for production.

---

## Final Notes
This README consolidates the core CSS concepts from MDN, CSS Reference, HTML Dog, CSS-Tricks, and Can I Use.

Use it as a quick study guide or project reference

---

## Author 
- **Eugenio Martinez**  
