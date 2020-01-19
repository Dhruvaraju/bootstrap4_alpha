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
```
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
- 
