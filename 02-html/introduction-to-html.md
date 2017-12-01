# Introduction to HTML

## What is HTML?
HTML (HyperText Markup Language) displays your content surrounded by tags (that look like this: `<p></p>`) that denote what that content is.

## Basics
Here's a basic HTML document structure:
```html
<!DOCTYPE html>
<html lang="en-US">  
    <head>
        <!-- Put information about your webpage (metadata) here inside the <head>! -->
    </head>

    <body>
        <!-- Put your own content here inside the <body>! -->
    </body>
</html>
```

Here are some commonly used tags:
- Headings `<h1></h1>` `<h2></h2>`...all the way to `<h6></h6>`
- Paragraph `<p></p>`
- Italics `<em></em>`
- Bold `<strong></strong>`
- Link `<a href="path/url-you-want-to-link-to">hyperlink text to display</a>`
- Image `<img src="path/url-you-want-to-link-to">`
- Embedded media (like Youtube videos) `<iframe src="path/url-you-want-to-link-to"></iframe>`
- Divider `<div></div>`
- Bulleted (unordered) lists
  ```html
  <ul>
    <li>Item 1</li>
    <li>Item 2</li>
  </ul>
  ```
- Numbered (ordered) lists
  ```html
  <ol>
    <li>Item 1</li>
    <li>Item 2</li>
  </ul>
  ```