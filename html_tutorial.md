# **HTML (Structure & Semantics)**

## 1. HTML Basics Strunture
* **`<!DOCTYPE html>`** → Declares the document type (HTML5).

* **`<html>`** → Root element of the HTML document.
  ```html
  <!DOCTYPE html>
  <html>
    <head></head>
    <body></body>
  </html>
  ```

* **`<head>`** → Contains metadata (title, meta info, links, scripts, styles).
  ```html
  <!DOCTYPE html>
  <html>
    <head>
      <title>My Page</title>
      <meta charset="UTF-8">
      <meta font-family="Trebuchet MS">
      <style>body {color: silver}</style>   <!-- color: rgb(253, 235, 233) -->
      <link rel="stylesheet" href="style.css" />
      <link rel="script" href="script.js" />
    </head>
    <body></body>
  </html>
  ```

* **`<body>`** → Contains visible page content.
---
> #### Elements & Attributes:
  > **Element** → Defined by start `<tag>` and end `</tag>`.<br>
  > **Attribute** → Provides extra info inside the opening tag.<br>
    <p title="Tooltip text">This is a paragraph with an attribute.</p>

---
  * **`<h1>`–`<h6>`** → Define headings (h1 = largest, h6 = smallest).
  * **`<p>`** → Defines a paragraph.
  ```html
  <!DOCTYPE html>
  <html>
    <head></head>
    <body>
      <h>
      <p>Hello World</p>
    </body>
  </html>
  ```
  ```html
  <body><p>Hello World</p></body>
  ```

---

## 2. Elements & Attributes
* **Element** → Defined by start `<tag>` and end `</tag>`.
* **Attribute** → Provides extra info inside the opening tag.
  ```html
  <p title="Tooltip text">This is a paragraph with an attribute.</p>
  ```

---

## 3. Headings

* **`<h1>`–`<h6>`** → Define headings (h1 = largest, h6 = smallest).
  ```html
  <h1>Main Title</h1>
  <h3>Sub Heading</h3>
  ```

---

## 4. Paragraphs
* **`<p>`** → Defines a paragraph.
  ```html
  <p>This is a paragraph.</p>
  ```

* **`<br>`** → Line break.
  ```html
  Hello<br>World
  ```

* **`<hr>`** → Horizontal line (divider).
  ```html
  <hr>
  ```

---

## 5. Formatting
* **`<b>` / `<strong>`** → Bold text (strong = important).
  ```html
  <strong>Important text</strong>
  ```

* **`<i>` / `<em>`** → Italic text (em = emphasized).
  ```html
  <em>Highlighted text</em>
  ```

* **`<u>`** → Underlined text.
  ```html
  <u>Underlined</u>
  ```

* **`<mark>`** → Highlighted text.
  ```html
  <mark>Highlighted</mark>
  ```

---

## 6. Links
* **`<a>`** → Creates a hyperlink.
  ```html
  <a href="https://example.com" target="_blank">Visit Example</a>
  ```

---

## 7. Head (Extra Tags)
* **`<title>`** → Page title (browser tab).
* **`<meta>`** → Metadata (charset, description, viewport).
* **`<link>`** → Link to external resources (CSS, favicon).
* **`<style>`** → Internal CSS.
* **`<script>`** → JavaScript code.
  ```html
  <head>
    <title>My Site</title>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="style.css">
  </head>
  ```

---

## 8. Images
* **`<img>`** → Embeds an image.
  ```html
  <img src="image.jpg" alt="A sample image" width="200">
  ```

---

## 9. Tables
* **`<table>`** → Creates a table.
* **`<tr>`** → Table row.
* **`<th>`** → Table header cell.
* **`<td>`** → Table data cell.
  ```html
  <table border="1">
    <tr><th>Name</th><th>Age</th></tr>
    <tr><td>Alice</td><td>22</td></tr>
  </table>
  ```

---

## 10. Lists
* **`<ul>`** → Unordered list (bullets).
* **`<ol>`** → Ordered list (numbers).
* **`<li>`** → List item.
  ```html
  <ul>
    <li>Apple</li>
    <li>Banana</li>
  </ul>
  ```

---

## 11. Blocks & Layout
* **`<div>`** → Block-level container.
  ```html
  <div style="background:lightblue;">Block element</div>
  ```

* **`<span>`** → Inline container.
  ```html
  <p>This is <span style="color:red;">highlighted</span> text.</p>
  ```

* **Semantic layout tags**:
  * `<header>` → Page header.
  * `<footer>` → Page footer.
  * `<section>` → Page section.
  * `<article>` → Self-contained content.
  * `<aside>` → Sidebar content.
  ```html
  <header><h1>My Blog</h1></header>
  <section><article>Blog Post</article></section>
  ```

---

## 12. Forms
* **`<form>`** → Creates a form.
* **`<input>`** → Input field (`text`, `email`, `password`, etc).
* **`<textarea>`** → Multi-line text input.
* **`<select>` & `<option>`** → Dropdown menu.
* **`<button>`** → Button.

  ```html
  <form>
    <label>Name:</label>
    <input type="text"><br>
    <textarea></textarea><br>
    <select>
      <option>Option 1</option>
    </select><br>
    <button type="submit">Submit</button>
  </form>
  ```

---

## 13. Multimedia
* **`<audio>`** → Embed audio.
  ```html
  <audio controls>
    <source src="song.mp3" type="audio/mp3">
  </audio>
  ```

* **`<video>`** → Embed video.
  ```html
  <video controls width="300">
    <source src="movie.mp4" type="video/mp4">
  </video>
  ```

* **`<iframe>`** → Embed another webpage (e.g., YouTube).
  ```html
  <iframe src="https://example.com" width="300" height="200"></iframe>
  ```

---

# 01: HTML & Basic Page Structure

#### Theory:
* HTML stands for HyperText Markup Language.
* It structures content for the web using elements (tags).
* Basic structure:

  ```html
  <!DOCTYPE html>
  <html>
    <head>
      <title>My First Webpage</title>
    </head>
    <body>
      <h1>Hello, World!</h1>
    </body>
  </html>
  ```

#### Variations:

1. Add a paragraph and image:

  ```html
  <body>
    <h1>Hello, World!</h1>
    <p>This is my first web page.</p>
    <img src="logo.png" alt="Logo">
  </body>
  ```

2. Add meta tag and styles:

  ```html
  <head>
    <meta charset="UTF-8">
    <title>Styled Page</title>
    <style>body { font-family: Arial; }</style>
  </head>
  ```

#### Practice:

* Create a file `index.html`
* Add the above structure and open in a browser.

---

## 02: Text Formatting

#### Theory:

* Headings: `<h1>` to `<h6>`
* Paragraph: `<p>`
* Line Break: `<br>`
* Horizontal Line: `<hr>`
* Bold: `<strong>`, Italic: `<em>`, Deleted: `<del>`, Underlined: `<u>`, Highlighted: `<mark>`

  ```html
  <h1>About Me</h1>
  <p>My name is Learner.<br>I am learning web development.</p>
  <hr>
  <p><strong>Hobbies:</strong> Reading, <em>Coding</em>, <u>Teaching</u>, <mark>Documenting</mark></p>
  ```

#### Variations:

1. Use all heading levels:

  ```html
  <h1>Heading 1</h1>
  <h2>Heading 2</h2>
  <h3>Heading 3</h3>
  .
  .
  <h6>Heading 6</h6>
  ```

2. Combine text styles:

  ```html
  <p>This is <strong>important</strong>, <em>interesting</em> <del>and boring</del> text.</p>
  ```

#### Practice:

* Create an “About Me” section using formatting tags.

---

## 03: Links and Images

#### Theory:

* Links: `<a href="URL">Text</a>`
* Images: `<img src="path" alt="description">`

  ```html
  <a href="https://www.google.com">Visit Google</a>
  <img src="me.jpg" alt="My Photo" width="200">
  ```

#### Variations:

1. Open link in new tab:

  ```html
  <a href="https://example.com" target="_blank">External Site</a>
  ```

2. Link to another page in the project:

  ```html
  <a href="about.html">About Us</a>
  ```

3. Add image with height and border:

  ```html
  <img src="image.jpg" alt="Sample" height="150" style="border: 1px solid black;">
  ```

#### Practice:

* Link to external and internal pages.
* Add at least two images with alt text.

---

## 04: Lists

#### Theory:

* Ordered List: `<ol>`
* Unordered List: `<ul>`
* List Items: `<li>`

  ```html
  <h2>My To-Do List</h2>
  <ul>
    <li>Learn HTML</li>
    <li>Practice CSS</li>
  </ul>

  <h2>Steps to Cook Rice</h2>
  <ol>
    <li>Wash rice</li>
    <li>Boil water</li>
    <li>Add rice and cook</li>
  </ol>
  ```

#### Variations:

1. Nested Lists:

  ```html
  <ul>
    <li>Frontend
      <ul>
        <li>HTML</li>
        <li>CSS</li>
      </ul>
    </li>
  </ul>
  ```

2. Numbered list with types:

  ```html
  <ol type="A">
    <li>Option 1</li>
    <li>Option 2</li>
  </ol>
  ```

#### Practice:

* Create a recipe or to-do list webpage.

---

## 05: Tables

#### Theory:

* Elements: `<table>`, `<tr>`, `<th>`, `<td>`
* Attributes: `colspan`, `rowspan`

  ```html
  <table border="1">
    <tr>
      <th>Day</th>
      <th>Subject</th>
    </tr>
    <tr>
      <td>Monday</td>
      <td>Math</td>
    </tr>
  </table>
  ```

#### Variations:

1. Merged Header:

  ```html
  <tr>
    <th colspan="2">Weekly Schedule</th>
  </tr>
  ```

2. Merged Rows:

  ```html
  <tr>
    <td rowspan="2">Monday</td>
    <td>Math</td>
  </tr>
  <tr>
    <td>Physics</td>
  </tr>
  ```

#### Practice:

* Create a class routine using a table.

---

## 06: Forms

#### Theory:

* Elements: `<form>`, `<input>`, `<textarea>`, `<select>`, `<button>`

  ```html
  <form>
    <label for="name">Name:</label>
    <input type="text" id="name" name="name"><br>

    <label for="msg">Message:</label><br>
    <textarea id="msg" name="msg"></textarea><br>

    <label for="gender">Gender:</label>
    <select id="gender" name="gender">
      <option value="male">Male</option>
      <option value="female">Female</option>
    </select><br>

    <button type="submit">Submit</button>
  </form>
  ```

#### Variations:

1. Add checkboxes and radio buttons:

  ```html
  <label>Interests:</label><br>
  <input type="checkbox" name="interest" value="coding"> Coding
  <input type="checkbox" name="interest" value="reading"> Reading
  ```

2. Radio button group:

  ```html
  <label>Level:</label>
  <input type="radio" name="level" value="beginner"> Beginner
  <input type="radio" name="level" value="advanced"> Advanced
  ```

#### Practice:

* Build a contact form with at least 3 input fields.

---

## 07: Semantic HTML

#### Theory:

* Gives meaning to your page structure.
* Common tags: `<header>`, `<footer>`, `<nav>`, `<main>`, `<article>`, `<section>`

  ```html
  <header>
    <h1>My Blog</h1>
  </header>
  <main>
    <section>
      <article>
        <h2>First Post</h2>
        <p>This is my first blog post.</p>
      </article>
    </section>
  </main>
  <footer>
    <p>&copy; 2025 Sayem</p>
  </footer>
  ```

#### Variations:

1. Add navigation links:

  ```html
  <nav>
    <a href="home.html">Home</a> |
    <a href="about.html">About</a>
  </nav>
  ```

2. Include multiple articles:

  ```html
  <article>
    <h2>Post 1</h2>
    <p>Content for first post.</p>
  </article>
  <article>
    <h2>Post 2</h2>
    <p>Content for second post.</p>
  </article>
  ```

### Practice:

* Redesign a basic webpage using semantic tags for clarity and SEO.

---

# HTML Divs

## 01: What is a Div?

#### Theory:

* `<div>` stands for "division" and is a block-level container.
* It’s used to group HTML elements together and apply styles or scripts to them.
* It does **not** add meaning like semantic tags do.

  ```html
  <div>
    <p>This is inside a div</p>
  </div>
  ```

#### Variations:

1. Wrap multiple elements:

  ```html
  <div>
    <h1>Title</h1>
    <p>Description</p>
  </div>
  ```

2. Nest divs:

  ```html
  <div>
    <div>
      <p>Nested content</p>
    </div>
  </div>
  ```

#### Practice:

* Create a section with two paragraphs and wrap it in a `<div>`.

---

## 02: Styling a Div;

#### Theory:

* You can use CSS to style `<div>`: background, padding, margin, border, etc.
* Divs can be styled using classes or IDs.

  ```html
  <style>
    .box {
      background-color: lightblue;
      padding: 20px;
      border: 2px solid black;
    }
  </style>
  <div class="box">
    <p>This box is styled.</p>
  </div>
  ```

#### Variations:

1. Use `id` selector:

  ```html
  <style>
    #highlight {
      background-color: yellow;
    }
  </style>
  <div id="highlight">Important content</div>
  ```

2. Add inline styles:

  ```html
  <div style="border: 1px solid red; padding: 10px;">Inline styled div</div>
  ```

#### Practice:

* Create a colored box with border and padding using a class.

---

## 03: Layout with Divs (Grid & Columns)

#### Theory:

* Divs are often used to create multi-column layouts.
* Use `float`, `flexbox`, or `grid` for layout design.

#### Example using Float:

  ```html
  <style>
    .left { float: left; width: 50%; background: #f0f0f0; }
    .right { float: right; width: 50%; background: #d0d0d0; }
  </style>
  <div class="left">Left Side</div>
  <div class="right">Right Side</div>
  ```

#### Example using Flexbox:

  ```html
  <style>
    .container {
      display: flex;
    }
    .box {
      flex: 1;
      padding: 20px;
      border: 1px solid #000;
    }
  </style>
  <div class="container">
    <div class="box">Box 1</div>
    <div class="box">Box 2</div>
  </div>
  ```

#### Practice:

* Create a two-column layout using both `float` and `flexbox` methods.

---

## 04: Centering with Div

#### Theory:

* You can center content inside a div or center the div itself.

#### Center text:

  ```html
  <div style="text-align: center;">
    <p>Centered Text</p>
  </div>
  ```

#### Center div horizontally:

  ```html
  <div style="width: 200px; margin: 0 auto; background: #ccc;">Centered Box</div>
  ```

#### Center using Flexbox:

  ```html
  <style>
    .center-box {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }
  </style>
  <div class="center-box">
    <div>Perfectly Centered</div>
  </div>
  ```

#### Practice:

* Create a div that centers both vertically and horizontally.

---

## 05: Responsive Layouts with Div

#### Theory:

* Combine divs with media queries to make layouts responsive.
* Use percentage widths or CSS Grid/Flex.

  ```html
  <style>
    .responsive {
      display: flex;
      flex-wrap: wrap;
    }
    .item {
      flex: 1 1 100%;
    }
    @media (min-width: 600px) {
      .item {
        flex: 1 1 50%;
      }
    }
  </style>
  <div class="responsive">
    <div class="item">Item 1</div>
    <div class="item">Item 2</div>
  </div>
  ```

#### Practice:

* Build a mobile-first responsive two-column layout.

---

## 06: Advanced Techniques

#### Theory:

* Use CSS Grid with divs for advanced layouts.
* Animate divs using `@keyframes`.

#### Example: CSS Grid

  ```html
  <style>
    .grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 10px;
    }
    .grid-item {
      background: #eee;
      padding: 20px;
      text-align: center;
    }
  </style>
  <div class="grid">
    <div class="grid-item">1</div>
    <div class="grid-item">2</div>
    <div class="grid-item">3</div>
  </div>
  ```

#### Example: Animation

  ```html
  <style>
    .fade {
      animation: fadein 2s;
    }
    @keyframes fadein {
      from { opacity: 0; }
      to { opacity: 1; }
    }
  </style>
  <div class="fade">Fades in!</div>
  ```

#### Practice:

* Create a grid layout and add animation to divs.

---

### Summary

* `<div>` is essential for structuring and styling content.
* Used in layout, grouping, styling, animation, and responsiveness.
* Mastery of `<div>` is key to building modern web pages.

---

**Challenge Project:**

* Create a responsive blog layout with:

  * Header, main content, sidebar, and footer
  * Use flexbox and grid
  * Apply styling and add animation
