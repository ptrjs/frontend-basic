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
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Ice Cream Shop</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>🍦 Ice Cream Paradise</h1>
    <p>Treat yourself to happiness</p>
  </header>

  <nav>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">Menu</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <main>
    <section class="menu-section">
      <h2>Our Favorite Flavors</h2>
      <div class="ice-cream-grid">
        <div class="ice-cream-card">
          <img src="https://i.ibb.co/vC01GPg4/delicious-ice-cream-studio.jpg" alt="Vanilla Ice Cream">
          <h3>Vanilla Ice Cream</h3>
          <p>Smooth and classic taste of vanilla bean.</p>
          <span class="price">Rp 10.000</span>
        </div>
        <div class="ice-cream-card">
          <img src="https://i.ibb.co/67BYs2RR/melting-ice-cream-cone.jpg" alt="Triple Trouble">
          <h3>Triple Trouble</h3>
          <p>Three scoops of ultimate pleasure!</p>
          <span class="price">Rp 30.000</span>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 Ice Cream Paradise</p>
  </footer>
</body>
</html>

```

### `style.css`
```css
body {
  font-family: 'Comic Sans MS', cursive, sans-serif;
  margin: 0;
  padding: 0;
  background: #faf8f9;
  color: #333;
}

header {
  background: #ffd3e0;
  text-align: center;
  padding: 40px 20px;
  color: #5b2c6f;
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}

header h1 {
  margin: 0;
  font-size: 2.5em;
}

header p {
  font-size: 1.2em;
  margin-top: 10px;
}

nav ul {
  list-style: none;
  display: flex;
  justify-content: center;
  background-color: #ff92a5;
  margin: 0;
  padding: 10px 0;
}

nav ul li {
  margin: 0 20px;
}

nav ul li a {
  text-decoration: none;
  color: white;
  font-weight: bold;
  transition: color 0.3s;
}

nav ul li a:hover {
  color: #ffe;
}

.menu-section {
  padding: 40px 20px;
}

.menu-section h2 {
  text-align: center;
  color: #d63384;
  margin-bottom: 30px;
}

.ice-cream-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 20px;
  max-width: 1000px;
  margin: 0 auto;
}

.ice-cream-card {
  background: white;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  padding: 20px;
  text-align: center;
}

.ice-cream-card img {
  width: 100%;
  border-radius: 12px;
  height: auto;
}

.ice-cream-card h3 {
  margin: 15px 0 10px;
  color: #ff5e99;
}

.ice-cream-card p {
  font-size: 0.95em;
  color: #555;
}

.price {
  display: inline-block;
  margin-top: 10px;
  font-weight: bold;
  color: #5b2c6f;
}

footer {
  background: #ff92a5;
  color: white;
  text-align: center;
  padding: 15px;
  margin-top: 40px;
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

## Exercise 😈
- [Exercise 1](https://github.com/ptrjs/frontend-basic/blob/main/exercise-material/exercise1.md)
