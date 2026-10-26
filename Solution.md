## Assignment 5.2 — CSS Selectors Practice

### 1. `index.html`

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>CSS Selectors</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>CSS Selectors Practice</h1>
    <p>This is a paragraph.</p>

    <div class="card">HTML</div>
    <div class="card">CSS</div>

    <section id="special">
        <h2>JavaScript</h2>
        <p>Learn web development.</p>
    </section>
</body>
</html>
```

### 2. `style.css`

```css
* {
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f0f4f8;
}

h1 {
    color: blue;
}

p {
    color: green;
}

.card {
    background-color: lightblue;
    padding: 15px;
    margin: 10px;
}

#special {
    background-color: lightyellow;
    padding: 15px;
}

h1, h2 {
    text-align: center;
}

/* Specificity and cascade */
p {
    color: red;
}

body p {
    color: purple;
}
```

### 3. Explanation

- **Universal selector (`*`):** Applies `box-sizing` to all elements.
- **Element selector (`h1`, `p`):** Styles HTML elements.
- **Class selector (`.card`):** Styles multiple cards.
- **ID selector (`#special`):** Styles a specific section.
- **Grouping selector (`h1, h2`):** Applies the same style to both headings.
- **Cascade and specificity:** `body p` overrides `p` because it has higher specificity, so paragraphs appear purple.

**Submission:** Save `index.html` and `style.css` in the same folder and open the HTML file using Live Server.