# Class 5 - Reading Notes

## What is CSS

CSS is a language for specifying how documents are presented to users how they are styled, laid out, etc.
A document is usually a text file structured using a markup language.
Presenting a document to a user means converting it into a form usable by your audience.

```
h1 {
  color: red;
  font-size: 5em;
}
```

```
h1 {
  color: red;
  font-size: 5em;
}

p {
  color: black;
}
```

As there are so many things that you could style using CSS, the language is broken down into modules.d

All web standards technologies (HTML, CSS, JavaScript, etc.) are defined in giant documents called specifications (or "specs"), which are published by standards organizations (such as the W3C, WHATWG, ECMA, or Khronos) and define precisely how those technologies are supposed to behave.

## How to add CSS

With an external style sheet, you can change the look of an entire website by changing just one file. Each HTML page must include a reference to the external style sheet file inside the <link> element, inside the head section.

```
External styles are defined within the <link> element, inside the <head> section of an HTML page:

<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

"mystyle.css"
```
body {
  background-color: lightblue;
}

h1 {
  color: navy;
  margin-left: 20px;
}
```

An ****internal style** sheet may be used if one single HTML page has a unique style.

The internal style is defined inside the <style> element, inside the head section.

Internal styles are defined within the <style> element, inside the <head> section of an HTML page:

```
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

An ****inline style** may be used to apply a unique style for a single element.

```
<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html>
```

## CSS color Property

```
body {
  color: red;
}

h1 {
  color: #00ff00;
}

p.ex {
  color: rgb(0,0,255);
}
```

The color property specifies the color of text.

### CSS Syntax

color: color|initial|inherit;

### Property Values

color	Specifies the text color. Look at CSS Color Values for a complete list of possible color values.	

initial	Sets this property to its default value.

inherit	Inherits this property from its parent element.

## Things I want to know more about

How does the process of a developer request for a new element of CSS to be add go about?


References: 
https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/What_is_CSS

https://www.w3schools.com/css/css_howto.asp 

https://www.w3schools.com/cssref/pr_text_color.php 