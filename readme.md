#Humble Grid

Humble is a lightweight, Flexbox based grid system built with Sass. Humble does not apply gutters in the form of margins or padding. Humble is humble.


##Rows and Columns
Just like grids in Foundation or Bootstrap, Humble focuses on rows and columns. By default, Humble allows for 12 columns per row. This can be overridden using the `$number_of_columns` variable. Set to any number you like.


###Breakpoints
Out of the box, Humble supports 5 Breakpoints: `xs`, `sm`, `md`, `lg`, and `xl`:

```scss
$breakpoints: (
  xs: (
    high: 30rem,
  ),
  sm: (
    low: 30.0625rem,
    high: 40rem,
  ),
  md: (
    low: 40.0625rem,
    high: 64rem,
  ),
  lg: (
    low: 64.0625rem,
    high: 90rem,
  ),
  xl: (
    low: 90.0625rem
  )
);
```

These values can be changed by completely overriding the `$breakpoints` map, or by merging two maps together.

###Orientation
Unlike other grid systems, Humble include modifiers for targeting device orientation. Example

```html
<div class="col-sm-6">50% Width for Small and Up</div>
<div class="col-sm-p-3">25% Width for Small and Up (portrait only)</div>
<div class="col-sm-l-12">100% Width for Small and Up (landscape only)</div>
```
