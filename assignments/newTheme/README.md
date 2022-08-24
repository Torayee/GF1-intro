# Make a new theme for your digital business card
An assignment in CSS variables and themes and praticing folowing a textual guide and find unknow CSS properties in the documentation/google.

# A short theory
Sometimes you wnat a different look on your site whether it's colors, typography, placement of the elements or all of these. You want your site to have a different theme. 

HTML is the skeleton of the website but CSS determines how it looks. Width, height, color, placement etc. 

But what if we want to be able to change these? 
We **DON'T** want to copy our stylesheet everytime and just changing the few variables - that's a waste of code. We wan't to keep it as simple an readable and easy to use as possible. I mean.. we can be lazy, it's actually a asset at times. 

**Introducing: variables.**

So you might remember in math classes having to write equations like `y = x + 6` and the result of `y` changes depending on the value of `x`. Those a variables. Their values can change but their names remains the same. So mathematicians like to write short letters as names. We rather want to write something that makes sense so we actually know what kind of value this variable holds. 

When designing our website we usually stick to 2 typographies and maybe 3-4 colors that repeat throughout the stylesheet. By placing these values in a variable we we will only have to call that variable whenever we need it's value. 

This also mean that we only have to change this value at 1 line in our CSS and not everytime that color is used in classes and elements. 

We define our variables at the absolut top of the stylesheet in an element called `:root{}`. The variable name should always start with 2 dashes `--` and the cabn hold any value. So defining your variables should look like this:

``` 
:root{
    --variablename: value;
}
```

When you wan't to call your variable name you use the build in `var()` function like this (note tha var is short for variable):


```
element{
    property: var(--variablename);
}

```

To give an example where I have saved 2 colors and use them. So in this example all text whatever the type that is within the `<body></body>` element in the HTML:

``` 
:root{
    --base-color: black;
    --accent-color: yellow;
}

body{
    color: var(--base-color);
}

.qoute{
    color: var(--accent-color);
}

```

### Making a theme out of variables
So you have all your theme related styling in variables - Maybe you also added some other values like placements or sizes. But you want to be able to switch between multiple themes. What you can do is make a new stylesheet or several and save your variables there. You can then link to the theme stylesheet you want to use within the HTML. 

So if you have 2 stylesheets `style.css` and `themeRed.css` you can link to both in your `<head></head>` element in HTML

``` 
<link rel="stylesheet" href="style.css" >
<link rel="stylesheet" href="themeRed.css" >

```

## The assignment
NOW we are going to play!!


You are going to make a new theme for your digital business - This assignemnets also train you in following a text based guide/tutorial that expects you to have a little knowledge about the subject already - it also expects you to know how to look up google and documentations for properties that you might not already know. 
Don't worry, if you have finished the other assignments this should not be too strange.


* In your "visikort" project add 2 other stylesheet called `themeBase.css` and `themeCustom.css`
* take your `:root{}` element from `style.css` and copy it over to `themeBase.css` and to `themeCustom.css`- delete it from `style.css`
* Link to you themes in the HTML below you other `<link>` element so you have 3 `<link>` elements in total
* Comment out the `<link>` to the theme you don't want to use. 
* In you `themeCustom.css` you can now play - change the values of the variables and see what happens. 
* You can also add variables, like background-color , or what else you like. 
* If you want to add some new properties you can call the element or class in the `themeCustom.css` that you want to apply the property to. This will be added to `style.css` when the browser reads the `index.html`


### A handy tip.. 
If you want inspiration on what you can change and how you can look at [CSS reference](https://cssreference.io/) for a pretty decent visual guide in backgrounds and typography in CSS. Also feel free to google "How to change the background color in CSS" or "how to change font size in HTML" or anything you might be curious about. 

If it gets too overwhelming or you get stuck or need inspiration - feel free to ask, each other AND me. 


