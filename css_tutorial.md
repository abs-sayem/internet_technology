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
    - color --> sets font color
    - font-seze --> sets the size of the font
    - font-weight --> sets the thickness of the font
    - font-style --> sets the font style
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
    - content --> includes the content's height and width<br>
    - border --> line that surrounds the content, can have specific - width, style and color<br>
    - padding --> space between content and border<br>
    - margin --> space between the border of the content and surrounding elements. 
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

## CSS Positioning
- Allows to place elements precisely in desired place.
- **Properties:** static, relative, absolute, fixed, sticky.
- The properties offer flexibility for organizing content.
- For Example,
    - **`relative`** - moves an element to its normal position
    - **`absolute`** - places an element based on its closest positioned ancestor.

### `Static` Positioning:
- The default position behavior of an element. If no position property is diclered, the element considered it as default position: **static**.

### `Relative` Positioning:
- The element will move relative to its normal/actual position.
- Allows the use of **top**, **bottom**, **left** and **right** properties for adjustment.
    ```css
        .one {
            background-color: powderblue;
            position: relative;
            right: 50px;
        }
    ```

### `Absolute` Positioning:
- The element will move relativele to the nearest positioned (parent) element.
- If none, it positioned relative to the initial containing block (usually - the <html> element).
    ```css
        .one {
            background-color: powderblue;
            position: absolute;
            top: 50px;
            left: 0px;
        }
    ```

### `Fixed` Positioning:
- The element will be positioned relative to the browser window.
- Remain fixed even when the page is being scrolled.
    ```css
        .navbar {
            background-color: gray;
            position: fixed;
            top: 0px;
            width: 100%;
            text-align: center;
        }
    ```

### `Sticky` Positioning:
- The element acts like relative positioning until the element reaches a specified point during scrolling, then it become `fixed`.
    ```css
        .sticky-navbar {
            background-color: gray;
            position: sticky;
            top: 0px;
        }
    ```

### `Z-Index` Positioning:**
- Z-Index specifies the stack order of an element.
- Higher z-index valued element is displayed in front of lower valued element.
    ```css
        #first {
            background-color: gray;
            position: absolute;
            z-index: -1
            top: 30px;
            left: 30px;
        }
        #second {
            background-color: maroon;
            position: absolute;
            top: 10px;
            left: 10px;
        }
        #third {
            background-color: gray;
            position: absolute;
            z-index: -2
            top: 50px;
            left: 50px;
        }
    ```

## CSS Flexbox and Grid
### FlexBox
- One dimensional layout model, designed for arranging elements in a row or in a column.
- Simplifly the complex layout. **How?** - Elements can dynamically adjust their size and position within a container, depending on the available space.

#### Display Flex:
- defines a flex container; enables a flex context for all its direct children.
    ```css
        .container {
            display: flex;
        }
    ```

#### Flex Direction:
- defines the direction of the flex items, places in the flex container.
    ```css
        .container {
            display: flex;
            flex-direction: row | row-reverse | column | column-reverse;
        }
    ```

#### Justify Content:
- distributes extra free space left over when all the flex items on a line are inflexible or flexible but have reached their maximum size.
    ```css
        .container {
            display: flex;
            justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly;
        }
    ```

#### Align Items:
- defines the default behavior for how flex items are laid out along the cross-axis on the current line.
    ```css
        .container {
            display: flex;
            align-items: stretch | flex-start | flex-end | center | baseline;
        }
    ```

#### Gap:
- gap controls the space between flex items.
    ```css
        .container {
            display: flex;
            gap: 10px;
            gap: 10px 20px; /*row-gap column-gap*/
            row-gap: 10px;
            column-gap: 20px;
        }
    ```

#### **Flexbox Example**
- In index.html:
    ```html
        <!DOCTYPE html>
        <html lang="en">
            <head>
                <title>CSS Flex Document</title>
                <link rel="stylesheet" href="style.css" />
            </head>
            <body>
                <div class="parent">
                    <div class="child">
                        <p>Flexbox is a one-dimensional layout model, primarily designed for arranging elements in a row or in a column.</p>
                    </div>
                    <div class="child">
                        <p>
                            Flexbox is a one-dimensional layout model, primarily designed for arranging elements in a row or in a column.
                        </p>
                    </div>
                    <div class="child">
                        <p>Flexbox is a one-dimensional layout model, primarily designed for 
                            arranging elements in a row or in a column.</p>
                    </div>
                    <div class="child">
                        <p>
                            Flexbox is a one-dimensional layout model, primarily designed for 
                            arranging elements in a row or in a column.
                        </p>
                    </div>
                </div>
            </body>
        </html>
    ```
- In style.css: 
    ```css
        .parent {
            display: flex;
            flex-direction: row;
            gap: 10px;
            padding: 10px;
            height: 600px;
            background-color: tan;
            align-items: center;
            justify-content: center;
        }
        .child {
            border: 2px solid gray;
            padding: 10px;
            width: 200px;
        }
    ```