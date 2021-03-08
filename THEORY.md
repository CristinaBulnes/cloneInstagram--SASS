# THEORY PART -- Answering some conceptual questions about SASS

## What is SASS? What does SASS stand for?
- Sass stands for Syntactically Awesome Stylesheet
- Sass is an extension to CSS
- Sass is a CSS pre-processor

Stylesheets are getting larger, more complex, and harder to maintain. This is where a CSS pre-processor can help.

Sass lets you use features that do not exist in CSS, like variables, nested rules, mixins, imports, inheritance, built-in functions, and other stuff.
<br></br>

## What is a CSS pre-processor?
CSS preprocessors are scripting languages that extend the default capabilities of CSS. They enable us to use logic in our CSS code, such as variables, nesting, inheritance, mixins, functions, and mathematical operations
<br></br>

## What does a pre-processor have to do with SASS?
<br></br>

## Why use SASS?
Sass facilitates you to write clean, easy and less CSS in a programming construct. It contains fewer codes so you can write CSS quicker. It is more stable, powerful, and elegant because it is an extension of CSS
<br></br>

## SASS has disadvantages? Which are?
- The developer must have enough time to learn new features present in this preprocessor before using it.
- Using Sass may cause of losing benefits of browser's built-in element inspector.
- Code has to be compiled.
- Difficult Troubleshooting.
<br></br>

## What is a SASS Variable? Explain why are useful
Variables are a way to store information that you can re-use later.
<br></br>

## Explain the SASS variables property with an example.
The following example declares 4 variables named myFont, myColor, myFontSize, and myWidth. After the variables are declared, you can use the variables wherever you want:

```sass
$myFont: Helvetica, sans-serif;
$myColor: red;
$myFontSize: 18px;
$myWidth: 680px;

body {
  font-family: $myFont;
  font-size: $myFontSize;
  color: $myColor;
}

#container {
  width: $myWidth;
}
```
<br></br>

## What is a mixin? Why is it important? Give an example
The mixin is one of the most powerful features of the CSS preprocessor Sass, an abstraction of a common pattern into a semantic and reusable chunk.

Mixins allow you to define styles that can be re-used throughout your stylesheet. They make it easy to avoid using non-semantic classes and to distribute collections of styles in libraries.

```
@mixin reset-list {
  margin: 0;
  padding: 0;
  list-style: none;
}

@mixin horizontal-list {
  @include reset-list;

  li {
    display: inline-block;
    margin: {
      left: -2px;
      right: 2em;
    }
  }
}

```
<br></br>

## What is SCSS? Give an example

Scss is Sassy Cascading Style Sheets
SCSS is a preprocessor which lets you use features that aren’t a part of the wider CSS standard yet, and provides better workflows for maintaining your stylesheets.

With SCSS preprocessor, you can reduce the amount of times you repeat yourself and ensure you’re writing clean, maintainable code for the future.

Scss can take css code and work. 

SCSS is fully compatible with the syntax of CSS, while still supporting the full power of Sass.

```
body {
  background-color:#000;
  color:#fff;
}
```
<br></br>

## What is SASS? Give an example
Sass is a stylesheet language that’s compiled to CSS. It allows you to use variables, nested rules, mixins, functions, and more, all with a fully CSS-compatible syntax. Sass helps keep large stylesheets well-organized and makes it easy to share design within and across projects.

```
body
  background-color:#000;
  color:#fff;
```
<br></br>

## What is the difference between .scss and .sass syntax.
SCSS (or Sass) offers a way to write styles for websites with more enhanced CSS syntax. In general, browsers do not know how to process SCSS features, such as functions, mixins, and nesting. We’ll need to convert them to regular CSS files to run them in the browser.
SCSS and Sass are two syntax flavors for the same concept. The difference between them is UI.
<br></br>

## In which cases would we use SCSS? And in which cases would we use SASS?

The difference is UI. Underneath the textual exterior they are identical. This is why sass and scss files can import each other. Actually, Sass has four syntax parsers: scss, sass, CSS, and less. All of these convert a different syntax into an Abstract Syntax Tree which is further processed into CSS output or even onto one of the other formats via the sass-convert tool.

Use the syntax you like the best, both are fully supported and you can change between them later if you change your mind.

SASS is used when we need a original syntax, code syntax is not required for SCSS.
Sass supports two different syntaxes. Each one can load the other, so it's up to you and your team which one to choose.

With a few small exceptions, it’s a superset of CSS, which means essentially all valid CSS is valid SCSS as well. Because of its similarity to CSS, it’s the easiest syntax to get used to and the most popular.

The indented syntax was Sass’s original syntax, and so it uses the file extension .sass. Because of this extension, it’s sometimes just called “Sass”. The indented syntax supports all the same features as SCSS, but it uses indentation instead of curly braces and semicolons to describe the format of the document.

In general, any time you’d write curly braces in CSS or SCSS, you can just indent one level deeper in the indented syntax. And any time a line ends, that counts as a semicolon. There are also a few additional differences in the indented syntax that are noted throughout the reference.

## Explain how traditional CSS and Preprocessed CSS workflows are different.
CSS Preprocessors compile the code which is written using a special compiler. They then use that to create a CSS file, which can then be referenced by the main HTML document.

When using any CSS Preprocessor, you will be able to program in normal CSS just as you would if the preprocessor were not in place. The good thing is you also have more options available to you. Some, such as SASS, has specific style standards which are meant make the writing of the document even easier, such as the freedom to omit braces if you want.

## Can we create functions with SASS? If it is true, give an example.
Yes, we can. 

Functions allow you to define complex operations on SassScript values that you can re-use throughout your stylesheet. They make it easy to abstract out common formulas and behaviors in a readable way.

For example: 
```
@function pow($base, $exponent) {
  $result: 1;
  @for $_ from 1 through $exponent {
    $result: $result * $base;
  }
  @return $result;
}

.sidebar {
  float: left;
  margin-left: pow(4, 3) * 1px;
}
```

## What is nesting? Is it useful? Give an example of nesting
Is a way you can write code to have a clear nested and visual hierarchy.
```
nav {
  ul {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  li { display: inline-block; }

  a {
    display: block;
    padding: 6px 12px;
    text-decoration: none;
  }
}
```
## Why use @import?
Becouse it allow you to keep the CSS code DRY (Don't Repeat Yourself).

One way to write DRY code is to keep related code in separate files.
You can create small files with CSS snippets to include in other Sass files. Examples of such files can be: reset file, variables, colors, fonts, font-sizes, etc.

The @import directive allows you to include the content of one file in another.

## How can we import other CSS/SASS files in SASS? Give an example
Sass Import Syntax:
```
@import filename;
```
You do not need to specify a file extension, Sass automatically assumes that you mean a .sass or .scss file. You can also import CSS files. The @import directive imports the file and any variables or mixins defined in the imported file can then be used in the main file.

You can import as many files as you need in the main file

## Explain the concept of inheritance in SASS.
Inheritance lets you share a set of CSS properties from one selector to another.

## Why use @extend? Give an example
@extend is used to share a set of CSS properties from one selector to another. It helps keep your Sass very DRY.