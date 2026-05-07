---
title: "Fonts"
weight: 7

chapter: false
---

There are a lot of different things we can do with fonts, including changing their family and size.

## Family

Head over to [Google Fonts](https://fonts.google.com/) and pick out a font that you like.

Select that font then view all your selected fonts:

![Screenshot of Google Font.](../../images/fonts_1.png)

Select the `@import` option:

![Screenshot of how to use Google Font](../../images/fonts_2.png)

Copy the code **between the `<style>` tags**.

Paste this code at the **top of your css file**.

```css {title="css"}

/* Your fonts here */
@import url('https://fonts.googleapis.com/css2?family=Pacifico&display=swap');
/* */
```
If you've noticed in our template, we've actually been making you use She Code's signature font Raleway - but of course you're free to change that since you have the power to now <3

Then head back to Google Fonts and copy the `font-family` line of code.

Let's style our headings with your selected font:

```css {title="css"}
/* Your CSS here */

h1 {
	font-family: 'Pacifico', cursive;
}

h2 {
	font-family: 'Pacifico', cursive;
}

h3 {
	font-family: 'Pacifico', cursive;
}
```

{{% notice style="info" title="Challenge!" icon="lightbulb" %}}

Find another font to use for the nav, footer and paragraphs.

{{% /notice %}}

## Size

Let's try changing the size of our text too.

Add the following to your CSS:

{{% notice style="warning" title="Before - Replace this code" %}}
```css
/* Your CSS here */

h1 {
	font-family: 'Pacifico', cursive;

}
```

{{% /notice %}}

{{% notice style="tip" title="After - Updated code" %}}
```css
/* Your CSS here */

h1 {
	font-family: 'Pacifico', cursive;
    font-size: 50px;
}
```
{{% /notice %}}

{{% notice style="info" title="Challenge!" icon="lightbulb" %}}

Change the font size of the `h2`, `h3`, and `p` tags.

{{% /notice %}}

## Colour

We can change the color of our fonts using the `color` attribute.

Add the following to your CSS:

```css {title="css"}
/* Your CSS here */

a {
	color: #ffa300;
}
```

{{% notice style="warning" title="Test" icon="vial" %}}

The colour of the `a` (link) tags in the `nav` should turn orange.

{{% /notice %}}

{{% notice style="info" title="Challenge!" icon="lightbulb" %}}

Change the colour of the `h1`, `h2` and `h3` headings.

{{% /notice %}}

Here's what your page could look like so far (using your own fonts). The following example uses Bebas Neue instead of Raleway:
{{% notice style="tip" title="Fun Fact" icon="lightbulb" %}}
This was She Code's old font.
Kate, please don't hate me <3
- Editor note
{{% /notice %}}
![](../../images/kate_fave_font.png)

