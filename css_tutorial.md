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
### Typography
- **Attribures**
    - color ==> sets font color
    - font-seze ==> sets the size of the font
    - font-weight ==> sets the thickness of the font
    - font-style ==> sets the font style
- **Example**
    ```css
        p {
            color: lightblue;
            font-size: 18px;
            font-weight: 700;
            font-style: italic;
        }
    ```
- **Attribures**
    - content ==> includes the content's height and width<br>
    - border ==> line that surrounds the content, can have specific - width, style and color<br>
    - padding ==> space between content and border<br>
    - margin ==> space between the border of the content and surrounding elements. 
- **Example**
    ```css
        .box {
            width: 200px;
            height: 100px;
            border: 2px solid gray;
            padding: 20px;
            margin: 10px;
        }
    ```