# bootstrap4_alpha
Learning Log for bootstrap

### What is bootstrap? 
- Bootstrap helps to create a responsive, mobile-first projects on the web with the most popular component library.
- In addition to the normal files we use while creating an UI we will be adding an additional CSS and JS file.
- We will be adding a lots of style classes to achieve this.

### Bootstrap pros and cons
#### Pros:
- Faster development, as lots of reusable components.
- Compatible with multiple browsers.
- Responsive layouts can be build with minimum code.
#### Cons:
- while using a single component you might have to load the entire file. which comes with bootstrap.

### Changes between bootstrap 3 to bootstrap 4
- Flexbox is enabled by default in bootstrap 4.
- Panels, thumbnails and wells were removed, replaced with cards.
- Unit of measure updated from pixels to rem.
- New grid size and tier added.
- Moved from LESS to SASS.
- Glypicons are removed.
- New utility classes are added.

### Environment Set up
- We need a code editor, prefer Microsoft Visual code if possible.
- Install __EMMET__ which is a plugin which will improve html editing a lot.
    - __EMMET__ comes preinstalled with VScode.
    - Some of the short cuts are, Create an empty html
```html
// ! and tab with out space will provide the basic html 5 structure.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
// if an element and tag is mentioned it will create a syntax for it example p.block
 <p class="block"></p>
// enter a tag name and name its class after '.' or its id after '#' use '*' for repeating the same
// div.note$#secops$*5
<div class="note1" id="secops1"></div>
<div class="note2" id="secops2"></div>
<div class="note3" id="secops3"></div>
<div class="note4" id="secops4"></div>
<div class="note5" id="secops5"></div>
// Nesting can also be done div>p>button.autoSize#button1
<p><button class="autoSize" id="button1"></button></p>
 ```
- Adding Live server to VS code
    - Search in extensions for __Live Server__ plugin (Author Ritwick Dey) and install it.
    - It will help to view the changes in browser, without refreshing the page.
- Themes can be set from extensions (Material theme by Mattia Astorino)

> Bootstrap documentation has multiple version, so check the version which you are using properly.

### Including bootstrap in your project
- __Using a cdn(Content Delivery network)__ link in your ui project.
- For which the links are added to our project as shown below.
```html
<!doctype html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" crossorigin="anonymous">

    <title>Hello, world!</title>
  </head>
  <body>
    <h1>Hello, world!</h1>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.4.1.slim.min.js" integrity="sha384-J6qa4849blE2+poT4WnyKhv5vZF5SrPo0iEjwBvKU7imGFAV0wwj1yYfoRSJoZ+n" crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.0/dist/umd/popper.min.js" integrity="sha384-Q6E9RHvbIyZFJoft+2mJbHaEWldlvI9IOYy5n3zV9zzTtmI3UksdQRVvoxMfooAo" crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js" integrity="sha384-wfSDF2E50Y2D1uUdj0O3uMBJnjuUD4Ih7YwaYd1iqfktj0Uod8GCExl3Og8ifwB6" crossorigin="anonymous"></script>
  </body>
</html>
```
- Downloading the files and linking them in you project.
- We can download production or source version from https://getbootstrap.com

### Basics of bootstrap
> Examples are present in demo.html
#### Colours
- CSS colour classes are given based on the functional overview, Success will have a specific colour, alert will have default and so on. This information can be found in Documentation >> Utilities >> colour
- Text colour classes will start with 'text-' example: text-primary
``` <p id="textdemo1" class="text-primary">Primary text</p> ```
- Back ground colours also will have the same thing.
- Background colour classes start with bg, eg: bg-primary
``` <p id="textdemo1" class="bg-primary">Primary background</p> ```
#### Buttons
- Buttons related info will be present in documentation >> components >> buttons
- Button classes are defined to perform there semantic purpose, Starts with btn
- Normal buttons
```html
<button type="button" class="btn btn-primary">Primary</button>
<button type="button" class="btn btn-secondary">Secondary</button>
<button type="button" class="btn btn-success">Success</button>
<button type="button" class="btn btn-danger">Danger</button>
<button type="button" class="btn btn-warning">Warning</button>
<button type="button" class="btn btn-info">Info</button>
<button type="button" class="btn btn-light">Light</button>
<button type="button" class="btn btn-dark">Dark</button>

<button type="button" class="btn btn-link">Link</button>
```
- Outline buttons will have only outline with out any background colour, class name example btn-outline-primary
- For button sizes there are 2 sizes small (btn-sm) and large (btn-lg) 
- Classes for button states are also available 
```html
<button type="button" class="btn btn-lg btn-primary" disabled>Primary button</button> // A boolean disabled is mentioned
```
#### Typography
- Default heading from h1 to h6 can be given without any class they will have there own formating.
- We can also use h1 to h2 as a class ```html <p class="h1">h1. Bootstrap heading</p> ```
- 'text-muted' will provide a slight faded effect.
- Display texts will provide an opinionated heading style for which we have display-1 to display-4 classes. ```html <h1 class="display-1">Display 1</h1> ```
- .lead will provide a paragraph to stand out from others.
- Basic text formating is done with the tags itself no additional classes required
```
            <p>You can use the mark tag to <mark>highlight</mark> text.</p>
            <p><del>This line of text is meant to be treated as deleted text.</del></p>
            <p><s>This line of text is meant to be treated as no longer accurate.</s></p>
            <p><ins>This line of text is meant to be treated as an addition to the document.</ins></p>
            <p><u>This line of text will render as underlined</u></p>
            <p><small>This line of text is meant to be treated as fine print.</small></p>
            <p><strong>This line rendered as bold text.</strong></p>
            <p><em>This line rendered as italicized text.</em></p>
```
- class blockquote for quoting others work and source can be mentioned in footer tag with class blockquote-footer wrap the source in cite.
```html
<blockquote class="blockquote">
  <p class="mb-0">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
  <footer class="blockquote-footer">Someone famous in <cite title="Source Title">Source Title</cite></footer>
</blockquote>
```
- For text alignment use the classes text-center, text-right, text-left
```html
<blockquote class="blockquote text-right">
            <p class="mb-0">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
            <footer class="blockquote-footer">Someone famous in <cite title="Source Title">Source Title</cite></footer>
          </blockquote>
```
### Jumbotron
- A lightweight, flexible component that can optionally extend the entire viewport to showcase key messages on your site.
- Available in documentation >> components >> Jumbotron
- This is a class that need to be applied on div tag, we have jumbotron and fluid jumbotron
  - Jumbotron will highlight the message provided by using container like style
  - Fluid jumbotron will extend up to the corners of the page created.
  - Simple Jumbotron is mentioned below, examples are available in jumbotron_eg.html
```html
<div class="jumbotron">
  <h1 class="display-4">Hello, world!</h1>
  <p class="lead">This is a simple hero unit, a simple jumbotron-style component for calling extra attention to featured content or information.</p>
  <hr class="my-4">
  <p>It uses utility classes for typography and spacing to space content out within the larger container.</p>
  <p class="lead">
    <a class="btn btn-primary btn-lg" href="#" role="button">Learn more</a>
  </p>
</div>
```

### Breakpoints
- The exact size of screen where bootstrap changes the appearance of the elements on the screen are called responsive breakpoints. General pixel sizes that are considered are mentioned below
- Documentation available under overview
```sass
// Extra small devices (portrait phones, less than 576px)
// No media query for `xs` since this is the default in Bootstrap

// Small devices (landscape phones, 576px and up)
@media (min-width: 576px) { ... }

// Medium devices (tablets, 768px and up)
@media (min-width: 768px) { ... }

// Large devices (desktops, 992px and up)
@media (min-width: 992px) { ... }

// Extra large devices (large desktops, 1200px and up)
@media (min-width: 1200px) { ... }
```
### Display
- docs available under utility 
- This utility class is used to hide and display ui elements when a breakpoint happens. Quickly and responsively toggle the 
display value of components.
- Display utility classes that apply to all breakpoints, from xs to xl, have no breakpoint abbreviation in them. This is because those classes are applied from min-width: 0; and up, and thus are not bound by a media query. The remaining breakpoints, however, do include a breakpoint abbreviation.
- Syntax for invoking display
```
    .d-{value} for xs
    .d-{breakpoint}-{value} for sm, md, lg, and xl.

Where value is one of:

    none
    inline
    inline-block
    block
    table
    table-cell
    table-row
    flex
    inline-flex
```
#### Hiding elements

- For faster mobile-friendly development, use responsive display classes for showing and hiding elements by device. Avoid creating entirely different versions of the same site, instead hide elements responsively for each screen size.
- To hide elements simply use the .d-none class or one of the .d-{sm,md,lg,xl}-none classes for any responsive screen variation.
- To show an element only on a given interval of screen sizes you can combine one ``` .d-*-none class with a .d-*-* class, ``` for example ```.d-none .d-md-block .d-xl-none``` will hide the element for all screen sizes except on medium and large devices.

Screen Size |	Class
------------------|------------------
Hidden on all |	.d-none
Hidden only on xs |	.d-none .d-sm-block
Hidden only on sm |	.d-sm-none .d-md-block
Hidden only on md |	.d-md-none .d-lg-block
Hidden only on lg |	.d-lg-none .d-xl-block
Hidden only on xl |	.d-xl-none
Visible on all |	.d-block
Visible only on xs |	.d-block .d-sm-none
Visible only on sm |	.d-none .d-sm-block .d-md-none
Visible only on md |	.d-none .d-md-block .d-lg-none
Visible only on lg |	.d-none .d-lg-block .d-xl-none
Visible only on xl |	.d-none .d-xl-block

```html
<p>Example for display classes</p>
            <p class="d-inline bg-dark text-light">This is a p tag with display inline class d-inline</p>
            <p class="bg-dark text-light">By default the display will be set to block, this is an example for it</p>
            <p class="d-none">This will not appear for any screen size</p>
            <p class="d-sm-none text-light bg-dark">This will only appear on xs screen</p>
            <p class="d-none d-sm-block d-md-none text-light bg-dark">This will only appear in sm screen</p>
            <p class="d-none d-md-block d-lg-none text-light bg-dark">This will only appear in md screen</p>
            <p class="d-none d-lg-block d-xl-none text-light bg-dark">This will only appear in lg screen</p>
            <p class="d-none d-xl-block text-light bg-dark">This will only appear in xl screen</p>
```