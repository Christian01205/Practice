# Learning HTML Full Course
- HTML (HyperText Markup Language) is the code that is used to structure a web page and its content. For example, content could be structured within a set of paragraphs, a list of bulleted points, or using images and data tables. As the title suggests, this article will give you a basic understanding of HTML and its functions.

# Basic Elements

- `<html></html>` -> (You can also add `<html lang="en">` attribute, to specify what language do you want to use.)
- `<body></body>`
   - `<h1></h1>` -> which stands for heading (only used once and it's used to say what your website's topic is about.)
   - `<p></p>` -> stands for paragraph.
- `<head></head>`
  - `<meta charset="UTF-8">`
  - `<title></title>` -> Webpage title.
- `<!DOCtype html>` -> A doctype declaration that you should have in EVERY html file at the beginning.

# Head Elements

- `<meta name="author" content="name-of-the-author">` -> This is used to identify the author of the website.
- `<meta name="description" content="description-of-the-website">` -> This is used to describe your website with details as to let them know what it's all about.
- `<link rel="icon" href="png-file" type="image/x-icon">` -> This is used to add a little fav icon on your website tab.

## *Take note:*

- One missing thing in a code line can result into a whole list of `errors` when validating it. So After validating the file and it shows an error, visual code tells you that by making a certain `prompt` to turn into either color red/pink so make sure to follow it and DON'T FORGET TO ALWAYS VALIDATE YOUR WEBPAGE.

# Text Basics

- `<h1></h1>`
  - `<h2>,/h2>`
  - `<h3></h3>` -> There's a heirarchy between these elements so you have to organize your elements by having `h1` as first then `h2` etc...
- `<hr>` -> makes a horizontal line.
- `<br>` -> this is used to make a paragraph inside the `<p>` element to not have `white space` or separate the other paragraph.
-  `&nbsp;` -> used to add more additional space to a text.
-  `&lt;` -> used to make a `<` symbol.
-  `&gt;` -> used to make a `>` symbol.
-  `&copy;` -> used to add a `copyright` symbol.
-  `<address>` -> used to add a specific location and tells the browser that this is an address.
-  `<!--Any kind of text-->` -> used to write a note or a reminder to yourself inside the code editor (not visible to the website interface).
-  `<abbr title="example"> Ex. </abbr>` -> used to see the meaning of an abbrevated word.

# List Types

1. Ordered list -> It makes an ordered list/numerical list
```html
<ol>
        <li>example name 1</li>
        <li>example name 2</li>
        <li>example name 3</li>      
</ol>
```
### _Result:_
```
1. example name 1
2. example name 2
3. example name 3
```


2. Unordered list -> It makes an unordered/non numerical list.

```html
<ul>
  <li>example name 1
  <li>example name 2
  <li>example name 3
<ul>     
```
### _Result:_

```
・example name 1
・example name 2
・example name 3
```

3. Detailed List -> It makes a detailed list and it consist with two additional elements which is DESCRIPTION TERM `dt` and DESCRIPTION DETAIL `dd`.

```html
<dl>
  <dt>Example Term 1</dt>
  <dd>Example detail 1</dd>

  <dt>Example Term 2</dt>
  <dd>Example detail 2</dd>
```

### _Result:_

```
Example Term 1
       Example detail 1
Example Term 2
       Example detail 2
```