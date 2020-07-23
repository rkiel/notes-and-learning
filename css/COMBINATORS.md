# Combinators

## Adjacent Siblings (+)

- share the same parent and directly follow one another

```css
h2 + p {
  color: red;
}
```

```html
<div>
  <h2>Hello</h2>
  <p>World</p>
</div>
```

## General Siblings (~)

- share the same parent only

```css
h2 ~ p {
  color: red;
}
```

```html
<div>
  <h2>Hello</h2>
  <h3>to the</h3>
  <p>World</p>
</div>
```

## Child (>)

- second element is a direct child of the first

```css
div > p {
  color: red;
}
```

```html
<div>
  <p>Hello</p>
</div>
```

## Descendant ( )

- second element is a descendant of the first

```css
div p {
  color: red;
}
```

```html
<div>
  <section>
    <p>Hello</p>
  </section>
</div>
```
