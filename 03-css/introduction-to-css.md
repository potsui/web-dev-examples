# More HTML and Introduction to CSS

## Introduction to CSS
Right now, our HTML looks a little plain. It is simply styled by the defaults from the user's browser. This is where **CSS (Cascading Style Sheets)** come in.

There are different ways to add CSS to your HTML:
- Inline
   ```html
   <h1 style="color:red;">Red heading</h1>
   ```
- Not inline, but still within the HTML
   ```html
   <style>
     h1 {
       color: red;
     }
   <\style>
   ```
- Link to an external style sheet
   ```html
   <link rel="stylesheet" type="text/css" href="main.css" />
   ```
   
   Then, in a separate file called *main.css*:
   ```css
     h1 {
       color: red;
     }
   ```
   
As you can see, you style an element by referring to its tag (like `h1`), followed by curly braces. Inside, you specify rules, such as `color: red;`. Each rule changes one of that element's properties.

## Selectors
Say you have three elements that look similar.
```html
<p>Hi, I want to be colored red</p>
<p>Hi, I want to be colored blue</p>
<p>Hi, I want to be colored yellow</p>
```
How can you style them differently? You can do so by labelling them by with an **id**, which is unique to *only one element per page*. It's like calling someone out by their name; only one person in the room has that name.
```html
<p id="red-text">Hi, I want to be colored red</p>
<p id="blue-text">Hi, I want to be colored blue</p>
<p id="yellow-text">Hi, I want to be colored yellow</p>
```
Then you can style them like so:
```css
#red-text {
	color: red;
}
#blue-text {
	color: blue;
}
#yellow-text {
	color: yellow;
}
```
What if you want to make only the red and blue text bigger? You could add them individually, but that would become a pain for many elements. Instead, you can add a **class** to them, which groups them together in a category. You can use the same class for multiple elements that you want to have the same property. It's like calling someone (or a group of people) by some thing they have in common, like "hey, all people who are graphic designers!"

Building on our current example,

```html
<p id="red-text" class="bigger-text">Hi, I want to be colored red</p>
<p id="blue-text" class="bigger-text">Hi, I want to be colored blue</p>
<p id="yellow-text">Hi, I want to be colored yellow</p>
```

Then you can style them like so:
```css
.bigger-text {
	font-size: 16px;
}
```

ID and class are types of **selectors**, which are patterns you use to select elements you want to style.

## Divs in HTML
Use the `<div></div>` tag to create imaginary "boxes" around your content. These boxes will come to be extremely useful for styling your elements.
```html
<div>
    <h1>Hi, I'm in a heading in a div</h1>
</div>
```

## Box Model TODO
![Box model diagram](box-model.png)