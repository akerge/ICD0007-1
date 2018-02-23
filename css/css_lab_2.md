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

5. `Add css styling to the html content to look same as the image below`

```html
<html>
<head>
<style>
</style>
</head>
<body>
<h2>Breadcrumb</h2>
<ul class="breadcrumb">
  <li><a href="#">Home</a></li>
  <li><a href="#">Courses</a></li>
  <li><a href="#">ICD0007</a></li>
  <li>CSS 2</li>
</ul>
</body>
</html>
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

### Transforms

1. `With the transform property, rotate the <div> element 150deg around its X-axis.`

```html
<style> 
div {
    width: 100px;
    height: 100px;
    background-color: lightblue;
    border: 1px solid black;
}
</style>
</head>
<body>
<div>This is a div element</div>
</body>
```

2. `With the transform property, rotate the <div> element 90deg around its Z-axis`

```html
<head>
<style> 
div {
    width: 100px;
    height: 100px;
    background-color: lightblue;
    border: 1px solid black;
}
</style>
</head>
<body>
<div>This is a div element</div>
</body>
```

### Transitions

1. `Add a 2 second transition effect for width changes of the <div> element and should have a "0.5" second delay before starting.`

```html
<head>
<style> 
div {
    width: 100px;
    height: 100px;
    background: red;
}

div:hover {
    width: 300px;
}
</style>
</head>
<body>
<div></div>
<p>Hover over the div element above.</p>
</body>
```

### Animations

1. `Given the animation code below, the flying objects collides, can you make sure there is no collision? Also, you should make element "example3" to alternate direction`

```html
<html>
<head>
    <title>Flying Objects</title>
    <link href="style.css" rel="stylesheet">
</head>
<style>
    /* The animation code */
@keyframes example1 {
  from {
    background-color: red;
  }
  to {
    background-color: yellow;
  }
}

/* The element to apply the animation to */
.example1 {
  width: 100px;
  height: 100px;
  background-color: red;
  animation-name: example1;
  animation-duration: 4s;
}

/* The animation code */
@keyframes example2 {
  0% {
    background-color: red;
  }
  25% {
    background-color: yellow;
  }
  50% {
    background-color: blue;
  }
  100% {
    background-color: green;
  }
}

/* The element to apply the animation to */
.example2 {
  width: 100px;
  height: 100px;
  background-color: red;
  animation-name: example2;
  animation-duration: 4s;
}

/* The animation code */
@keyframes example3 {
  0% {
    background-color: red;
    left: 0px;
    top: 0px;
  }
  25% {
    background-color: yellow;
    left: 200px;
    top: 0px;
  }
  50% {
    background-color: blue;
    left: 200px;
    top: 200px;
  }
  75% {
    background-color: green;
    left: 0px;
    top: 200px;
  }
  100% {
    background-color: red;
    left: 0px;
    top: 0px;
  }
}

/* The element to apply the animation to */
.example3 {
  width: 100px;
  height: 100px;
  position: relative;
  background-color: red;
  animation-name: example3;
  animation-duration: 4s;
  animation-iteration-count: infinite;
}

#animated_div {
  width: 100px;
  height: 47px;
  background: #92b901;
  color: #ffffff;
  position: relative;
  font-weight: bold;
  font-size: 20px;
  padding: 10px;
  animation: animated_div 5s 1;
  animation-iteration-count: infinite;
  /* animation-direction: reverse; */
  -moz-animation: animated_div 5s 1;
  -webkit-animation: animated_div 5s 1;
  -o-animation: animated_div 5s 1;
  border-radius: 5px;
  -webkit-border-radius: 5px;
  animation-iteration-count: infinite;
}

@keyframes animated_div {
  0% {
    transform: rotate(0deg);
    left: 0px;
  }

  25% {
    transform: rotate(20deg);
    left: 0px;
  }
  50% {
    transform: rotate(0deg);
    left: 500px;
  }
  55% {
    transform: rotate(0deg);
    left: 500px;
  }
  70% {
    transform: rotate(0deg);
    left: 500px;
    background: #1ec7e6;
  }
  100% {
    transform: rotate(-360deg);
    left: 0px;
  }
}

.example4 {
  width: 100px;
  height: 100px;
  background-color: red;
  position: relative;
  -webkit-animation-name: example4; /* Safari 4.0 - 8.0 */
  -webkit-animation-duration: 4s; /* Safari 4.0 - 8.0 */
  -webkit-animation-delay: 2s; /* Safari 4.0 - 8.0 */
  animation-name: example4;
  animation-duration: 4s;
  animation-delay: 2s;
  animation-iteration-count: infinite;
}

/* Safari 4.0 - 8.0 */
@-webkit-keyframes example4 {
  0%   {background-color:red; left:0px; top:0px;}
  25%  {background-color:yellow; left:200px; top:0px;}
  50%  {background-color:blue; left:200px; top:200px;}
  75%  {background-color:green; left:0px; top:200px;}
  100% {background-color:red; left:0px; top:0px;}
}

/* Standard syntax */
@keyframes example4 {
  0%   {background-color:red; left:0px; top:0px;}
  25%  {background-color:yellow; left:200px; top:0px;}
  50%  {background-color:blue; left:200px; top:200px;}
  75%  {background-color:green; left:0px; top:200px;}
  100% {background-color:red; left:0px; top:0px;}
}

</style>
<body>
    <p>
        <b>Note:</b> This example does not work in Internet Explorer 9 and earlier versions.
    </p>
    <div class="example1">example1</div>
    <p>
        <b>Note:</b> When an animation is finished, it changes back to its original style.</p>

    <div class="example2">example2</div>
    <br>
    <div class="example3">example3</div>

    <br>
    <div class="example4">Animation with delays</div>

    <br>
    <div id="animated_div">I'm just flying here.</div>
</body>
</html>
```
