# `HTML`

### `Hyper Text Markup Language`

```html
<!DOCTYPE html> 
<html>
 
   <head> 
      <title>Align Attribute  Example</title> 
   </head>
	
   <body> 
      <p align = "left">This is left aligned</p> 
      <p align = "center">This is center aligned</p> 
      <p align = "right">This is right aligned</p> 
   </body>
	
</html>
```

![Element](Image/Element.png)

### `HTML Element` : `Start Tag` + `Content` + `End Tag`

### What are HTML `Tags` ?
- Primary component of the HTML enclosed within angle braces `<>`

### What are `Attribute` ?
- Define the characteristics of an HTML Element (Case Sensitive)

```html
<p align = "left">This is a content</p> 

Here 👆🏻 
<p> : Paragraph Starting Tag.
align : Attribute that define the characteristic for content. 
left : Value of an attribute.	
content : Text to be displayed on website.	
</p> : Paragraph End Tag.	
```

### What are HTML `Void Elements` ?  
- HTML Elements which do not have closing tags e.g. `<img>`, `<br>`, `<hr>`, etc.

### What are `HTML Entities` ?  
- Reserved Characters like `<`, `>`, `\`, etc
- To use this characters on web pages we need to use HMTL Entities.

Character | Entity Name
:--- | :---
`<` | `&lt;`
`>` | `&gt;`
`&` | `&amp;`
non breaking space e.g 10 PM | `&nbsp;`

### What is the `class attribute` in HTML?
- Class attribute is used to specify class name for an HTML Element.
- Multiple elements in HTML can have same class value.
- We can use `id` attribute to create difference between same class values.

```html>
<p class = "row"></p>
```

### Describe HTML `layout structure`
- Web page has different components to display the intended content.
- `<header` : Display header information of the web page (Top)
- `<footer` : Display footer of the web page (Bottom)
- `<nav>` : Navigation menu of HTML page.
- `<article>` : Set of information.
- `<section>` : Used inside article block to define basic structure of a page.
- `<aside>` : Sidebar content of page.

### HTML `Formatting tags`
- `<b>` - `bold` text
- `<i/>` - `italic` text
- `<em>` - `italic` text with added semantics importance 
- `<big>` - increases the font size of the text by one unit
- `<small>` - decreases the font size of the text by one unit
- `<sub>` - `subscript` text
- `<sup>` - `superscript` text
- `<del>` - `strikeout` text
- `<strong>` - `bold` important text
- `<mark>` - `highlight` text
	
### `<head>` and `<body>` tag in HTML
	
- `<head>` tag provides information `metadata` about web page
- `<head>` is defined at top of HTML page.
- `<body>` tag is defined below `<head>` tag.
- `<body>` tag defines the body of the HTML document.
- All the contents to be displayed on web page like image, text, video using `<p>`, `<img>`, `<audio>`, `<video>`, etc

### How to display a web page inside a web page (`Embed`)?

```html
<iframe src=”url of the web page to embed” />
```

### What is `Cell Padding` and `Cell Spacing` ?
- `Cell Padding` : Space between `content` and `border` of the cell.
- `Cell Spacing` : The space or gap between two consecutive cells.

### `rowspan` : Club two or more rows into one single row.

### `colspan` : Club two or more columns into one single column. 	

### Difference between `display:none` and `visibility:hidden` attributes 
- `display:none` : Element will be `hidden` and won't take up any extra space on web page.
- `visibility: hidden` : Element will be `hidden` from the web page but still takes up space.

### How to specify `link` in HTML and explain `target` attribute ?
- HTML provide `hyperlink` : `<a>` tag with `href` attribute to specify the link.
- `target` attribute is used to specify the behaviour of click.

Target Attribute Value | Behaviour
:--- | :---
`_self` | Default value, opens page in same window.
`_blank` | Open the page into new tab
`_parent` | Open the page in parent frame
`_top` | Open page in full body window 

### How many ways to specify `CSS` Styles ?
- `Inline` : Use `style` attribute inside HTML elements
```html
<p style='font-family:SF Mono'>
</html>	
```
- `Internal` : Use `<style>` tag inside `<head>` tag. Bind elements using `id` or `class` attributes.
```html
<html>
	<head>
		<style>
			@font-face {font-family: 'Moon'; src: url(../Font/MoonBold.ttf);}
		</style>
	</head>
	
	<body>
	</body>
</html>	
```			
