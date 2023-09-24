# CSS Selectors

- a `CSS selector` selects the HTML element(s) you want to style

## CSS Selectors

- used to find/select HTML elements you want to style
- 5 Categories
    1. Simple selectors (name, id, class)
    2. Combinator selectors (select elements based on a specific relationship bewtween them)
    3. Pseudo-class selectors (select elements based on a certain state)
    4. Pseudo-elements selectors (select and style a part of an element)
    5. Attribute selectors (select elements based on an attribute or attribute value)

## The CSS element Selector

- the `element selector` selects HTML elements based on the element name:

```css
p {
  text-align: center;
  color: red;
}
```

## The CSS id Selector

- the `id selector` uses the id attribute of an HTML element to select a specific element
- the id of an element is unique within a page, so the id selector only selects one unique element
- to select an item with a specific id, write # (hash) + the id:

```css
/* applies to all HTML elements with id="para1" */
#para1 {
  text-align: center;
  color: red;
}
```


## The CSS class Selector

- the `class Selector`  selects HTML elements with a specific class attribute
- to select elements with a specific class, write: . (period) + the class name:

```css
/* applies to all HTML elements with class ="center" */
.center {
  text-align: center;
  color: red;
}
```

- to select specific HTML elements within a specific class, write: selector.class:

```css
p.center {
  text-align: center;
  color: red;
}
```

- refer to more than one class with an HTML element:

```html
<p class="center large">This paragraph refers to two classes.</p>
```
- NOTE: a class name cannot start with a number!

## The CSS Universal Selector

- the `universal selector` selects all HTML elements on the page:

```css
* {
  text-align: center;
  color: blue;
}
```

## The CSS Grouping Selector

- the `grouping selector` selects all the HTML elements with the same style definitions

Instead of:
```css
h1 {
  text-align: center;
  color: red;
}

h2 {
  text-align: center;
  color: red;
}

p {
  text-align: center;
  color: red;
}
```

Minimize the code with the `grouping selector`:

```css
h1, h2, p {
  text-align: center;
  color: red;
}
```



