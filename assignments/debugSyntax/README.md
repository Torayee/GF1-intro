# Debug Syntax
Small assignments in debugging syntax of HTML and CSS to get introduced to working with coding. 

## Debugging
Working with code is not just pure tapping and creation. Most of the time is used to think, to optimize, to refactor, to analyze - most of the time you a debugging your code or someone elses code. 

These assignments are to help you become familiar not only with some of the process of debugging but also to become more familiar with the code it selv and it's syntax. 

*So A quick summary of the syntax of HTMl and CSS:*

### HTML
```
<element property="value">
    Content
</element>
```
As a Markup language HTML mainly contains element tags with other nested elemenent tags with - it's a box of boxes. 
Tags are used in HTML to signal the start and end of any element. The tag contains a element and some even contains properties. An element can be a heading like `<h1></h1>` or a paragraph like `<p></p>`. A property with a value is anything that might be descriptive about or connected to the element. This can be a name like `<h1 name="bigHeadline"></h1>` (name is the property and bigHeadline is the value), a CSS class with some styling to space up the look of our headline `<h1 class="sparkles"><h1>` or many other - the full list of properties can be found in the documentation. You are NOT supposed to know them all - not now, not in 20 years either. 

Most tags also contains content bestween them. This is the tekxt in your heading or paragraph like `<h1>An amazing headline</h1>` or `<p>This is a text... </p>`. Some tags have a reference to content that are stored elsewhere like an image `<img src="../images/picture.jpg" />`. Notice that the image tag is self closing (src standss for source, btw) `<img />`. Because the tag doesn't contain content stored in the HTML document such as text it doesn't need a start or close tag to contain them. So it just closes it self with a `< />` or just `< >` instead of `<></>`. 

Again - don't fret too much that you can't remember is it's selfclosing or not. You are NOT expected to be a walking encyclopedia as a succesfull developer. You just need to know how to use the encyclopedia provided for you in the documentation. Sounds easy enough right? It is! 

### CSS
```
element {
    property: value;
}
 ```
 The syntax for CSS has the same principles behind it as the Markup language - or any program language. You have your element then you have your start `{` and your end `}` tag. Within those you have your descriptive properties and their values. Allthough CSS don't deal with content. That is the HTMLs job. CSS only concerns it self with styling. How does the element look. it provides the sparkles. 

 CSS is pretty cool as it can interact directly with your HTML. This means that you can reference your HTML element tags in your CSS like our heading `h1 {}`. You can also make your own elements. These are called class and id. The rule is that classes can be reused throughout the document and you can have several classes on every element. Ids can only be used ONCE, hence they are rarely used in todays webdesigns. You will probaly see them on old designs though. Styling on direct elements like our h1 will be applied to EVERY h1 in the HTML document. 

You define that you are making a class with a dot befor the element as this `.sparkles {}`. We like classes they let us choose with elements in our HTML we want to sparkle. 

You define that you are making an id with a hashtag `#sparkles {}`. We don't want to risk limiting our sparkels oportunities so we won't use ids that much. 

The element name it self won't make it sparkle. For that you need properties and values. Though I havent found an actuan sparkle property yet. The most common you'll get to use will deal with the size, position and scalability of your elements. Both in regard to the viewport (the screen), browser type and in reference to each other. 

You can't have any space in the element, class, id or property name you can have dashes though. 


How you connect them to make them work together comes later - for now you'll work with each language seperately.

### The assignments
In the files index.html and style.css are several syntax errors. Your job is to correct them. When talking syntax errors we talk about the grammar of the language. How do we write our element, properties and values, how du we start and close etc. 

Each assignment is written in the comment before the codesnippet. A comment in CSS is written between a slash and star `/* comment */` and in html its between exclammation mark and dashes  `<!-- Comment -->`. 

Remember that syntax errors also includes spelling errors.

Use the syntax highlighter and the ES Lint eextention to provide some clues to where the bug exists.
