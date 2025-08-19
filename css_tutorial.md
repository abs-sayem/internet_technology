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