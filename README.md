# ScriptEd >_
## Code Patterns in HTML, CSS, and JavaScript

### Table of Contents
[HTML](#html)
- [Linking CSS](#linking-css)
- [Linking JavaScript](#linking-javascript)
- [Linking CSS and JavaScript for Bootstrap](#linking-css-and-javascript-for-bootstrap)

[JavaScript](#javascript)
- [Running JavaScript after HTML loads](running-javascript-after-html-loads)
- [Making API request and process response](making-api-request-and-process-response)
- [Read values from JavaScript object](read-values-from-javascript-object)

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
### JavaScript
#### Running JavaScript after HTML loads
```javascript
$( document ).ready(function(){
    console.log( "ready!")
});
```
#### Get an input element's value with jQuery
```javascript
// select <input id="search" />
var value = $("#search").val();
```
#### Changing an element's text with jQuery
```javascript
// <p id="result">Hello</p>
$("#result").text('Hello World')
// <p id="result">Hello World</p>
```
#### Respond to and element click event
```javascript
// <div id='box'></div>
$("#box").click(function(){
    console.log("Box clicked")
})
```
#### Change element CSS
```javascript
// <div id='box'></div>
$("#box").css("background", "green");
```
#### Making API request and process response
```javascript
$.getJSON("https://api.giphy.com/v1/gifs/search?q=dogs&api_key=dc6zaTOxFJmzC", function(response) {
    console.log(response);
});
```
#### Read values from JavaScript object
```javascript
var restaurant = {
    name: 'Coffee Place',
    location: 'New York'
}
console.log(restaurant.name)
// 'Coffee Place'

var restaurants = [
    {
        name: 'Coffee Place',
        location: 'New York'
    },
    {
        name: 'Burger Place',
        location: 'St. Louis'
    }
]
console.log(restaurants[1].location)
// 'St. Louis'
```
#### For Loop
```javascript
for (var i = 0; i <= 5; i++){
    console.log(i)
}
// 1, 2, 3, 4, 5
```
#### Loop through an array
```javascript
var myArray = ['a', 'b', 'c'];
for (var i = 0; i < myArray.length; i++){
    console.log(myArray[i])
}
// 'a', 'b', 'c'
```