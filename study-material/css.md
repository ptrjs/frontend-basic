# CSS

CSS (Cascading Style Sheets) is a styling language used to control the appearance and layout of HTML elements on a web page. CSS allows you to separate content (HTML) from presentation (styling), making it easy to change the appearance of an entire website just by modifying the CSS file without having to touch the HTML structure.

With CSS, you can control many style properties, such as text color, text size, font type, spacing between elements, positioning, and more. CSS also supports selection by element type (tag), class, ID, attributes, and pseudo-classes like `:hover` to control how elements appear in different states.

Here are some common CSS properties:

- `color`: Sets the text color.
- `font-family`: Defines the font type.
- `font-size`: Sets the text size.
- `background-color`: Sets the background color of an element.
- `margin` and `padding`: Control spacing around elements.
- `border`: Creates borders around elements.
- `text-align`: Aligns text (left, center, or right).
- `width` and `height`: Set element dimensions.
- `position`: Sets the position of elements.

Example CSS code:

```css
/* Element selector */
p {
    color: blue;
    font-size: 16px;
}

/* Class selector */
.button {
    background-color: #ff6600;
    color: white;
    padding: 10px 20px;
}

/* ID selector */
#header {
    background-color: #333;
    color: white;
    text-align: center;
}
```

CSS is crucial in web development as it enables you to create visually appealing, responsive, and consistent designs for your website.

## CSS Selectors

CSS selectors are ways to select an element or group of elements in an HTML document to apply CSS rules. Here's a list of common selector types:

1. **Element Selector:**
   ```css
   p {
       color: blue;
   }
   ```

2. **Class Selector:**
   ```css
   .button {
       background-color: #ff6600;
       color: white;
   }
   ```

3. **ID Selector:**
   ```css
   #header {
       background-color: #333;
       color: white;
   }
   ```

4. **Attribute Selector:**
   ```css
   input[type="text"] {
       border: 1px solid #ccc;
   }
   ```

5. **Pseudo-Class Selector:**
   ```css
   a:hover {
       color: red;
   }
   ```

6. **Nested Selector:**
   ```css
   ul li {
       list-style-type: disc;
   }
   ```

7. **Combined Selector:**
   ```css
   h1, h2 {
       font-family: "Arial", sans-serif;
   }
   ```

8. **Conditional Selector:**
   ```css
   p:first-child {
       font-weight: bold;
   }
   ```

## Common CSS Properties

Here’s a list of frequently used CSS properties:

1. **Color:**
   - `color`, `background-color`

2. **Font:**
   - `font-family`, `font-size`, `font-weight`, `line-height`

3. **Border:**
   - `border`, `border-radius`

4. **Spacing:**
   - `padding`, `margin`

5. **Layout:**
   - `width`, `height`, `display`, `position`, `float`

6. **Text:**
   - `text-align`, `text-decoration`

7. **Lists:**
   - `list-style-type`

8. **Background:**
   - `background-image`, `background-size`, `background-position`

9. **Transform:**
   - `transform`

10. **Transition & Animation:**
    - `transition`, `animation`

11. **Box Model:**
    - `box-sizing`

12. **Flexbox & Grid:**
    - `flex`, `flex-direction`, `grid-template-columns`, etc.

13. **Pseudo-Classes & Elements:**
    - `:hover`, `::before`, etc.

14. **Media Queries:**
    - `@media`

15. **Filter:**
    - `filter`

16. **Variables:**
    - `--var-name`

## CSS Usage Example

Create a folder named `icecream` and add two files:

### `index.html`
```html
<!DOCTYPE html>
<html>
<head>
    <title>Zexo Ice Cream</title>
    <link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
    <header>
        <h1>Welcome to Zexo Ice Cream</h1>
        <p>Enjoy the Sweet Sensation</p>
    </header>

    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">Menu</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>

    <section id="menu">
        <h2>Ice Cream Menu</h2>
        <div class="ice-cream">
            <img src="https://img.freepik.com/free-photo/cornet-ice-cream-with-strawberry-scoop-colorful-surface_463209-35.jpg?w=900&t=st=1697370192~exp=1697370792~hmac=a915bb72a43604b81f5587132d45a077ae5caef0fae976d625e88478474d4653" alt="Ice Cream 1">
            <h3>Raspberry Sorbet</h3>
            <p>Experience the freshness of raspberry in our sorbet.</p>
            <span>Rp 25.000</span>
        </div>

        <div class="ice-cream">
            <img src="https://img.freepik.com/free-photo/high-angle-hand-holding-ice-cream-cup_23-2149681943.jpg?w=900&t=st=1697370298~exp=1697370898~hmac=54bf42e3e84cd5d10e073448e93659a7e83fa5214af0c8cb569badbca640e5c5" alt="Ice Cream 2">
            <h3>Chocolate Delight</h3>
            <p>Enjoy the richness of chocolate in this scoop.</p>
            <span>Rp 30.000</span>
        </div>
    </section>

    <footer>
        <p>&copy; 2023 Zexo Ice Cream</p>
    </footer>
</body>
</html>
```

### `style.css`
```css
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f5f5f5;
}

header {
    background-color: #ff6600;
    color: white;
    text-align: center;
    padding: 20px;
}

nav ul {
    background-color: #ff6600;
    list-style: none;
    padding: 0;
    text-align: center;
}

nav ul li {
    display: inline;
    margin: 0 10px;
}

nav ul li a {
    text-decoration: none;
    color: white;
}

section {
    margin: 20px;
}

h2 {
    text-align: center;
}

.ice-cream {
    background-color: #fff;
    border: 1px solid #ddd;
    border-radius: 5px;
    padding: 20px;
    margin: 10px;
    text-align: center;
}

img {
    width: 300px;
    height: auto;
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px;
}
```

## CSS Exploration Challenge

Explore the following concepts from https://www.w3schools.com/w3css/default.asp:

1. **CSS Grid Layout**
2. **CSS Flexbox**
3. **CSS Transformations**
4. **CSS Animations**
5. **CSS Transitions**
6. **CSS Variables**
7. **Media Queries and Responsive Design**
8. **Advanced Pseudo-Classes and Pseudo-Elements**
9. **Advanced CSS Selectors**
10. **Themes and Dark Mode**
11. **CSS Preprocessors: Sass & Less**
12. **CSS Frameworks: Bootstrap, Foundation**
13. **CSS BEM (Block-Element-Modifier) Methodology**
14. **CSS for Interactions and Animation Effects**

Mastering these concepts will help you design advanced, appealing, and responsive web pages.