# How To Add CSS

- when a browser reads a style sheet, it formats the HTML document according to the info in the style sheet

## Three Ways to Inset CSS

1. External CSS
2. Internal CSS
3. Inline CSS

## External CSS

- change the look of an entire website by changing just one file
- each HTML page must include a reference to the external style sheet inside of the `<link>` element in the `<head>` section of the HTML page

```html
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

- the external style sheet can be written in any text editor, must be saved with a .css extension, and cannot contain any HTML tags

mystyle.css:
```css
body {
  background-color: lightblue;
}

h1 {
  color: navy;
  margin-left: 20px;
}
```

NOTE: do not add a space between the property value and the unit: 
```css
/* Incorrect: */
p {
    margin-left: 20 px;
}
/* Correct: */
p {
    margin-left: 20px;
}
```

## Internal CSS

- can be used if one single HTML page has a unique style
- the internal style is defined inside the `<style>` element in the `<head>` section:

```html
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

## Inline CSS

- used to apply a unique style for a single element
- to use an inline style, add the style attribute to the relevant element
- the style attribute can contain any CSS property

```html
<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html>
```

## Multiple Style Sheets

- if some properties have been defined for the same selector in different style sheets, the value from the last read style sheet will be used

Assume an external style sheet looks like:
```css
h1 {
  color: navy;
}
```

If the internal style is defined after the external style, the internal style wins:

```css
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
<style>
h1 {
  color: orange;
}
</style>
</head>
```

If the internal style is defined before the external style, the external style wins:

```css
<head>
<style>
h1 {
  color: orange;
}
</style>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
```

## Cascading Order

- What style is used when more than one style is specified for an HTML element?
- Priority list:
1. Inline style (inside an HTML element)
2. External and internal style sheets (in the head section)
3. Browser default
