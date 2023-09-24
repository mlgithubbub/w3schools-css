# What is CSS?

- stands for Cascading Style Sheets
- describes how HTML elements are to be displayed on screen, paper or other media
- saves a lot of work, because can control the layout of multiple web pages at once
- external stylesheets are stored in CSS files

## CSS Demo - One HTML Page - Multiple Styles!

## Why Use CSS?

- to define styles for web pages including design, layout and variations in display for different devices and screen sizes

Example:
```css
body {
  background-color: lightblue;
}

h1 {
  color: white;
  text-align: center;
}

p {
  font-family: verdana;
  font-size: 20px;
}
```

## CSS Solved a Big Problem

- HTML was never intended to contain tags for formatting a web page
- HTML was created to describe the content of a web page, like:

```html
<h1>This is a heading</h1>

<p>This is a paragraph.</p>
```
- When tags like `<font>` and color attributes were added to HTML 3.2 it started a nightmare for developers
- It was a long and expensive process to add font and color info to every page
- To solve this problem, the World Wide Web Consortium (W3C) created CSS
- CSS removed the style formatting from the HTML page

## CSS saves a lot of work

- style definitions are usually saved in external .css files
- you can change the entire look of a website just by changing one file!
