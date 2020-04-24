# FLEXBOX FROGGY

##  🌸 justify-content: aligns items horizontally
Guide the frog to the lilypad on the right by using the `justify-content` property, which `aligns items horizontally` and accepts the following values:

- flex-start: Items align to the left side of the container. It's default.
- flex-end: Items align to the right side of the container.
- center: Items align at the center of the container.
- space-between: Items display with equal spacing between them.
- space-around: Items display with equal spacing around them.

For example, justify-content: flex-end; will move the frog to the right. 

```css
#pond {
  display: flex;
  justify-content: flex-end;
}
```

##  🌸 align-items: aligns items vertically
Now use align-items to help the frogs get to the bottom of the pond. This CSS property aligns items vertically and accepts the following values:

- flex-start: Items align to the top of the container.
- flex-end: Items align to the bottom of the container.
- center: Items align at the vertical center of the container.
- baseline: Items display at the baseline of the container.
- stretch: Items are stretched to fit the container.

```css
#pond {
  display: flex;
  align-items: flex-end;
}
```

Lead the frog to the center of the pond using a combination of justify-content and align-items.
`Center the item horizontally and vetically!`

```css
#pond {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

##  🌸 flex-direction: defines the direction items are placed in the container

The frogs need to get in the same order as their lilypads using flex-direction. This CSS property defines the direction items are placed in the container, and accepts the following values:

- row: Items are placed the same as the text direction (left to right).
- row-reverse: Items are placed opposite to the text direction (right to left).
- column: Items are placed top to bottom.
- column-reverse: Items are placed bottom to top.

```css
#pond {
  display: flex;
  flex-direction: row-reverse;
}
```

`When items take both flex-direction and justify-content to get aligned, notice that when you set the direction to a reversed row or column, start and end are also reversed.`

```css
#pond {
  display: flex;
  flex-direction: row-reverse;
  justify-content: flex-end; // so if item has to be aligned on the left, you need to do flex-end, not flex-start
}
```

`Notice that when the flex direction is a column, justify-content changes to the vertical and align-items to the horizontal.`

```css
#pond {
  display: flex;
  flex-direction: column;
  justify-content: flex-end; // it will place items vertically in the bottom since flex-direction column is used
}
```
