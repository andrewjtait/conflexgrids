# ConsistentFlexibleGrids

A simple stylesheet using Sass to generate a flexible grid with consistent margins.

Set any margin you want to use, and the columns in the grid will flex to the size of the browser or parent element while always retaining the same margin between columns.

## Example

[View a demo](http://www.andrewjamestait.co.uk/conflexgrids/).

## How to use it

### Configuring the Sass file

To include the CSS, import the conflexgrids SCSS file into your Sass stylesheet:

```scss
@import "/sass/conflexgrids";
```

You can configure the margin size by setting the `$grid-margin` value (defaults to `20px`).

You can configure the max number of columns you can use by setting the `$max-columns` value (defaults to `12`).

### Constructing a grid in your HTML

You can construct rows and columns with some simple HTML:

```html
<div class="row column-2">
  <div class="column">...</div>
  <div class="column">...</div>
</div>
```

#### Span columns

A column can span the width of multiple columns with an additional class:

```html
<div class="row column-4">
  <div class="column span-2">...</div>
  <div class="column">...</div>
  <div class="column">...</div>
</div>
```

#### Offset columns

A column can be offset (skipping a number of columns) with an additional class:

```html
<div class="row column-6">
  <div class="column offset-4">...</div>
  <div class="column">...</div>
</div>
```
