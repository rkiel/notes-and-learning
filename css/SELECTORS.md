# Selectors

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
```

## Id selector (#)

```css
#product-name {
  color: red;
}
```

## Attribute selector ([])

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
