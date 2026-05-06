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
    <h2>She Codes by the Beach 2026</h2>
    <a href="https://en.wikipedia.org/wiki/Turtle"> 
      <img src="https://assets.codepen.io/5804361/turtle_2.jpg" alt="A baby turtle on the beach"/>
    </a>
    <img src="https://images.ctfassets.net/0zg5jftjwixq/2wqI4cgOUXecvmBiQ2v7pi/8f8f2a4ec1bca634ea15f587593f4ee7/NEW-Broome-Coast-WA-122782-56.jpg?w=1600" alt="We love Broome"/>
    <img src="https://www.foundanimals.org/wp-content/uploads/2023/02/twenty20_b4e89a76-af70-4567-b92a-9c3bbf335cb3.jpg" alt="Black Cat Lying Upside Dowwn Staring Adorably"/>
    <img src="https://www.color-hex.com/palettes/8143.png" alt="Colour Palette Featuring Orange and Purple"/>

    <p>“Creativity takes courage.”</p>
  </div>
</main>
```

Let's make a second `div` for our quote text, which we will use for styling purposes shortly.

## Check your Code

```html 
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>She Codes</title>
  <link rel="stylesheet" href="./styles.css">
</head>

<body> <!-- Your content goes under here -->
  <header>
    <h1>Mood Board</h1>
    <p>A place for inspiration and creativity</p>
  </header>

  <main>
    <div>
      <h2>She Codes by the Beach 2026</h2>
      <a href="https://en.wikipedia.org/wiki/Turtle"> 
        <img src="https://assets.codepen.io/5804361/turtle_2.jpg" alt="A baby turtle on the beach"/>
      </a>
      <img src="https://images.ctfassets.net/0zg5jftjwixq/2wqI4cgOUXecvmBiQ2v7pi/8f8f2a4ec1bca634ea15f587593f4ee7/NEW-Broome-Coast-WA-122782-56.jpg?w=1600" alt="We love Broome"/>
      <img src="https://www.foundanimals.org/wp-content/uploads/2023/02/twenty20_b4e89a76-af70-4567-b92a-9c3bbf335cb3.jpg" alt="Black Cat Lying Upside Dowwn Staring Adorably"/>
      <img src="https://www.color-hex.com/palettes/8143.png" alt="Colour Palette Featuring Orange and Purple"/>

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


