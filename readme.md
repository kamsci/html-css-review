# HTML/CSS Review

This is a review of your working knowledge of HTML and CSS. Note that this review is designed to help you recall and familiarize yourself with technical concepts.

## Getting Started

* Fork and clone this repository
* Answer the following questions by...
  * Opening this file in Sublime
  * Answering the questions via Markdown. Feel free to refer to this [Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* Commit your changes
* Make a pull request for submission

---

## HTML

1.) Create a valid, empty HTML page with the necessary tags.

```html
<!-- Code goes here -->
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" type="text/css" href="">
    <meta charset="utf-8">
    <title></title>
  </head>
  <body>
    <h1></h1>
    <script type="text/javascript"></script>
  </body>
</html>
```

2.) What are the differences between these tags?

```html
<!-- Tag 1 -->
<img src="images/me.jpg" alt="My profile image">

<!-- Tag 2 -->
<div></div>
```

```
Explain here.
```
  img is a void element, you typically don't next inside of it. It will put the image to the div or location you are in. 
  div will always have an opening and closing tag. div does not add content, but creates containers for content to be placed into.. divisios.
---

## CSS

1.) Compare and contrast the following ways to add CSS to HTML elements.

```html
<!-- Inline CSS -->
<div style="background-color: red;"></div>

<!-- Internal style sheet -->
<style type="text/css">
  div {
    background-color: red;
  }
</style>

<!-- External style sheet (not shown) -->
<link rel="stylesheet" type="text/css" href="css/style.css">
```

```
Explain here
  Inline CSS is quick and dirty css styling directing in your html code. it is not recomended, it can get complex and you might want to use a different style sheet in the future, like boostrap etc. All html code will trump anything you have in a css stylesheet. 

  Internal stylesheet is separated from the html code, however, it is in the same file as your html. also not recommended

  Exteral style sheet is it's own .css file that is referenced in the html file. Recommended way to ass style guides. you can add more than 1 style guide to reference. 
```

2.) Below are some different CSS selectors. Use CSS comments to describe what each selector will do.

```css
/* comment like this */
div {
  border-radius: 50%;
}
/* alters the boarder around an object, if the object is square, 50% will make it a circle. */

.header p {
  font-size: 18px;
}
/* changes font size of the paragraph in the header class only */

.footer {
  position: absolute;
  bottom: 0;
}
/* positions your footer absolutely to the parent element that should have position relative. This ignores the standard layout and allows you to place certain content above or below other content */

.splash-image {
  background-image: url("../images/ocean.jpg");
  background-size: cover;
  width: 100%;
}

/* adds a picture as a background to the class 'splash-image'. the picture will cover the background once instead of repeating, and it's widthe is 100% of the container*/

.ninja:hover {
  display: none;
  color: black;
}

/* adds the hover css  style to the ninja class so when you hover over the container, the color turns black when hovering and the dispaly is none*/
```

