# Html Website Tutorial
## What Is HTML?

The HyperText Markup Language (HTML) is the most fundamental building block of the web. It defines the structure and content of every web page. It is the common language for all websites and browsers, which is why you can use your browser to visit any website, and your browser just knows what to do. An HTML document is a file with extension .html.

Generally speaking, other technologies are used alongside. The Cascading Style Sheet (CSS), for example, can be used to describe the page’s appearance, and JavaScript can define the web page’s behavior and make it more interactive for the user. We will talk about these technologies in detail in future articles.

Before proceeding with this article, make sure you have a code editor and a browser installed on your computer.

Here is an example of an HTML file:

```js

1.  <!DOCTYPE html>
2.  <html>

3.  <head>
4.    <meta charset="utf-8" />
5.    <title>My HTML page</title>
6.  </head>
7.  
8.  <body>
9.    <h1>This is a heading</h1>
10.    <p>This is a paragraph.</p>
11. </body>
12. 
13. </html>

```

Elements are the basic components of this HTML file. An HTML element is usually defined by a start tag and an end tag, and with some content in between like this:

```js

1.  <body>
2.    <h1>This is a Heading</h1>
3.    <p>This is a paragraph.</p>

4.    <div>
5.      <p>This is also a paragraph.</p>
6.    </div>
7.  </body>

```
<p align="center">
    <img src="/docsImages/html-dom-tree.png">
</p>

The `<body>` has three elements inside, a heading `<h1>`, a paragraph `<p>`, and a `<div>`. And the `<div>` element has another paragraph `<p>` inside. The plot above is what the structure tree looks like. There is no limit on how long or complex this tree could be. This is related to a fundamental concept in frontend development called the Document Object Model (DOM). With the DOM, we can find and change any element in an HTML file.

Another important note is that you should never escape the end tag (if it needs one). Sometimes the elements will display correctly, but you should never rely on that. It can cause unexpected consequences.

Usually, each HTML element is assigned multiple attributes. They provide additional information to the HTML elements. They are always specified in the start tag, and they usually come in name/value pairs like this:

``bash
1.  <tag name="value">An Example</tag
``

There are two essential things you should always remember. First, the attributes should always be in lower case. It is not a requirement, but it is highly recommended. [XHTML,](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/XHTML) the strict version of HTML, actually demands that. Second, the value of the attributes should always be in quotes. It doesn’t matter if you use single or double quotes, but they should always match. Using double quotes is highly recommended. Again, XHTML requires you to use double quotes

# Some common elements and attributes
Next, let’s take a look at some commonly used HTML elements. Please note that this is not a complete list of all elements for HTML. That would make this article long and tedious. However, [here](https://www.ericsdevblog.com/posts/html-basics-1/) is a complete tutorial on HTML from w3schools if you need them.

## Headings and paragraphs
Headings are used to defining the hierarchy and structure of the web page. HTML offers six different levels of heading, from `<h1>` to `<h6>`. `<h1>` is the most important heading, and it should summarize your entire page content, which is why there should only be one `<h1>` heading in the HTML file

```js

    <body>
1.    <h1>Heading level 1</h1>
2.    <h2>Heading level 2</h2>
3.    <h3>Heading level 3</h3>
4.    <h4>Heading level 4</h4>
5.    <h5>Heading level 5</h5>
6.    <h6>Heading level 6</h6>
</body>

```

The output should look like this:
<p align="center">
    <img src="/docsImages/html-headings.png">
</p>

Paragraphs on the other hand, are defined with the `<p>` tag

```js

1.  <p>This is a paragraph.</p>
2.  <p>This is also a paragraph.</p>

```

In HTML, you cannot change how the paragraphs are displayed in the browser by adding extra spaces or extra lines in the code. They will be automatically removed by the browser. For instance, the following two paragraphs will produce the same resul

```js

1.  
2.  <p>This is a paragraph.</p>
3.  
4.  <p>This           is a 
5.  paragraph.</p>

```
However, what if we do want a line break? The answer is simple, we use a `<br>` element:

```js
1.    <p>This is a `<br>` paragraph.</p>
```
The output will be:

# Formatting elements
The formatting elements are a special collection of elements that give texts special meaning and appearance.
-    `<b>` - Bold text
-    `<strong>` - Important text
-    `<I>` - Italic text
-    `<em>` - Emphasized text
-    `<mark>` - Marked text
-    `<small>` - Smaller text
-    `<del>` - Deleted text
-    `<ins>` - Inserted text
-    `<sub>` - Subscript text
-    `<sup>`- Superscript text


```js

1.  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. <b>Vestibulum volutpat pretium turpis, sodales facilisis metus
2.       porta a.</b> Morbi condimentum porta massa, eu mattis turpis cursus sit amet. <strong>cursus ut tellus a convallis. In nec
3.       nisl nisl.</strong> Mauris a ligula et ligula malesuada luctus. <i>Fusce placerat id tortor at tristique.</i> Quisque non vulputate
4.       eros. <em>Pellentesque malesuada interdum ligula, et dignissim arcu vestibulum tincidunt.</em></p>
5.
6.  <p><mark>Aliquam imperdiet volutpat lorem, in viverra lorem ultricies sed.</mark> Integer bibendum velit sit amet hendrerit
7.       venenatis. <small>Suspendisse interdum ornare molestie.</small> Nulla porttitor venenatis purus eu sollicitudin. <del>In quis aliquet
8.       ipsum. Curabitur eu feugiat sem.</del> Etiam rhoncus lectus eget dolor cursus, a viverra tellus faucibus. <ins>Nam aliquam
9.       rhoncus urna.</ins> Vivamus pulvinar eleifend nibh quis semper. <sub>Sed finibus neque in</sub> sollicitudin cursus. <sup>Curabitur ut ex
10.      </sup>egestas, suscipit lectus a, auctor ante.</p>

```

The output should look like this:
<p align="center">
    <img src="/docsImages/html-formatting-elements.png">
</p>

## Links
Links are found on nearly all web pages. They allow users to travel from page to page. When you click on a link, it takes you to another HTML file, and this simple action forms the foundation of the internet. The links are defined as follows:

```js
1.  <a href="https://www.example.com/">link text</a

```
The browser will display an underlined text, and when you click on it, it will take you to https://www.example.com/.

By default, when you click on a link, the target shows up in the same browser tab. You can change this behavior using the target attribute.

-   _self - Default. Opens the document in the same window/tab as it was clicked
-   _blank - Opens the document in a new window or tab
-   _parent - Opens the document in the parent frame
-   _top - Opens the document in the full body of the window

For example, the following link will take you to a new tab:

```js
1.  <a href="https://www.example.com/" target="_blank">link text</a>

```