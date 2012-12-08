javascript-keycode-jelly
========================

javascript-keycode-jelly is a Javascript library that makes handling keyboard events as sweet as jelly. The library is developed in coffeescript and includes a javascript compilation if you don't have access to a coffee compiler. This library is meant to be used in web applications that run in a browser.

## Installing

To install this library simply include the following line of code in the head tag of the HTML page you wish to use it in:

`````html
<script type="text/javascript" src="path/to/key.js"></script>
`````

The library attaches itself to the global window object and is accessed through:

`````javascript
window.Key
`````

or simply

`````javascript
Key
`````

## Low-level Constants

Don't you hate having to lookup the key code for the enter key every time you want to check and see whether it has been pressed? With javascript-keycode-jelly you can say goodbye to all of that and use intuitive key code references like the following:

`````javascript
// Example of constants in the library
Key.A // returns key code for 'A' key
Key.ENTER // returns key code for 'Enter' key
Key._0 // returns key code for '0' key
Key.NUM_PAD_2 // returns key code for '2' key on the number pad
Key.UP_ARROW // returns key code for 'up arrow' key
Key.CTRL // returns key code for 'control' key
Key.ESCAPE // return key code for 'escape' key
Key.COMMA // returns key code for 'comma' key
Key.F1 // returns key code for 'F1' key
Key.BACK_SLASH // returns key code for 'back slash' key
`````

Well you get the idea. These constant values can be used to verify what key was pressed when handling a keyboard event as in the following examples:

`````javascript
// For IE
if (e.keyCode === Key.TAB)
  // Do something awesome
  
// For all the other browsers
if (e.which === Key.CAPS_LOCK)
  // Do something else that's awesome
````