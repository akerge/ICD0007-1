CSS Lab 2
====================

## Concepts to cover
* Display

* Positioning

* Overflow

* Transforms

* Transitions

* Animation

### Display

1. `Hide the <h1> element. It should still take up the same space as before.`

```html
<body>
<h1>This is a Heading</h1>
<p>This is a paragraph.</p>
<p>This is another paragraph.</p>
</body>
```

2. `Hide the <h1> element. It should not take up any space.`

```html
<h1>This is a Heading</h1>
<p>This is a paragraph.</p>
<p>This is another paragraph.</p>
```

3. `Display the list items as inline elements.`

```html
<body>
<h1>This is a Heading</h1>
<ul>
<li>Apple</li>
<li>Orange</li>
<li>Pear</li>
</ul>
</body>
```

4. `Display the <strong> elements as block elements.`

```html
<body>
<h1>This is a Heading</h1>
<p>This is a <strong>paragraph</strong>, with some words more <strong>important</strong> than others </p>
<p>This is another paragraph.</p>
</body>
```

### Position

1. `Position the <h1> element relative to the browser window. 50px from the top, and 50px from the right.`
```html
<head>
<style>
h1 {
    color: red;
}
</style>
</head>
<body>
<h1>This is a Heading</h1>
<p>This is a paragraph.</p>
<p>This is another paragraph.</p>
</body>
```

2. `Position the <h1> element 20px left, and 30px down, relative to its normal position.`

```html
<head>
<style>
h1 {
    color: red;
}
</style>
</head>
<body>
<h1>This is a Heading</h1>
<p>This is a paragraph.</p>
<p>This is another paragraph.</p>
</body>
```

3. `Position the <img> element behind the text.`

```html
<style>
img {
    position: absolute;
    left: 0px;
    top: 0px;
}
</style>
</head>
<body>
<h1>This is a Heading</h1>
<p>This is a paragraph.</p>
<p>This is another paragraph.</p>
<img src="put_any_image_here.png" width="100" height="140">
</body>
```

4. `Position the element with the "topleft" class 30px from the left, and 15px from the top, relative to its container.`

```html
<head>
<style>
.container {
    position: relative;
}

.topleft {
    font-size: 18px;
}

img {
    width: 100%;
    height: auto;
    opacity: 0.3;
}
</style>
</head>
<body>
<div class="container">
  <img src="put_image_here.jpg" alt="alt_name" width="1000" height="300">
  <div class="topleft">Top Left</div>
</div>
</body>
```

### Overflow

1. `Add a scrollbar to the <div> element.`

```html
<head>
<style>
div {
    background-color: #eee;
    width: 200px;
    height: 70px;
    border: 1px dotted black;
}
</style>
</head>
<body>
<div>
  <p>The Web is evolving rapidly. Front-end Web development has been majorly affected by recent changes in coding techniques and approaches.</p>
  <p>'In 2003, a competent front-end Web developer would have known HTML and CSS, possibly with a bit of copy-and-pasted JavaScript, and they built websites that would be viewed on desktop computers.'</p>
</div>
</body>
```

2. `Specify that the overflowing text in the <div> element should not be visible, not even with scrolling.`

```html
<head>
<style>
div {
    background-color: lightblue;
    width: 200px;
    height: 200px;
}
</style>
</head>
<body>
<div>Some text to hide overflow text. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus. Some text to hide overflow text. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus. Some text to hide overflow text. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus.</div>
</body>
```

3. `Add a horizontal scrollbar to <div>.`

```html
<head>
<style>
div {
    background-color: #eee;
    width: 150px;
    height: 70px;
    border: 1px dotted black;
    white-space: nowrap;
}
</style>
</head>
<body>

<div>
  <p>Some text to hide overflow text. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus. Some text to hide overflow text. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus. Some text to hide overflow text. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus.</p>
</div>
</body>
```
