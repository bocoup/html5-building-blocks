JavaScript is a programming language invented by the honerable Brendan Eich in 1995 when he worked at netscape. It is a programming language born of the internet, and developed for the browser. However, JavaScript is not just a browser scripting language. JavaScript is a first class programming language with desktop and server side runtimes just like any other programming language.

##JavaScript Types
In JavaScript there are 6 types; `object`, `string`, `array`, `number`, `boolean`, `function`. All JavaScript programs are written using these types.

###[[Object]]
Objects are the building blocks of JavaScript programs. In JavaScript, everything is an object.

Here is an example of a JavaScript Object. This object is called an object literal, because it is literally written out in the code, as apposed to being constructed by a function and stored in memory:
    {
      property: 'value',
      secondPropery: {
        property: 'this is a property of the secondProperty object which is a property of the parent object literal'  
      }
    }

An object can also be assigned to a variable like so `var myObject = { property: 'value', secondProp: 'anotherValue'}`

###[[String]]
A string is piece of text in quotes. For exaple:

    'I am a string of text'

###[[Array]]
An array is a list of members. These members can be anything, including a string, number, array, function, boolean. For example:
    ['I am', 'an array of', 'strings and', 18, 'numbers']

###[[Number]]
A number is a literally a number.

For example


###[[Boolean]]
A boolean is either true or false. Booleans can be used to evaluate the truthiness of something.
For example:
    true

###[[Function]]
Functions are the things that actually do something in a JavaScript program. Functions in JavaScript are very similar to the functions you learned about in algebra ( remember f(4) = 8, solve for f ?). Functions take arguments, and do things with them. Functions can be called by other functions, passed around in variables, and much more.

--------------------
##More vocabulary
###[[Method]]
A method is a function property of an object.

###[[Variable]]
A variable is a placeholder. A variable can hold anything, including a string, number, array, function, boolean.
--------------------
##List of javascript things
* Native
    * Math
    * JSON
* Host
    * document.location
    * history
    * screenLeft
    * screenTop
    * screenX
    * screenY
    * scrollX
    * scrollY
    * top
    * self
    * statusBar
    * Range