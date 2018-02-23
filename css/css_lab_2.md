CSS Lab 2
====================

Instructions
====================

* You should create a repository, add me as collaborator from tab `Settings`. My Github username is `sunnepah`

* For each of the section below, you should create a separate folder and put your work inside

* Once you are done with any section, you should `commit and push the code to the remote repository` - A single commit for everything at once is not ALLOWED.

## Concepts to cover
* Display

* Positioning

* Overflow

* Transforms

* Transitions

* Animation

Display
====================

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

![Alt text](https://github.com/ICD0007/ICD0007/blob/master/css/breadcrumb_image.png "Optional title")

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

Position
====================

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

Overflow
====================

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

Responsiveness
====================

1. Make the web page responsive using the html content below

Expected result

![Alt text](https://github.com/ICD0007/ICD0007/blob/master/css/Responsiveness.png "Optional title")

```html
<html>
<head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        * {
            box-sizing: border-box;
        }

        .row::after {
            content: "";
            clear: both;
            display: table;
        }

        [class*="col-"] {
            float: left;
            padding: 15px;
        }

        .col-1 {
            width: 8.33%;
        }

        .col-2 {
            width: 16.66%;
        }

        .col-3 {
            width: 25%;
        }

        .col-4 {
            width: 33.33%;
        }

        .col-5 {
            width: 41.66%;
        }

        .col-6 {
            width: 50%;
        }

        .col-7 {
            width: 58.33%;
        }

        .col-8 {
            width: 66.66%;
        }

        .col-9 {
            width: 75%;
        }

        .col-10 {
            width: 83.33%;
        }

        .col-11 {
            width: 91.66%;
        }

        .col-12 {
            width: 100%;
        }

        html {
            font-family: "Lucida Sans", sans-serif;
        }

        .header {
            background-color: #9933cc;
            color: #ffffff;
            padding: 15px;
        }

        .menu ul {
            list-style-type: none;
            margin: 0;
            padding: 0;
        }

        .menu li {
            padding: 8px;
            margin-bottom: 7px;
            background-color: #33b5e5;
            color: #ffffff;
            box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12), 0 1px 2px rgba(0, 0, 0, 0.24);
        }

        .menu li:hover {
            background-color: #0099cc;
        }
    </style>
</head>

<body>

    <div class="header">
        <h1>ICD0007</h1>
    </div>

    <div class="row">
        <div class="">

        </div>
        <div class="">
            <h1>ICD0007</h1>
            <p>The goal of the course is to give an overview of web based information systems development and standards. The
                course provides foundation for next level web development courses.
            </p>
            <p>
                Student knows how to create HTML pages Student knows how to style HTML pages with CSS Student knows how to use Javascript
                Student knows how to use PHP Student knows how to write MySQL queries and make use of them in the PHP application
                Student knows how to read and explain HTML, CSS, JS, PHP code and MySQL queries
            </p>
            <p style="color: red;"><strong>Resize the browser window to see how the content respond to the resizing.</strong></p>
        </div>

        <div class="menu">
            <ul>
                <li>Group 1</li>
                <li>Group 2</li>
                <li>Group 3</li>
                <li>Group 4</li>
            </ul>
        </div>
    </div>
</body>
</html>
```

Transforms
====================

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

Transitions
====================

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

Animations
====================

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
