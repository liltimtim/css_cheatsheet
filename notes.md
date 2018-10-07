# CSS

What is `CSS`?

- cascading stylesheets
- **not** a programming language
- stylesheet / styling language
- used for website layout and design
- can be extended with sass / less

### Ways of adding CSS

1. inline css: directly in the html element (this is bad practice but supported)
2. internal css: using `<style>` tags within a single document
3. External CSS: linking an external .css file

**Internal CSS** is better than inline CSS but is not the suggested method. This CSS is not reusable and fattens up the HTML

**External CSS** is the preferred and best practice method. CSS is reusable.

### Example of Inline

```html
<body>
  <!-- This is NOT the recommended way -->
  <!-- <h1 style="color:red">Hello World</h1> -->
</body>
```

### Example of Internal cSS

```html
  <style type="text/css">
    h1 {
      color: blue
    }
  </style>
```

---

## CSS Selectors

Basic structure of a CSS `Selector`
a { background-color: yellow; }

a: selector
property: `background-color:`
value: `yellow`

## Colors in CSS

1. Color names
2. HTML5 color names
3. Hexadecimal
4. RGB

```css
body {
  color: red;
  background: coral;
}

h1 {
  color: #00ff00;
}

p {
  color: rgb(0, 0, 255);
}
```

# ID vs. Class

ID: Unique identifier
Class: similar too an ID but its not unique

Generally speaking, the convention is that a `class` is used with styling but an `id` is used for identifying a unique HTML element.

ID = unique; class = reusable

# Class

Targetting a class is done with the following syntax

```html
<div class="box-1"></div>
```

```css
.box-1 {
  background-color: #333;
}
```

To target a class, the syntax `.<class_name>` is used.

**margin**: is the `spacing` in between two elements

```css
h1 {
  margin: auto;
}
```

The example above places an automatic margin around an element. This is generally found in `containers`.

### Responsive design

Using percentages when dealing with container type objects.

### Box Model

CSS content is whatever the element is

There are 3 layers

1. padding (space between content and border)
2. border (space between padding and margin)
3. margin (space between border and outside)

### Targetting States of an Element

```css
a {
  text-decoration: none;
  color: #000;
}
/* targets links hover state */
a:hover {
  color: red;
}

a:visited {
  color: yellow;
}
```

# Positioning in CSS

**static**: default pos, renders in order of doc flow
**relative**: pos relative to normal position
**absolute**: target position inside a relative element
**fixed**: fixed position to the browser window
**initial**: sets default value
**inherit**: inherits from the parent
