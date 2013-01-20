# Javascript Talk

## Why Javascript?
- de facto language of the web
- Write once, run anywhere (browsers, servers(node), windows8…)
- asynchronous (nonblocking)

### What can you do with Javascript?
1. Respond to user actions
- clicks, hovers, key presses
2. Manipulate page content
- Add text, images, etc dynamically
3. Get data from external APIs
- your javascript asks another server for information which you can manipulate and add to the page.
- For example, insert weather.
4. Get data from local APIs
- window size, scroll position
- accelerometers, camera

## Tools of the Trade
### Why jQuery?
- most popular javascript library
- write simpler code
- simplifies cross browser compatibility
- plugins which cover lots of common behavior
- jquery ui covers lots of elements like tabs, date pickers, accordions, sliders, and more. See http://webdeveloperpost.com/Articles/10-most-useful-jQuery-functions-for-your-website.aspx#jQuery-Animate-Functions

### Inspector
- Most browsers have them. Chrome's is my favorite.
- Offer a console, sort of like a terminal interface for your browser
- See errors/debug messages, inject code, 

## Functions

### Hello World
function hello() { console.log("hello world");}
hello(); -> "hello world"

### Composing Functions
function addOne(value){ return value + 1;}
function addTwo(value){ return addOne(addOne(count));}

addOne(5) --> (5 + 1) --> 6
addTwo(5) --> addOne(5 + 1) --> ((5 + 1) + 1) --> 7

### Variable Scope (local, global)
var count = 1;
function incrementCount(){ count++; }

incrementCount();
console.log(count); --> count == 2;

incrementCount();
console.log(count); --> count == 3;
…

### Respond to User Input

var someButton = $('#myButton');
someButton.click(function(){ do stuff });

### Manipulate Page Content

var someDiv = $('#myDiv');
someDiv.text('Hello world');
someDiv.html('<a>link</a>');
someDiv.append(some element);

### Fetch Data from APIs

- GET requests work like regular URLs
- $.get(url, function(data){ do stuff });
- YQL API is super friendly




