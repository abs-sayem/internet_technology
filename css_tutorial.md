# CSS (Cascading Style Sheet)
### Inline CSS:
- applied directly to the HTML element using the style attribute.
    ```html
        <p style="text-align: justify;">This paragraph contains inline CSS.</p>
    ```
### Internal CSS:
- defined within the <style> tag in the <head> section of the HTML document.
    ```html
        <!DOCTYPE html>
        <html lang="en">
        <head>
            <style>
                h2 { text-align: center; color: red; }
            </style>
        </head>
        <body>
            <h2>This heading is with internal CSS.</h2>
        </body>
    ```
### External CSS:
- defined in a seperate CSS file and linked to the HTML document using the <link> tag.
    - `index.html`
    ```html
        <!DOCTYPE html>
        <html lang="en">
        <head>
            <link rel="stylesheet" href="style.css"/>
        </head>
        <body>
            <h2>This heading is with internal CSS.</h2>
        </body>
    ```
    - `style.css`
    ```css
        h2 {
            text-align: center;
            color: red;
        }
    ```
---
## CSS Selectors:
### Element Selector:
- Select all instances of a particular HTML element.
    ```css
        p {
            color: lightblue;
        }
    ```
### Class Selector:
- Selects elements with a specific class attribute.
    ```css
        .container {
            background-color: silver;
        }
    ```
### ID Selector:
- Selects a single element with a specific id attribute.
    ```css
        #navbar {
            background-color: pink;
        }
    ```
---

## CSS Typography and CSS Box Model
<table>
    <tr>
        <th>Typography</th>
        <th>Box Model</th>
    </tr>
    <tr>
        <th>Attributes</th>
        <th>Example</th>
        <th>Attributes</th>
        <th>Example</th>
    </tr>
</table>