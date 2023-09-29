# Introduction to HTML and CSS

This section will teach me the basics of HTML and CSS, the two foundational building blocks of almost everything on the web.

## HTML and CSS

**HTML** and **CSS** are two languages that work together to create everything that you see when **look** at something on the internet.

- **HTML** is the raw data that a webpage is built out of.
    - Text
    - Links
    - Cards
    - Lists
    - Buttons
    - .....

- **CSS** is what adds style to those plain elements.

**HTML** puts information on a webpage, and **CSS** positions that information gives it the color, changes the font, and makes it look great!

## Elements and Tags

Almost all elements on an HTML page are just pieces of content wrapped in opening and closing HTML tags.

A full paragraph element looks like this:

```html
<p> some text content </p>
```

> You can think of elements as containers for content.

HTML has a ***vast list of predefined tags*** that you can use to create all kinds of different elements.

Using the correct tag can have a big impact on two aspects of your sites:
- How they are ranked in search engines.
- And how accessible they are to users who rely on assistive technologies:
    - like screen readers, to use the internet.

> Using the correct elements for content is called **SEMANTIC HTML**.

## HTML Boilerplate

All **HTML** documents have the same basic structure or boilerplate that needs to be in place before anything useful can be done. 

- **DOCTYPE:**
    - Every HTML page starts with a doctype declaration.
    - The doctype's purpose is to tell the browser what version of HTML is should use to render the document
    ```html
    <!DOCTYPE html>
    ```

- **HTML element:**
    - This is what's known as the **ROOT** element of the document.
    - Meaning that every other element in the document will be a descendant of it.
    ```html
    <!DOCTYPE html>

    <html lang="en">
    </html>
    ```

- **HEAD element:**
    - Is where we put important **meta-information** ***about*** our webpage.

- **CHARSET meta element:**
    - Setting the encoding is very important because it ensures that the webpage will display special symbols and characters from different languages correctly in the browser.

- **TITLE element:**
    - The title element is used to give webpages a **human-readable** title which is displayed in our webpage's browser tab.

    ```html
    <!DOCTYPE html>

    <html lang="en">
        <head>
            <meta charset="UTF-8">
            <title>My first web page</title>
        </head>
    </html>
    ```

- **BODY element:**
    - This is where all the content will be displayed to users.
        - text
        - images
        - lists
        - links
        - ....
    
    ```html
    <!DOCTYPE html>
    <html lang="en">

        <head>
            <meta charset="UTF-8">
            <title>My first web page</title>
        </head>

        <body>
        </body>

    </html>
    ```

    [boilerpalate index.html](/TOP-Training/foundations/HTML-foundations/html-boilerplate/index.html)

## Working with text

Most content on the web is ***text-based***, so you will find yourself needing to work with **HTML** text elements quite a bit.

- **PARAGRAPHS elements:**
    - If we want to create paragraphs in HTML, we need to use the paragraph element:
    ```html
    <body>
        <p> This is the paragraph element </p>
    </body>
    ```

- **HEADINGS elements:**
    - There are 6 different levels of headings starting from `<h1>` to `<h6>`.
    - The number within a heading tag represents the heading's level.
    - The largest and most important heading is `<h1>`, while `<h6>` is the tiniest heading at the lowest level.
    ```html
    <body>
        <h1>This is a heading 1</h1>
        <h2>This is a heading 2</h2>
        <h3>This is a heading 3</h3>
        <h4>This is a heading 4</h4>
        <h5>This is a heading 5</h5>
        <h6>This is a heading 6</h6>
    </body>
    ```
    > Using the correct level of heading is important as levels provide a hierarchy to the content.

- **STRONG element:**
    - This element makes text bold.
    - It also semantically marks text as important.
    - This affects tools like:
        - **screen readers** that users with visual impairments will rely on to use your website.
        - The tone of voice on some **screen readers** will change to communicate the importance of the text within a `<strong>` tag.
    ```html
    <body>
        <p>Lorem ipsum dolor sit amet, <strong>consectetur</strong> adipiscing elit.</p>
    </body>
    ```

- **EM element:**
    - This element makes text italic.
    - It also semantically places emphasis on the text,  which again may affect things like **screen readers**.
    ```html
    <body>
        <p>Lorem <em>ipsum</em> dolor sit amet</p>
    </body>
    ```

- **NESTING AND INDENTATION**
    - When we nest elements within other elements, we create a parent-and-child relationship between them.
    ```html
    <body> <!-- this is the parent element -->
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p> <!-- child element -->
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p> <!-- child element -->
        <!-- the two paragraphs in this example are siblings -->
    </body>
    ``` 
    > Just as in human relationships, HTML parent elements can have many children

- **HTML Comments**:
    - Comments are not visible to the browser.
    - They allow us to get some context about something in the code.
    ```html
    <!--This is a comment in html -->
    ```

## Lists

List are everywhere on the web.

- **UNORDERED LISTS**
    - If you want to have a list of items where the order doesn't matter, then you can use an unordered list.
    - Unordered lists are created using `<ul>` parent element and `<li>` child element.
    ```html
    <body>
        <ul> <!-- this create the unordered list -->
            <li>cat</li>
            <li>dog</li> <!--this create the items in the unordered list-->
            <li>bird</li>
        </ul>
    </body>
    ```
    > Each list item in an unordered list begins with a bullet point.

- **ORDERED LISTS**
    - If you instead want to create a list of items where the order does matter, like step-by-step instructions, then you can use an ordered list.
    ```html
    <body>
        <ol> <!-- this create the ordered list -->
            <li>cat</li>
            <li>dog</li> <!--this create the items in the ordered list-->
            <li>bird</li>
        </ol>
    </body>
    ```
    > Each list item in an ordered list begins with a number instead.

## Links and Images

Links are one of the key features of HTML.

- They allow us to link to other HTML pages on the web.

> In fact, this is why it's called the web.

- **ANCHOR elements:
    - An anchor element is defined by wrapping the text or another HTML element we want to be a link with `<a>` tag.
    ```html
    <!-- href is an attribute. -->
    <!-- href = hyperlink reference. -->
    <!-- value = is the destination we want our link to got to. -->
    <!-- target = where the linked resource will be opened.  -->
    <a href="value" target="_blank" rel="noopener noreferrer">click me</a>
    ```

- **IMAGES**
- To display an image in HTML we the `<img>` element.
```html
<!--src = tell the browser where the image file is located.-->
<!--alt = describe an image -->
<img src="" alt="" height="" width="">
```

## Commit Messages
