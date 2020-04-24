# FLEXBOX FROGGY

##  🌸 justify-content: aligns flex-items along the main-axis (horizontally)
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

##  🌸 align-items: aligns flex-items along the cross-axis (vertically)
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

##  🌸 flex-direction: defines the direction of the main axis

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
  justify-content: flex-end; /* so if item has to be aligned on the left, you need to do flex-end, not flex-start */
}
```

`Notice that when the flex direction is a column, justify-content changes to the vertical and align-items to the horizontal.`

```css
#pond {
  display: flex;
  flex-direction: column;
  justify-content: flex-end; /* it will place items vertically in the bottom since flex-direction column is used */
}
```

##  🌸 order: Specifies the order of the flex item
Sometimes reversing the row or column order of a container is not enough. In these cases, we can apply the order property to individual items. By default, items have a value of 0, but we can use this property to also set it to a positive or negative integer value (-2, -1, 0, 1, 2).

Use the order property to reorder the frogs according to their lilypads.

```css
#pond { /* parent */
  display: flex;
}

.yellow { /* child item */
  order: 1
}
```

##  🌸 align-self: Aligns a flex item along the cross-axis, overriding the align-items value
This property accepts the same values as align-items and its value for the specific item
  - flex-start: Items align to the top of the container.
  - flex-end: Items align to the bottom of the container.
  - center: Items align at the vertical center of the container.
  - baseline: Items display at the baseline of the container.
  - stretch: Items are stretched to fit the container.
  
 ```css
 #pond {
  display: flex;
  align-items: flex-start;
}

.yellow {
  align-self: flex-end
}
```

Combine order with align-self to help the frogs to their destinations.

```css
#pond {
  display: flex;
  align-items: flex-start;
}

.yellow {
  align-self: flex-end;
  order: 1
}
```

##  🌸 flex-wrap: Specifies whether flex-items are forced on a single line or can be wrapped on multiple lines

Accepts the following values:
- nowrap: Every item is fit to a single line (default).
- wrap: Items wrap around to additional lines.
- wrap-reverse: Items wrap around to additional lines in reverse.

```css
#pond {
  display: flex;
  flex-wrap: wrap;
}
```

or

```css
#pond {
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
}
```

##  🌸 flex-flow: Shorthand property for `flex-direction` and `flex-wrap`
The two properties `flex-direction` and `flex-wrap` are used so often together that the shorthand property `flex-flow` was created to combine them. This shorthand property accepts the value of one of the two properties separated by a space.

For example, you can use `flex-flow: row wrap` to set rows and wrap them.

Try using flex-flow to repeat the previous level.

```css
#pond {
  display: flex;
  flex-flow: column wrap;
}
```

##  🌸 align-content: Aligns a flex container's line within the flex container when there is extra space on the cross-axis
The frogs are spread all over the pond, but the lilypads are bunched at the top. You can use align-content to set how multiple lines are spaced apart from each other. This property takes the following values:

- flex-start: Lines are packed at the top of the container.
- flex-end: Lines are packed at the bottom of the container.
- center: Lines are packed at the vertical center of the container.
- space-between: Lines display with equal spacing between them.
- space-around: Lines display with equal spacing around them.
- stretch: Lines are stretched to fit the container (default).

This can be confusing, but `align-content determines the spacing between lines, while align-items determines how the items as a whole are aligned within the container`. When there is only one line, align-content has no effect.

```css
#pond {
  display: flex;
  flex-wrap: wrap;
  align-content: flex-start;
}
```

Use a combination of flex-direction and align-content.

```css
#pond {
  display: flex;
  flex-wrap: wrap;
  flex-direction: column-reverse;
  align-content: center;
}
```

----------------------------------

Bring the frogs home one last time by using the CSS properties you've learned:

1. justify-content
2. align-items
3. flex-direction
4. order
5. align-self
6. flex-wrap
7. flex-flow
8. align-content


```css
#pond {
  display: flex;
  flex-flow: column-reverse wrap-reverse;
  align-content: space-between;
  justify-content: center;
}
```
