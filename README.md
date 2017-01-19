# ScriptEd >_
## Code Patterns in HTML, CSS, and JavaScript

### Table of Contents
[HTML](#html)
- [Linking CSS](#linking-css)
- [Linking JavaScript](#linking-javascript)
- [Linking CSS and JavaScript for Bootstrap](#linking-css-and-javascript-for-bootstrap)

### HTML
#### Linking CSS 
_where `app.css` is your custom CSS file_
```html
<!DOCTYPE html>
<html>
    <head>
        <title>Page Title</title>
        <link rel="stylesheet" type="text/css" href="./app.css">
    </head>
    <body>
    </body>
</html>
```
#### Linking JavaScript 
_where `app.js` is your custom JavaScript file_
```html
<!DOCTYPE html>
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body>
    
    <script type="text/javascript" src="./script.js"></script>
    </body>
</html>
```
#### Linking CSS and JavaScript for Bootstrap 
_where `app.css` and `app.js` are your custom CSS 
and JavaScript files respectively_
```html
<!DOCTYPE html>
<html>
    <head>
        <title> </title>
        <!-- Bootstrap -->
        <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" 
        integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">
        <!-- Custom -->
        <link rel="stylesheet" type="text/css"  href="app.css">
    </head>
    <body>
    
    <!-- jQuery -->
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
    <!-- Bootstrap -->
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js" integrity="sha384-
    Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa" crossorigin="anonymous"></script>
    <!-- Custom -->
    <script type="text/javascript"  src="app.js"></script>
    </body>
</html>
```
