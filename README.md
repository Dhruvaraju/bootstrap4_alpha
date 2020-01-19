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
- Adding Live server to VS code
    - Search in extensions for __Live Server__ plugin (Author Ritwick Dey) and install it.
    - It will help to view the changes in browser, without refreshing the page.
- Themes can be set from extensions (Material theme by Mattia Astorino)

> Bootstrap documentation has multiple version, so check the version which you are using properly.

### Including bootstrap in your project
- __Using a cdn(Content Delivery network)__ link in your ui project.
- For which the links are added to our project as shown below.
```
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