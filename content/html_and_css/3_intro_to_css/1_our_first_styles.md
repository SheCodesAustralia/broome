---
title: "CSS Selectors"
weight: 1
chapter: false
---

There are two parts to CSS: selectors and declarations.
We'll just focus on selectors for now.
The selector tells the webpage which part of the page to apply the styles (declarations) to.

![Annotated CSS selector and declaration.](../../images/css_selector.png)

There are three different kinds of selectors:
- Tag
- ID
- Class

Take a look at the HTML provided to you.
You should notice that our `div` elements look a bit different to what we've seen before. They all have **classes** and **ids**:

```html {title="html"}
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
```

We'll use type, class and ID selectors to change the colour of different elements on the page.

## Type Selectors

First, let's change the colour of the text.
We can use a **type selector** to do this.
By referencing the `p` tag, we can change the colour of all text in a `p` tag.
Add the following to your css:

{{% notice style="warning" title="Before - Add to this code" %}}
```css
/* Your CSS here */

body {
	background-color: #8246af;
}
```
{{% /notice %}}

{{% notice style="tip" title="After - Updated code" %}}
```css
/* Your CSS here */

body {
	background-color: #8246af;
}
p {
	color: #ffa300;
}
```
{{% /notice %}}
The text should now be She Code's shade of orange.

## ID Selectors

Each box has a unique `id`, which means that we can reference each box individually.

Let's try changing the background colour of `box-1` only:

{{% notice style="warning" title="Before - Add to this code" %}}
```css
/* Your CSS here */

body {
	background-color: #8246af;
}
p {
	color: #ffa300;
}
```
{{% /notice %}}

{{% notice style="tip" title="After - Updated code" %}}
```css
/* Your CSS here */

body {
	background-color: #8246af;
}
p {
	color: #ffa300;
}

#box-1 {
	background-color: #be9fd5;
}
```
{{% /notice %}}


The top left box should now be another shade of purple.


{{% notice style="note" title="Note" %}}

Notice that we used a `#` before `box-1`, which tells our CSS that we are looking for an ID.

{{% /notice %}}

## Class Selectors

The top two boxes have the `first-row` class, and the bottom two boxes have the `bottom-row` class.
This means that we could use these classes to reference each row individually, i.e. two boxes at a time.

Let's try changing the background colour of the two boxes in the bottom row:

{{% notice style="warning" title="Before - Add to this code" %}}
```css
/* Your CSS here */

body {
	background-color: #8246af;
}
p {
	color: #ffa300;
}

#box-1 {
	background-color: #be9fd5;
}
```
{{% /notice %}}

{{% notice style="tip" title="After - Updated code" %}}
```css
/* Your CSS here */

body {
	background-color: #8246af;
}
p {
	color: #ffa300;
}

#box-1 {
	background-color: #be9fd5;
}
.second-row {
	background-color: #ffffff;
}
```
{{% /notice %}}

The bottom boxes should now be white.

{{% notice style="note" title="Note" %}}

Notice that we used a `.` before `second-row`, which tells our CSS that we are looking for a class.

{{% /notice %}}

This should be the final result:

![](../../images/boxes_complete.png)

{{% notice style="info" title="Challenge!" icon="lightbulb" %}}

Try changing the background colour of box 2 only.

{{% /notice %}}
