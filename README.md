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
