---
title: "Sizing"
weight: 3
chapter: false
---

The images on our page are all enormous, so let's start by learning how to specify element sizes.

## Step 1

Add the following to your CSS:

```css {title="css"}
/* Your CSS here */
img {
	height: 200px;
}
```

The tag selector will get every `img` element.
The `height` property changes the height of an element by whatever value you provide - in this case, we've specified 100 pixels (`px`).


{{% notice style="warning" title="Test" icon="vial" %}}

Every image on the page should now have the same height.

{{% /notice %}}

Every image now has the same height, but if we have a look at our preview of the final product, we can see images of different sizes:

![Screenshot of completed webpage.](../../images/sized_images.png)

Instead of changing the height of all images at once, let's start at the top of the page and, working our way from top to bottom, resize each group of images.

## Step 2

If we take a look at the HTML, we can see that the first image is in the header.

Instead of setting the height of *every* image to `200px`, let's only set the height of the header image.

To do this, we can combine the header and image selectors, like so:

{{% notice style="warning" title="Before - Replace this code" %}}
```css
/* Your CSS here */
img {
	height: 200px;
}
```

{{% /notice %}}

{{% notice style="tip" title="After - Updated code" %}}
```css
/* Your CSS here */
header img {
	height: 200px;
}
```
{{% /notice %}}

We read this like: "select all the `img` tags that are in the `header` tag.

{{% notice style="warning" title="Test" icon="vial" %}}

Only the first image will be `200px` in height, and the rest will return to their default sizes.

{{% /notice %}}

## Step 3

The next couple of images are a bit different.
They all have rounded edges and have captions describing them. Notice how they're also aligned next to each other.

![](../../images/mood_board_pics.png)

Let's take a look at the HTML to see the structure of this part of the page:

```html {title="html"}
<section class="row" id="favourite_things">
	<div class = "grid-container"> <!-- Your images goes under here -->
		<h3>My favourite things</h3>
		<figure class="grid-item"> <!-- Your first image -->
			<a href="https://en.wikipedia.org/wiki/Turtle" target="_blank"> 
				<img src="https://assets.codepen.io/5804361/turtle_2.jpg" alt="A baby turtle on the beach" />
			</a>
			<figcaption>Save the Turtles</figcaption>
		</figure>

		<figure class="grid-item"> <!-- Your second image -->
			<img src="https://images.ctfassets.net/0zg5jftjwixq/2wqI4cgOUXecvmBiQ2v7pi/8f8f2a4ec1bca634ea15f587593f4ee7/NEW-Broome-Coast-WA-122782-56.jpg?w=1600" alt="We love Broome" />
			<figcaption>Broome ❤</figcaption>
		</figure>

		<figure class="grid-item">
			<img src="https://www.color-hex.com/palettes/8143.png" />
			<figcaption>Favourite Colour</figcaption>
		</figure>

		<figure class="grid-item">
			<img src="https://www.wildplanetblog.com/img/croatia-df4a3205.jpg" alt="Plitvice National Park Waterfalls" />
			<figcaption>Dream Holiday Location</figcaption>
		</figure>
		<!-- You can add more images to your grid view of images by repeating the process above -->
	</div>
</section>
```

Notice how these white boxes are all the same height?
Let's add some CSS for this.
From the HTML above we can see that each box is in a `div` with the class `card`.

Add a height to each of these cards:

{{% notice style="warning" title="Before - Add to this code" %}}
```css
#favourite_things div img {
	width: 200px;
}
```

{{% /notice %}}

{{% notice style="tip" title="After - Updated code" %}}
```css
#favourite_things div img {
	width: 200px;
}
.grid-item {
	height: 250px;
}
```
{{% /notice %}}

Well, that definitely did something, but it did not resize the images.

Add the following to your CSS to now resize the images:

{{% notice style="warning" title="Before - Replace this code" %}}
```css
.grid-item {
	height: 250px;
}
```

{{% /notice %}}

{{% notice style="tip" title="After - Updated code" %}}
```css
.grid-item {
	height: 250px;
}
.grid-item img {
	height: 40%;
}
```
{{% /notice %}}

{{% notice style="warning" title="Test" icon="vial" %}}

The images in the cards should now all be the same height.

{{% /notice %}}

The way we set the height of these images is a bit different to what we did previously.

Rather than specifying a value in pixels, we gave a percentage.
This CSS is saying "set the height of this element to be `40%` of the height of its parent (where **parent** means the element it is in, in this case, that is the card).

{{% notice tip %}}

This only works when the parent element has a specific size set.
Try removing `height: 250px` from the `.card` to see this for yourself!

{{% /notice %}}

## Step 4

So far we have just been setting the height, but we can actually set the width using the same format.
Let's modify our CSS to also set the width of the cards and their images.

{{% notice style="warning" title="Before - Replace this code" %}}
```css
.grid-item {
	height: 250px;  
}
.grid-item img {
	height: 40%;
}
```

{{% /notice %}}

{{% notice style="tip" title="After - Updated code" %}}
```css
.grid-item {
	height: 250px;
	width: 25%;   
}
.grid-item img {
	height: 40%;
	width: 100%;
}
```
{{% /notice %}}

{{% notice style="warning" title="Test" icon="vial" %}}

The images should now be as wide as the cards.

{{% /notice %}}

{{% notice tip %}}

Our cards aren't side by side like they are in the preview - don't worry! We'll get to that soon!

{{% /notice %}}

## Step 6

{{% notice style="info" title="Challenge!" icon="lightbulb" %}}

{{% /notice %}}

## Step 7

The last section is `favourite_quotes` and has multiple boxes with quotes (a reference to your work in part 3.1!.

Let's take a look at the structure of the HTML:

```html {title="html"}
<section class="row" id="favourite_quotes">
	<div id = "quotetile">
		<p>“Creativity takes courage.”</p>
	</div>
	<div class="first-row" id="box-1">
		<p>Box 1</p>
	</div>
	<div class="first-row" id="box-2">
		<p>Box 2</p>
	</div>
	<div class="second-row" id="box-3">
		<p>Box 3</p>
	</div>
	<div class="second-row" id="box-4">
		<p>Box 4</p>
	</div> 
</section>
```

Each of these images is in a `div` with the class `first-row` and `second-row`.
Eventually, these columns will be side by side, which means they need to be `50%` wide each in order to fit beside each other.

{{% notice style="info" title="Challenge!" icon="lightbulb" %}}

Set the `width` of the divs with the `column` class to `50%`.

{{% /notice %}}

We will then resize the images inside of these columns.

{{% notice style="info" title="Challenge!" icon="lightbulb" %}}

For images inside the divs with the `column` class: set their `height` to `200px` and their `width` to `80%`.

{{% /notice %}}

Here's what your page should look like at this stage:

![](../../images/mood_board_pics.png)


