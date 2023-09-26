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

> You can think of elements as conainers for content.

HTML has a ***vast list of predefined tags*** that you can use to create all kind of different elements.

Using the correct tag can have a gig impact on two aspects of yor sites:
- How they are ranked in search engines.
- And how accessible they are to users who rely on assistive technologies:
    - like screen readers, to use the internet.

> Using the correct elements for content is call **SEMANTIC HTML**.

## HTML Boilerplate

All **HTML** documents hve the same basic structure or boilerplate that needs to be in place before anything useful can be done. 

- DOCTYPE: 
    - Every HTML page starts with a doctype declaration.
    - The doctype's purpose is to tell the browser what version of html is should use to render the document
    ```html
    <!DOCTYPE html>
    ```

- HTML element:
    - This is what's known as the **ROOT** element of the document.
    - Meaning that every other element in the document will be a descendant of it.
    ```html
    <!DOCTYPE html>

    <html lang="en">
    </html>
    ```

- HEAD element:
    - Is where we put important **meta-information** ***about*** our webpage.

- CHARSET meta element:
    - Setting the encoding is very important because it ensuere that the webpage will deisplay special symobls and characters from different languages correctly in the browser.

- TITLE element:
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

- BODY element:
    - This is where all the content will be displayed to users will go.
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

