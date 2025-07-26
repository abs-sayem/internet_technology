# **HTML (Structure & Semantics)**

---

## 01: HTML & Basic Page Structure

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
* Bold: `<strong>`, Italic: `<em>`

```html
<h1>About Me</h1>
<p>My name is Sayem.<br>I am learning web development.</p>
<hr>
<p><strong>Hobbies:</strong> Reading, <em>Coding</em></p>
```

#### Variations:

1. Use all heading levels:

```html
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
```

2. Combine text styles:

```html
<p>This is <strong>important</strong> and <em>interesting</em> text.</p>
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
