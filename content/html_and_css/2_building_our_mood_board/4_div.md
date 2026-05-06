---
title: "Div"
weight: 4
chapter: false
---

Great job, we've got a page with some content on it, some images and some links. But its a bit messy, we want to structure our content so it looks nice on our page. 


Unlike the `header` and `body` elements we used earlier, the `div` (divider) element does not inherently represent anything.
Instead, this element is used to group other elements.

Let's wrap our 5 images and quote in a `div` tag:

```html

<main>
  <div>
        <a href="https://en.wikipedia.org/wiki/Turtle" target="_blank"> 
            <img src="https://assets.codepen.io/5804361/turtle_2.jpg" alt="A baby turtle on the beach" />
        </a>
        <img src="https://www.brighteyedbaker.com/wp-content/uploads/2020/12/Chai-Latte-recipe-image.jpg" alt="Chai Latte in a Glass with spices surrounding" />
        <img src="https://www.foundanimals.org/wp-content/uploads/2023/02/twenty20_b4e89a76-af70-4567-b92a-9c3bbf335cb3.jpg" alt="Black Cat Lying Upside Dowwn Staring Adorably" />
        <img src="https://www.color-hex.com/palettes/6658.png" alt="Colour Palette Featuring Multiple Shades of Pink" />
        <img src="https://www.wildplanetblog.com/img/croatia-df4a3205.jpg" alt="Plitvice National Park Waterfalls" />
        <p>“Creativity takes courage.”</p>
</div>
</main>
```

Let's make a second `div` for our quote text, which we will use for styling purposes shortly.

## Check your Code

```html 

<head>
    <meta charset="UTF-8">
    <title>She Codes</title>
    <link rel="stylesheet" href="./styles.css">
</head>

<body>
    <!-- Your content goes here -->
    <header>
        <h1>Mood Board</h1>
        <p>A place for inspiration and creativity</p>
    </header>

    <main>
      <h2>2025</h2>
      <div>
        <a href="https://en.wikipedia.org/wiki/Turtle" target="_blank"> 
            <img src="https://assets.codepen.io/5804361/turtle_2.jpg" alt="A baby turtle on the beach" />
        </a>

        <img src="https://www.brighteyedbaker.com/wp-content/uploads/2020/12/Chai-Latte-recipe-image.jpg" alt="Chai Latte in a Glass with spices surrounding" />
        
        <img src="https://www.foundanimals.org/wp-content/uploads/2023/02/twenty20_b4e89a76-af70-4567-b92a-9c3bbf335cb3.jpg" alt="Black Cat Lying Upside Dowwn Staring Adorably" />
        
        <img src="https://www.color-hex.com/palettes/6658.png" alt="Colour Palette Featuring Multiple Shades of Pink" />
        
        <img src="https://www.wildplanetblog.com/img/croatia-df4a3205.jpg" alt="Plitvice National Park Waterfalls" />
      
        <div>
          <p>“Creativity takes courage.”</p>
        </div>
      </div>  
    </main>

    <footer>
        <p>Created with ❤️ by Your Name</p>
    </footer>

</body>

</html>
```


