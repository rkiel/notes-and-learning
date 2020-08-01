# Selectors

[MDN](https://developer.mozilla.org/en-US/docs/Web/CSS)
[Can I use?](https://caniuse.com/)

## Tag / Element selector

```css
h1 {
  color: red;
}
```

## Class selector (.)

```css
.heading {
  color: red;
}
a.active {
  color: red;
}
a:not(.active) {
  color: blue;
}
```

```html
<a class="active" />
```

## Id selector (#)

```css
#product-name {
  color: red;
}
```

## Attribute selector ([ ])

```css
input[type="text"] {
  color: red;
}
```

## Universal (\*)

```css
* {
  color: red;
}
```

## Priority

1. inline styles
1. \#id selectors
1. .class, :pseudo-class, [attribute]
1. \<tag>, :pseudo-element
1. inherited styles

## Class vs Id

- Class selectors are re-usable
- Class selectors allow you to make/name things for styling purposes only
- Class selectors should be your go-to selector
- Id selectors used only once per page
- Id also has a non-CSS meaning (e.g. on-page link)
- Id should not be used ONLY to add some style

## !important

- overwrites specificity and all other selectors
- in general, do NOT use !important

```css
div {
  color: red !important;
}
```
