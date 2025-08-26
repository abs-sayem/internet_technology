# **HTML (Structure & Semantics)**

## 1. HTML Basics Strunture
### `<!DOCTYPE html>` → Declares the document type (HTML5).

### `<html>` → Root element of the HTML document.
  ```html
  <!DOCTYPE html>
  <html>
    <head></head>
    <body></body>
  </html>
  ```

### `<head>` → Contains metadata (title, meta info, links, scripts, styles).
* **`<title>`** → Page title (browser tab).
* **`<meta>`** → Metadata (charset, description, viewport).
* **`<link>`** → Link to external resources (CSS, favicon).
* **`<style>`** → Internal CSS.
* **`<script>`** → JavaScript code.
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

### `<body>` → Contains visible page content.
---
#### Elements & Attributes:
* **Element** → Defined by start `<tag>` and end `</tag>`.<br>
* **Attribute** → Provides extra info inside the opening tag.<br>
```html
  <p title="Tooltip text">This is a paragraph with an attribute.</p>
```
---

* **`<h1>`–`<h6>`** → Define headings (h1 = largest, h6 = smallest).
* **`<p>`** → Defines a paragraph.
* **`<article>`** → Defines independent piece of content. Can contain - headings, paragraph, ...
  ```html
  <!DOCTYPE html>
  <html>
    <head></head>
    <body>
      <h1>Internet Technology</h1>
      <p>This is the paragraph that represents a block of text. Can not contain any other elements.</p>
      <article>
        <h2>Article</h2>
        <p>Article used for things like - blog posts, new articles, or any block of content that can stand alone.</p>
        <p>Article indicates this chunk is a meaningful and complete content.</p>
      </article>
    </body>
  </html>
  ```
#### Formatting
* **`<b>` / `<strong>`** → Bold text (strong = important).
* **`<i>` / `<em>`** → Italic text (em = emphasized).
* **`<u>`** → Underlined text.
* **`<mark>`** → Highlighted text.
* **`<del>`** → Deleted text.
* **`<br>`** → Line break.
* **`<hr>`** → Horizontal line (divider).
  ```html
  <!DOCTYPE html>
  <html>
    <head></head>
    <body>
      <h1><mark>Internet Technology</mark></h1>
      <p>This is the paragraph that represents a block of text.<br><del>Can contain</del> Can not contain any other elements.</p>
      <article>
        <h2><u>Article</u></h2>
        <p>Article used for things like - <b>blog posts</b>, <strong>new articles</strong>, or any block of content that can stand alone.</p>
        <p>Article indicates this chunk is a <i>meaningful</i> and <em>complete</em> content.</p>
      </article><hr>
    </body>
  </html>
  ```

---

#### Links and Images
* **`<a>`** → Creates a hyperlink.
* **`<img>`** → Embeds an image.
  ```html
  <a href="https://example.com">Visit Example</a>
  <a href="https://example.com" target="_blank">Visit Example</a>   <!-- Opens in new tab -->

  <img src="image.jpg" alt="descript_image" width=100% height="400px">
  ```

---

## 9. Tables
* **`<table>`** → Creates a table.
* **`<tr>`** → Table row.
* **`<th>`** → Table header cell.
* **`<td>`** → Table data cell.
  ```html
  <table border="1">
    <tr><th>Std Id</th><th>Attance</th><th>Mid</th><th>Final</th></tr>
    <tr><td>CCE001</td><td>10</td><td>24</td><td>40</td></tr>
    <tr><td>CCE002</td><td>10</td><td>25</td><td>44</td></tr>
    <tr><td>CCE003</td><td>8</td><td>20</td><td>48</td></tr>
    <tr><td>CCE004</td><td>10</td><td>30</td><td>38</td></tr>
    <tr><td>CCE005</td><td>7</td><td>20</td><td>50</td></tr>
  </table>
  ```
* **`colspan`** → Merge table colums.
* **`rowspan`** → Merge table rows.
  ```html
        <table border="1" cellpadding="5" cellspacing="0">
            <tr><th colspan="10">Web Programming Lab Records</th></tr>
            <tr>
                <th rowspan="2">Std Id</th>
                <th colspan="2">Lab-01</th>
                <th colspan="2">Lab-02</th>
                <th colspan="2">Lab-03</th>
                <th colspan="2">Total</th>
                <th rowspan="2">Final<br>(attendacne % marks)</th>
            </tr>
            <tr>
                <th>Attend</th><th>Marks</th>
                <th>Attend</th><th>Marks</th>
                <th>Attend</th><th>Marks</th>
                <th>Attend</th><th>Marks</th>
            </tr>
            <tr>
                <td>CCE001</td>
                <td>Y</td><td>10</td>
                <td>Y</td><td>10</td>
                <td>Y</td><td>10</td>
                <td>3</td><td>30</td>
                <td>10</td>
            </tr>
            <tr>
                <td>CCE002</td>
                <td>Y</td><td>10</td>
                <td>N</td><td>00</td>
                <td>Y</td><td>10</td>
                <td>2</td><td>20</td>
                <td>7</td>
            </tr>
            <tr>
                <td>CCE003</td>
                <td>Y</td><td>00</td>
                <td>N</td><td>00</td>
                <td>Y</td><td>10</td>
                <td>2</td><td>10</td>
                <td>4</td>
            </tr>
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
