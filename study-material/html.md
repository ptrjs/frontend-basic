# HTML: Hypertext Markup Language

HTML, or Hypertext Markup Language, is a markup language used to create the structure and organize content on a web page. HTML allows web developers to define elements such as text, images, links, tables, forms, and more, and specify how these elements should be displayed in the web browser.

## How HTML Works

HTML works using a series of tags or elements placed in an HTML document. Each tag has a specific function and represents different elements. For example, the `<h1>` tag is used to create a level 1 heading, the `<p>` tag is used to mark a paragraph, and the `<a>` tag is used to create a hyperlink to another web page.

## Simple HTML Document Example

```html
<!DOCTYPE html>
<html>
<head>
    <title>HTML Example</title>
</head>
<body>
    <h1>Welcome to My Web Page</h1>
    <p>This is a sample paragraph of text.</p>
    <a href="https://www.example.com">Visit Example.com</a>
</body>
</html>
```

## Understand tags, elements, and attributes

Tags, elements, and attributes are basic concepts in HTML that form the structure and content of a web page. Let's take a look at each of them:

1. **Tag**:
   - A tag is a basic unit in HTML used to wrap elements on a web page. They are usually written inside angle brackets, like: `<tag>`. HTML tags always open with `<` and close with `>`. Most elements use both opening and closing tags, such as `<p>` for opening a paragraph and `</p>` for closing it. Some tags, such as `<img>` or `<br>`, do not have closing tags and are usually self-closing, like `<img src="image.jpg" />`.

2. **Element**:
   - An element is a combination of the opening tag, content, and closing tag (if needed) that forms a functional unit in an HTML document. For example, a paragraph element looks like this:
     ```html
     <p>This is a paragraph.</p>
     ```
   - Elements can also be nested, meaning other elements are placed inside an element. This creates a hierarchy of elements in an HTML document.

3. **Attribute**:
   - Attributes are additional information placed inside an HTML tag to provide specific details or parameters about an element. They always consist of an attribute name and value, separated by an equals sign (`=`). An example of attributes in an image element is `src` (source of the image) and `alt` (alternative text if the image fails to load):
     ```html
     <img src="image.jpg" alt="Image Description" />
     ```
   - Attributes allow you to customize or control the behavior of HTML elements.

So, in HTML, tags are used to wrap elements, elements are combinations of tags, and attributes provide extra information about those elements. These are fundamental concepts for understanding how HTML organizes and displays information on web pages.

## Understand the basic structure of HTML

After learning about the building blocks of HTML, you also need to understand the core framework as the base structure of an HTML document. A single HTML document contains hundreds of tags. Therefore, it is helpful to understand the basic skeleton used whenever you create an HTML document.

`<!doctype HTML>`: used to tell the browser that this is an HTML document.

`<HTML></HTML>`: tag that marks the start and end of the HTML document.

`<head></head>`: contains metadata for the HTML document such as the tab title, description, etc.

`<body></body>`: will contain the content of the page for website creation.

As additional information, if you are learning HTML and curious about the HTML document of a website, you can visit any web page, right-click and select “View Page Source”. You can also use the keyboard shortcut Ctrl + U.

## Common HTML Tags

Here are some common tags used in HTML to create and format content on web pages:

1. **Basic Tags:**
   - `<html>`: Defines the HTML document.
   - `<head>`: Contains metadata information such as page title and stylesheet links.
   - `<title>`: Sets the page title shown on the browser title bar.
   - `<meta>`: Used to include metadata, such as character set and page description.
   - `<body>`: Contains all content to be displayed on the web page.

2. **Text:**
   - `<h1>`, `<h2>`, `<h3>`, ..., `<h6>`: Create headings with different importance levels.
   - `<p>`: Creates a text paragraph.
   - `<a>`: Creates a link to another web page or resource.
   - `<strong>`: Makes text bold.
   - `<em>`: Makes text italic.
   - `<u>`: Underlines text.
   - `<br>`: Inserts a line break.
   - `<hr>`: Inserts a horizontal line to separate content.

3. **Lists and Tables:**
   - `<ul>`: Creates an unordered list.
   - `<ol>`: Creates an ordered list.
   - `<li>`: Defines an item in a list.
   - `<dl>`: Creates a definition list.
   - `<dt>`: Defines a term in a definition list.
   - `<dd>`: Defines a description in a definition list.
   - `<table>`: Creates a table.
   - `<tr>`: Defines a row in a table.
   - `<th>`: Defines a header cell in a table.
   - `<td>`: Defines a data cell in a table.

4. **Images:**
   - `<img>`: Inserts an image into the page.
   - `<figure>`: Defines self-contained content, such as an image or video.
   - `<figcaption>`: Provides a caption for the `<figure>` element.

5. **Forms:**
   - `<form>`: Creates a user input form.
   - `<input>`: Creates various types of input fields like text, password, checkbox, etc.
   - `<textarea>`: Creates a larger text area for long text input.
   - `<select>`: Creates a dropdown list.
   - `<button>`: Creates a button in a form.
   - `<label>`: Defines a label for form elements.

6. **Multimedia:**
   - `<audio>`: Embeds audio.
   - `<video>`: Embeds video.
   - `<iframe>`: Embeds content from another website.

7. **Comment:**
   - `<!-- This is a comment -->`: Adds a comment in HTML code for documentation or organization.

These are just a few basic tags in HTML. There are many other tags available to build web pages with more features and functionality. These HTML tags build the structure and content of a web page, and with CSS and JavaScript, you can control the appearance and behavior of your web page to meet your needs.

## ID and Class

In HTML, "id" and "class" are attributes used to identify and refer to specific HTML elements. They are used in combination with CSS and JavaScript to modify or control the appearance and behavior of those elements.

1. **ID (Identifier):**
   - "id" is an attribute that gives a unique identity to a specific HTML element on a page. Each "id" must be unique within the HTML document.
   - In CSS, you can refer to an element by its "id" using the hash symbol (`#`). For example, if you have an element like `<div id="header">`, you can target it in CSS like this:
     ```css
     #header {
         background-color: #ff6600;
         color: white;
     }
     ```
   - In JavaScript, you can refer to an element by its "id" to modify or manipulate it:
     ```javascript
     var header = document.getElementById("header");
     header.innerHTML = "Home Page";
     ```

2. **Class:**
   - "class" is an attribute used to group one or more HTML elements together. You can assign the same class to multiple elements.
   - In CSS, refer to elements by their class using a dot (`.`). For example, if you have elements with the class "menu", you can target them like this:
     ```css
     .menu {
         font-size: 18px;
         color: #333;
     }
     ```
   - In JavaScript, you can select elements by their class name and apply certain actions or changes:
     ```javascript
     var menus = document.getElementsByClassName("menu");
     for (var i = 0; i < menus.length; i++) {
         menus[i].style.fontWeight = "bold";
     }
     ```

Using "id" and "class" allows you to manipulate elements in detail on your web page. Use "id" for unique elements, and "class" for elements that can be grouped by characteristics or styles. In practice, you'll use a combination of both to precisely control your web page.

## Logic Challenge: Create Your First HTML

Create a file named `index.html` in your VS Code, and open it. The `index.html` can automatically be opened in a browser using a browser extension.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Simple Page</title>
</head>
<body>
    <h1>Welcome to the Simple Page</h1>
    <p>This is an example of a simple HTML page.</p>
    <ul>
        <li>Item 1</li>
        <li>Item 2</li>
        <li>Item 3</li>
    </ul>
    <p>Thank you for visiting this page.</p>
</body>
</html>
```

![image](https://github.com/user-attachments/assets/bc1f1f44-299c-4e70-ac77-490ff4df32bb)


Recreate your own version of this HTML, try out all the tags and submit your HTML file.

*USE ADVANCED OR UNIQUE HTML TAGS TO INCREASE YOUR EXPERIENCE*

## Explore Challenge

https://www.w3schools.com/html/

W3Schools is the easiest way to explore HTML. Try diving into every topic and experiment with all the HTML tags you learn.
