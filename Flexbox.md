# Using Flexbox in CSS

![beach](https://images.unsplash.com/photo-1723444059774-743b0e6d19e9?q=80&w=3135&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)
Flexbox is a powerful layout system in CSS that allows you to easily align, distribute, and arrange items in a container. It’s useful for building responsive web designs. Here's a brief tutorial on how to use Flexbox.

## 1. Setting Up a Flex Container

To use Flexbox, you must define a container as a flex container using the `display: flex;` property.

```css
.container {
  display: flex;
}
```

- **`display: flex;`**: Enables Flexbox on the container.
- **Child elements (flex items)**: All direct children of the container will automatically become flex items.

*Example:*

```html
<div class="container">
  <div class="item">Item 1</div>
  <div class="item">Item 2</div>
  <div class="item">Item 3</div>
</div>
```

```css
.container {
  display: flex;
  background-color: lightgray;
}

.item {
  background-color: steelblue;
  color: white;
  padding: 20px;
  margin: 5px;
}
```

## 2. Controlling Flex Direction

By default, Flexbox arranges items in a row. You can control the direction using `flex-direction`.

```css
.container {
  display: flex;
  flex-direction: column; /* Change to row-reverse or column-reverse as needed */
}
```

### Common values:
- `row` (default): Items are placed in a horizontal row.
- `row-reverse`: Items are placed in reverse order.
- `column`: Items are placed in a vertical column.
- `column-reverse`: Items are placed in reverse vertical order.

## 3. Aligning Items with Justify Content

You can align items along the main axis using `justify-content`.

```css
.container {
  display: flex;
  justify-content: center;
}
```

### Common values:
- `flex-start` (default): Items align at the start.
- `flex-end`: Items align at the end.
- `center`: Items are centered.
- `space-between`: Items spread out with space between them.
- `space-around`: Items spread out with space around them.
- `space-evenly`: Equal spacing around all items.

## 4. Aligning Items with Align Items

You can align items along the cross axis using `align-items`.

```css
.container {
  display: flex;
  align-items: center;
}
```

### Common values:
- `stretch` (default): Items stretch to fill the container.
- `flex-start`: Items align at the start.
- `flex-end`: Items align at the end.
- `center`: Items align in the middle.
- `baseline`: Items align according to text baselines.

## 5. Controlling Item Sizing with Flex Grow, Shrink, and Basis

You can control how items grow, shrink, and start using `flex-grow`, `flex-shrink`, and `flex-basis`.

```css
.item {
  flex: 1; /* Equivalent to flex-grow: 1; flex-shrink: 1; flex-basis: 0; */
}
```

### Common properties:
- `flex-grow`: Determines how much an item can grow.
- `flex-shrink`: Determines how much an item can shrink.
- `flex-basis`: Defines the starting size of the item.

## 6. Wrapping Items

If items should wrap to a new row when the container is too small, use `flex-wrap`.

```css
.container {
  display: flex;
  flex-wrap: wrap;
}
```

### Common values:
- `nowrap` (default): Items stay in a single row.
- `wrap`: Items wrap onto new rows if necessary.
- `wrap-reverse`: Items wrap onto new rows in reverse order.

## 7. Aligning Multiple Lines with Align Content

When items wrap into multiple lines, you can use `align-content` to control their alignment.

```css
.container {
  display: flex;
  flex-wrap: wrap;
  align-content: center;
}
```

### Common values:
- `flex-start`: Lines align at the start.
- `flex-end`: Lines align at the end.
- `center`: Lines align in the middle.
- `space-between`: Lines are evenly distributed.
- `space-around`: Lines have equal space around them.
- `stretch`: Lines stretch to fill the container.

For more information on Flexbox, check out the [MDN Docs](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox).
```

