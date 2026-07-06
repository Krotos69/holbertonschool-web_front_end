

---

# **Advanced HTML Foundations**

Modern HTML5 is more than a markup language — it is a semantic, accessible, and structured system for building meaningful web documents. The objective of this topic is to help you understand not only *how* to write HTML, but *why* each element exists, how it contributes to structure, accessibility, and maintainability, and how to apply best practices aligned with the HTML Standard (WHATWG) and MDN Web Docs. This guide provides detailed explanations, examples, and authoritative references to help you master advanced HTML.

---

## **1. Guidelines to Follow for HTML**

### **Key Principles**
- **Semantic Structure:** Use elements according to their meaning.  
- **Accessibility:** Provide proper headings, alt text, and logical structure.  
- **Content Models:** Follow allowed child elements for each tag.  
- **Separation of Concerns:** HTML = structure, CSS = style, JS = behavior.  
- **Validation:** Use conformance checkers to ensure correctness.  

### **Example**
```html
<header>
  <h1>My Portfolio</h1>
</header>
```

### **Resources**
- WHATWG HTML Standard  
- MDN Web Docs — HTML  
- HTML Reference  
- WebsiteSetup HTML Cheat Sheet  

---

## **2. How to Create the Skeleton of an HTML5 Page**

### **Example**
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document Title</title>
</head>
<body>
  <h1>Hello World</h1>
</body>
</html>
```

### **Resources**
- MDN — HTML basics  
- WebsiteSetup — HTML5 skeleton  

---

## **3. How to Use Semantic HTML Tags to Structure a Web Page**

Semantic tags give meaning to content and improve accessibility.

### **Example**
```html
<main>
  <article>
    <h2>Blog Post</h2>
    <p>Content goes here.</p>
  </article>
</main>
```

### **Resources**
- MDN — Semantic HTML  
- WHATWG — Sectioning content  

---

## **4. Use Cases for `<div>` vs `<span>`**

### **`<div>`**
- Block-level  
- Used for layout or grouping when no semantic element fits  

### **`<span>`**
- Inline-level  
- Used for styling or grouping text within a line  

### **Example**
```html
<div class="container">
  <span class="highlight">Important text</span>
</div>
```

### **Resources**
- HTML Reference — div, span  

---

## **5. Semantic Value of `header`, `main`, `footer`, `article`, `nav`, `section`, `aside`**

### **header**
Introductory content for a page or section.

### **main**
Primary content of the page (only one allowed).

### **footer**
Closing or legal information.

### **article**
Self-contained content (blog post, comment, news item).

### **nav**
Major navigation links.

### **section**
Thematic grouping of content, usually with a heading.

### **aside**
Complementary or tangential content.

### **Example**
```html
<aside>
  <p>Related links</p>
</aside>
```

### **Resources**
- WHATWG — Sectioning elements  
- MDN — Semantic elements  

---

## **6. How to Use Headings and Why Hierarchy Matters**

Headings (`h1`–`h6`) define the document outline.

### **Rules**
- Follow hierarchical order  
- Do not skip levels for styling  
- Use one `<h1>` per page  

### **Example**
```html
<h1>Main Title</h1>
<h2>Subsection</h2>
<h3>Detail</h3>
```

### **Resources**
- WHATWG — Headings and outlines  
- MDN — Headings  

---

## **7. How to Make Lists in HTML**

HTML supports three list types.

### **Example**
```html
<ul>
  <li>Item</li>
</ul>

<ol>
  <li>Step 1</li>
</ol>

<dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language</dd>
</dl>
```

### **Resources**
- MDN — Lists  

---

## **8. Differences Between Media Formats (SVG, GIF, PNG, JPG)**

### **SVG**
- Vector  
- Infinite scalability  
- Best for icons, logos, diagrams  

### **GIF**
- Animation  
- Limited colors  
- Not ideal for photos  

### **PNG**
- Lossless  
- Supports transparency  
- Best for UI elements, screenshots  

### **JPG**
- Lossy  
- Best for photographs  
- Small file size  

### **Example**
```html
<img src="logo.svg" alt="Company Logo">
```

### **Resources**
- MDN — Image file types  

---

## **9. How to Structure Data in a Table**

### **Example**
```html
<table>
  <caption>Sales Report</caption>
  <thead>
    <tr>
      <th>Month</th>
      <th>Total</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>January</td>
      <td>$1000</td>
    </tr>
  </tbody>
</table>
```

### **Resources**
- WHATWG — Tabular data  
- MDN — Tables  

---

## **10. How to Integrate a Video in a Webpage**

### **Example**
```html
<video controls width="600">
  <source src="movie.mp4" type="video/mp4">
</video>
```

### **Resources**
- MDN — Video element  

---

## **11. How to Integrate an Audio File in a Webpage**

### **Example**
```html
<audio controls>
  <source src="sound.mp3" type="audio/mpeg">
</audio>
```

### **Resources**
- MDN — Audio element  

---

## **12. How to Embed External Content**

### **Example**
```html
<iframe src="https://example.com" width="600" height="400"></iframe>
```

### **Resources**
- MDN — Embedding content  

---

## **13. How to Correctly Structure an HTML Page**

### **Example**
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Example Page</title>
</head>
<body>
  <header>
    <h1>Site Title</h1>
  </header>

  <main>
    <article>
      <h2>Article Title</h2>
      <p>Content goes here.</p>
    </article>
  </main>

  <footer>
    <p>© 2026</p>
  </footer>
</body>
</html>
```

### **Resources**
- WHATWG — Document structure  
- MDN — HTML structure  

---

# **Author: Eugenio Martínez**

---

