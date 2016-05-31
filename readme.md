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
```

<!-- <!DOCTYPE html>
<html lang="en">
  <head>
    <title>Title</title>
    <link rel="stylesheet" type="text/css" href="style.css">
  </head>
  <body>
    <h1>This is the HEADER</h1>
    <nav>
      <ul>
        <li>Link 1</li>
        <li>Link 2</li>
        <li>Link 3</li>
        <li>Link 4</li>
      </ul>
    </nav>
    <div>This is a DIV</div>
    <footer>This is a footer</footer>
    </body>
</html> -->

2.) What are the differences between these tags?

```html
<!-- Tag 1 -->
<img src="images/me.jpg" alt="My profile image"> 
<!-- This is an image -->

<!-- Tag 2 -->
<div></div>
<!-- This is a div -->
```

```
Explain here.
```
The first one is an image, the second is a div

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
```

  Inline Styles are the most specific, they override the rest
  Internal Style Sheets are usually used if you have just one HTML page that has a different style from the rest
  External Style Sheets should be used most, this way all the css can link to multiple pages, easier to edit css
  If there is a property defined twice on the same element either within a css style sheet or if there is an external and internal style sheet loaded, the last listing is the one that will take precidence

2.) Below are some different CSS selectors. Use CSS comments to describe what each selector will do.

```css
/* comment like this */
div {
  border-radius: 50%;
}

/* will giv all divs rounded cornered borders with a radius of 50% */

.header p {
  font-size: 18px;
}

/* all paragraphs that are children of an element with the class "header" will have a font of 18px */

.footer {
  position: absolute;
  bottom: 0;
}

/*any element with a class of "footer" will be absolutely positioned to the bottom of it's closest positioned ancestor or the containing block, margins do not collapse, does not leave sqace for it for where it would have been */

.splash-image {
  background-image: url("../images/ocean.jpg");
  background-size: cover;
  width: 100%;
}

/* any element with the class "splash-image" will have an image of the ocean, the size will be to cover the element, and the width will be 100% of it's container */

.ninja:hover {
  display: none;
  color: black;
}

/* when any element with a class of "ninja" is hovered over, it will disappear and the font will turn black */
```