# Properties

## Display

- block - rendered as a block and take up all available horizontal space
- inline - rendered to take up only the space they require
  - don't use top & bottom margin
  - top & bottom padding have different effects
  - width & height have no effect
- inline-block - behave like inline but allow for top & bottom margin/padding
  - be careful of the white space in you file
- none - not visible and not in the document flow but in the DOM
- hidden - not visible but in the document flow and in the DOM

## Text

```css
.one {
  text-decoration: underline;
}
.two {
  text-decoration: none;
}
```

## Vertical

```css
.one {
  vertical-align: middel;
}
```

## Width & Height

- block-level elements use `width: 100%` by default
- height is relative to the available height in the parent container
- never includes margin

```css
.one {
  width: 100%;
  height: 528px;
  padding: 10px;
  border: 5px solid orange
  margin: 10px;
  box-sizing: content-box; /* does not include padding & border */
}
.two {
  width: 100%;
  height: 528px;
  padding: 10px;
  border: 5px solid orange
  margin: 10px;
  box-sizing: border-box; /* does include padding & border */
}
* {
  box-sizing: border-box; /* a good default */
}
```

## Short Hand

### Border - order does not matter

```css
.one {
  border-width: 2px;
  border-style: solid;
  border-color: orange;
}
.two {
  border: 2px solid orange;
}
.three {
  border-top-width: 2px;
  border-top-style: solid;
  border-top-color: orange;
  border-bottom-width: 2px;
  border-bottom-style: solid;
  border-bottom-color: orange;
}
```

### Background - order does not matter

```css
.one {
  background-color: orange;
}
.two {
  background: orange;
}
```

### Marging & Padding - order matters

```css
.one {
  margin-top: 5px;
  margin-right: 10px;
  margin-bottom: 15px;
  margin-left: 20px;
}
.two {
  marging: 5px 10px 15px 20px; /* top right bottom left */
}
.three {
  marging: 5px 10px; /* top&bottom left&right */
}
.four {
  marging: 10px;
}
```
