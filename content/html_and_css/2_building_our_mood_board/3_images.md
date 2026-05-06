---
title: "Images"
weight: 3
chapter: false
---

All of the elements we have used so far have had an opening and a closing tag.

There are a few elements that are **self closing**.
For these tags, instead of having content between an open and close tag, they have content provided as an **attribute**.

![Annotated self closing HTML Element.](../../images/self_closing_element.png)

The image element is a self closing element, and has the tagname `img`.

We can use the following html to add an image to a webpage:

```html
<img src="link/to/image" alt="Sample Image 1"  />
```

The `src` attribute means **source** and it expects a URL to an image. `alt` is the alt text that will display if you can't load the image, and is also what screenreaders use for visually impaired folks to view your website. We are big fans of accessibility here, so make sure you've got helpful alt text on all your images.

Let's add in a few images to our `main`. It should now look like this:

```html
<main>
    <h2>2025</h2>
        <img src="https://assets.codepen.io/5804361/turtle_2.jpg" alt="A baby turtle on the beach" />
        <img src="https://www.brighteyedbaker.com/wp-content/uploads/2020/12/Chai-Latte-recipe-image.jpg" alt="Chai Latte in a Glass with spices surrounding" />
        <img src="https://www.foundanimals.org/wp-content/uploads/2023/02/twenty20_b4e89a76-af70-4567-b92a-9c3bbf335cb3.jpg" alt="Black Cat Lying Upside Dowwn Staring Adorably" />
        <img src="https://www.color-hex.com/palettes/6658.png" alt="Colour Palette Featuring Multiple Shades of Pink" />
        <img src="https://www.wildplanetblog.com/img/croatia-df4a3205.jpg" alt="Plitvice National Park Waterfalls" />
        <p>“Creativity takes courage.”</p>
</main>
```


{{% notice tip %}}

If you want to use a different image from the internet, you can right click on the image and copy it's URL (see the screenshot below).

{{% /notice %}}

![Screenshot of right click menu for image on Google Images.](../../images/image_link.png)

## Links

Now, we also might want to link the image (or text) to somwhere else.

To link to a page we use an **anchor** element, which has the tagname `a`.
The `a` tag has an `href` attribute which has a value of a URL.

Here's an example:

```html
<a href="https://en.wikipedia.org/wiki/Turtle">Read more about turtles here.</a>
```

The above HTML would render like so:

[Read more about turtles here.](https://en.wikipedia.org/wiki/Turtle)

We can also link from our images to other places on our website or external websites.

Let's add `a` tag before our image tag. 

```html
    <a href="https://en.wikipedia.org/wiki/Turtle"> 
            <img src="https://assets.codepen.io/5804361/turtle_2.jpg" alt="A baby turtle on the beach" />
    </a>
```

Notice here that our `img` is nestled inside of our opening `a` tag and closing `</a>` tag. 

{{% notice style="info" title="Challenge!" icon="lightbulb" %}}

Add at least one link to another website to your page. Play around with adding it to your images or perhaps one of your headings.

{{% /notice %}}

{{% notice tip %}}

When you click the link it takes us to that page in our CodePen window.
Instead, we could open that link in a new tab by adding `target="_blank"` to the `a` tag.
Try it!

{{% /notice %}}

## Check your code

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
        <a href="https://en.wikipedia.org/wiki/Turtle" target="_blank"> 
            <img src="https://assets.codepen.io/5804361/turtle_2.jpg" alt="A baby turtle on the beach" />
        </a>
        <img src="https://www.brighteyedbaker.com/wp-content/uploads/2020/12/Chai-Latte-recipe-image.jpg" alt="Chai Latte in a Glass with spices surrounding" />
        <img src="https://www.foundanimals.org/wp-content/uploads/2023/02/twenty20_b4e89a76-af70-4567-b92a-9c3bbf335cb3.jpg" alt="Black Cat Lying Upside Dowwn Staring Adorably" />
        <img src="https://www.color-hex.com/palettes/6658.png" alt="Colour Palette Featuring Multiple Shades of Pink" />
        <img src="https://www.wildplanetblog.com/img/croatia-df4a3205.jpg" alt="Plitvice National Park Waterfalls" />
        <p>“Creativity takes courage.”</p>
    </main>

    <footer>
        <p>Created with ❤️ by Your Name</p>
    </footer>

</body>

</html>

```