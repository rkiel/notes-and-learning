# Pseudo

## Pseudo Class

[MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes)

- define style of a special state of an element

```css
.one {
  a:hover {
    color: white;
  }
  a:active {
    color: white;
  }
}
```

### not

- represents elements that do not match a list of selectors
- always better to use a positive case rather than the negative (i.e. performance, bugginess)

```css
:not(p) {
  color: blue;
}
```

## Pseudo Element

(MDN)[https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-elements]

- define style of a special part of an element

```css
.one {
  a::before {
    color: white;
  }
}
```
