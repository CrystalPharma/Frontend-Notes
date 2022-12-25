# Bootcamp Notes
## Fundamental Javascript
## Javascript 
JavaScript is a programming language that allows programmers to implement complex features on web pages — every time a web page does more than just sit there and display static information for you to look at — displaying timely content updates, interactive maps, animated 2D/3D graphics, scrolling video jukeboxes, etc. 

## JavaScript engine
-	Converts human readable codes into machine code without producing intermediate codes
-	Many of the JavaScript engine to date are JIT compilers (just in time compilers) that produce in time translation and optimisation 

## Console windows/ interfaces
- Allow to input commands and view outputs
- Input commands to console, taken live to JavaScript JIT engine compiled, processed and presented viewing the outputs of the commands delivered into human readable format texts 
- useful in debugging and reviewing any errors in inputting codes and highlight in the Console window
- Consoles are opened in common developer tools

## Console.log
Console.log is a function that prints message that exits in the Javascript engine
- it is particularly impprtant to test whether the code is functioning as intended

## Variables 
(Noun) in Javascript in the following forms:
- numbers  (1)
- strings ("string")
- Booleans (true, false)
etc.

## Arithmetic operators
- +(addition)
- -(subtraction)
- *(multiplication)
- /(division)

## Modulo Remainder
- Remainder operator(%) 
returns the remainder left over when one operand is divided by a second operand

## Assignment Operator
- Equality operators (=, ==, === strictly equality,!=== strict inequality )
- Comparison operators (>, <)

## Logical Operator
- || (or), && (and), ! (not)

## Array (arr)
- Single variable to store multiple elements (list of elements)
- simple to access particular element / variable later on 
<br>e.g. <code>var string = [1,2,3,,4,5,6];</code>
### Member access in arr
- start from 0 to the arr length - 1 (as starts from 0) <br>
e.g. <code>var string = [1,2,3,,4,5,6];<br> string[0] // print 1//
   </code>

## for loop
Control flow statement
for specifying iteration, which allows code to be executed repeatedly. A for 
loop has two parts: a headerspecifying the iteration, and a body
which is executed once per iteration.
<br>e.g. <code>
var string = [apple,pear,orrange,avocado,strawberry]; <br>
for (var i = 0; i < string.length; i++) { <br>
   console.log string[i]; <br>
} // print apple,pear,orrange,avocado,strawberry
</code>



## Alerts, Confirms and Prompts (text pop up or fill-in)
Alerts
<code>alert("Hello! I am an alert box!!");</code><br>
Confirms
<code>confirm("Would you like to code");</code>//return true or false in string form (confirm/cancel)<br>
Prompts
<code>
function myFunction() {
let person = prompt("Please enter your name", "Harry Potter");
  if (person != null) {
    document.getElementById("demo").innerHTML =
    "Hello " + person + "! How are you today?";}</code><br>
//return as string <br>
Important to parseInt* to return as number from string

## if else statement
The if...else statement executes a statement if a specified condition is true. If the condition is false, another statement in the optional else clause will be executed.
<br><code>function testNum(a) {<br>
  let result;<br>
  if (a > 0) {<br>
    result = 'positive';<br>
  } else {<br>
    result = 'NOT positive';<br>
  }<br>
  return result;<br>
}<br>

console.log(testNum(-5));
// expected output: "NOT positive"
</code>

## switch statement (simplified for multiple conditions)
The switch statement evaluates an expression, matching the expression's value against a series of case clauses, and executes statements after the first case clause with a matching value, until a break statement is encountered. The default clause of a switch statement will be shown if no case matches the expression's value.

<code> 
const expr = 'Papayas';<br>
switch (expr) {<br>
  case 'Oranges':<br>
    console.log('Oranges are $0.59 a pound.');<br>
    break;<br>
  case 'Mangoes':<br>
  case 'Papayas':<br>
    console.log('Mangoes and papayas are $2.79 a pound.');<br>
    // expected output: "Mangoes and papayas are $2.79 a pound."<br>
    break;<br>
  default:<br>
    console.log(`Sorry, we are out of ${expr}.`);<br> //ES6
}
</code>

## while loop
While loop execute a specified statement upon evaluating the condition to be true.
<br> <b>*Main difference between for loop and while loop</b>
<br> While loop executes the statement until there is a break condition (usually using if statements) / when the condition returned to be false
<br> for loop uses incrementation with the definite length
<br> e.g. 
<br> <code>let n = 0;

while (n < 3) {
  n++; <br>// looping though 1 - 3 and then returned n = 3

}

console.log(n);
// expected output: 3</code>


## Object
- Object literal 
JavaScript is designed on a simple object-based paradigm. An object is a collection of properties, and a property is an association between a name (or key) and a value. A property's value can be a function, in which case the property is known as a method.

Objects in JavaScript, just as in many other programming languages, can be compared to objects in real life. In JavaScript, an object is a standalone entity, with properties and type. Compare it with a cup, for example. A cup is an object, with properties. A cup has a color, a design, weight, a material it is made of, etc. The same way, JavaScript objects can have properties, which define their characteristics.

In addition to objects that are predefined in the browser, you can define your own objects. This chapter describes how to use objects, properties, and methods, and how to create your own objects.
- Key-value pairs
Unique identifier for accessing particular member value.<br>In objects, key-value pairs define the properties of an object


<img src ="./mc20.png">
<h2><u>Maserati MC20 Cielo</u></h2>

<code>
var maseratiMc20 = {

  engine :'v6', //key and value pairs 

  maxTorque : '730 Nm',

  maxSpeed : '>325 km/h',


}

//keys: engine, maxTorque, maxSpeed
//values: 'v6', '730 Nm', '>325 km/h'
</code>

## Method
Built in Named pieces of code with built in functions.
And in Window object, Console preview, contains of many functions (methods) set up by JIT compilers<br>
eg. -console.log -Math.random()
- Obj Method s
1. Object.keys()
Object.keys() returns an array iterate object that contains the keys of object
If you need the property values, use Object.values() instead. If you need both the property keys and values, use Object.entries() instead.<br>
<code>
const object1 = { 
  
   a: 'somestring',

    b: 42,

    c: false

    };


    console.log(Object.keys(object1));

    var arr = Object.keys(object1);

    console.log(arr[0]);

    for (var i = 0; i < arr.length; i++) {

      console.log(arr[i]);

    }
</code>
<br>

2. Object.values()<br>
Object.values() returns an array of values of the object

    <code>
    var maseratiMc20 = {

    engine :'v6',//key and value pairs 

    maxTorque : '730 Nm',

    maxSpeed : '>325 km/h',
    
    }
    var arrMc20 = Object.values(maseratiMc20);

    console.log(arrMc20);

    //return in console Array(3)

    arrMc20 = ['v6', '730 Nm', '>325 km/h'];
    
    </code>

3. Object.entries()<br>
Object.entries() returns an array of values of the object

    <code>
    var maseratiMc20 = {

    engine :'v6', //key and value pairs 

    maxTorque : '730 Nm',

    maxSpeed : '>325 km/h',
    
    }
    var arrMc20En = Object.entries(maseratiMc20);

    console.log(arrMc20En);

    //return in console Array(3)

   [
    [
        "engine",
        "v6"
    ],
    [
        "maxTorque",
        "730 Nm"
    ],
    [
        "maxSpeed",
        ">325 km/h"
    ]
]
    
    </code>

4.  parseInt Method
parseInt method is used to parse in strings(''/ "") into integers
<br>e.g.
<code>
</code>

## Nested data structure
A robust data structure is important to maintain function in multiple settings so that code inside can be easily updated <br>
There are different examples of nested data structures
- Arr of Arr
- Obj of Obj
- Arr of Obj
- Obj of Arr

## Composition
Simplified hierachy system created by compositioning - Javascript objects are integrated together from large complex objects into simpler objects which produce code that is more reusable, clean and provide better solution.

## Function
Block of code designed to perform particular task and it is executed when fucntion is called or invoked

- Function declaration
indicate by named function 
* particularly useful especially create on the global scope and be accessible throughout the code
<code>
function drive() {

  //function block;

  return;

}
</code>

- Function expression
Assign variable a function 
<code>
var drive = function() {

  //function block;

  return;

}
</code>
Assignment operator = we use function followed by {}

- Callback function
Callback function is usually passed into another function asynchronously  as an arguement to invoke a planned response - awaits for results generated from a synchronous function then complete the routine / action intended


## Parameters and Logic
Parameters allows to pass values into function by providing a name, values are then assigned when the function is being called/ invoked.
<code>
function greet(firstName) {

  console.log("Hello, " + firstName);

  return;

}
c
greet('Harry');
</code>

## Scope and Shadowing
Scope refers to the current context of scope that determines the accessibility of variables declared.
- Global Scope
Variables are accessible globally outside of block
- Local Scope
Variables are accessible locally inside of block
- Variable shadowing
Declaring a variable in certain scope and reassign values in another level of scope
The variable assigned within an inner scope shadows the outer variable assigned in the outer scope.

## This keyword
This is a keyword that always refer to an object and it can be referred to different values depends on the context. - window object, function, class or global.
<br> e.g.<br>
<code>
// this is refer to the global object

console.log(this);

// this is refer to the window object

function helloThis() {

  console.log('Inside this function, this is ' + this);

}

helloThis ();


// this is refer to the variable child object and refer to age:10 (property)

var child = {

  age: 10,

  ageTenYears: function () {

    console.log(this.age + 10);

  },

};

child.ageTenYears();

// this is refer to the variable investor and call property initial investment and multiply

var investor = {

  name: 'Cash Saver',

  investment: {

    initialInvestment: 5000,

    investmentGrowth: function () {

      console.log(this.initialInvestment * 1.15);

    },

  },

};

investor.investment.investmentGrowth();
</code>

## Array Methods
Method is an object that contains function value
### .sort()
sort() method is used to sort arr items into alphabetical order 
<br> e.g.<br>
<code>

const months = ['March', 'Jan', 'Feb', 'Dec'];

months.sort();

console.log(months);

// expected output: Array ["Dec", "Feb", "Jan", "March"]
</code>

### .push()
push() method is used to add one or more element(s) at the end of an array to the *original array
<br> e.g.<br>
<code>const arr1 = ['Moon', 'Sun', 'Mars'];

const space = arr1.push('Jupiter'); 
; // expected to be arr1 =['Moon', 'Sun', 'Mars', 'Jupiter'];

conaole.log(space); // expected to return as 4;
</code>


### .slice(start,end)
slice() method is used to slice and returns a portion of array into a new array object (passing in arguements of the start and end of slice)
<br>*require to store in a new varible, const
<br> e.g.<br>
<code>
	var animals = ['ant', 'bison', 'camel', 'duck', 'elephant'];
	var animalSlice = animals.slice(2);

  console.log(animals); // expected to return as ["ant",	"bison",	"camel",	"duck",	"elephant]
  console.log(animalSlice); //expected to return as ["camel",	"duck",	"elephant"]
</code>

### replace (pattern, replacement)
Returns a new string with part or all matches of a pattern replaced by a replacement
<br> e.g.<br>
<code>
Syntax

replace(pattern, replacement);
</code>

## String methods
Apart from array methods, string methods also provide in-built methods to manipulate strings.

## Iterative methods
### .forEach()
forEach method is used as a call-back function that accepts up to 3 arguements, that executes a provided function once for each array element
- value
- index
- arr

<br>e.g.<br>
<code> 
const numbers = [1, 2, 3, 4, 5];

*forEach function
function consoleItem (item), index, arr) {

  console.log(item);

  // expected to return 1 2 3 4 5

}

<br> 
*Arrow function

numbers.forEach((item, index, arr) => {

  console.log('a['+ index +'] = ' + item);

  // expected to return a[0] = 1 a[1] = 2 a[2] = 3 a[3] = 4 a[4] = 5

}); 

<br>
*Sum function using forEach method

numbers.forEach(item => {

  sum += item;

});
 
console.log(sum);

<br> function to check frequency

const letters = ['a','b','c','d','e','a','b'];

let count = {};

letters.forEach (item => {<br>
  if (count[item]) {<br>
    count[item]++;<br>
  } else {<br>
    count[item] = 1;<br>
  }

});

console.log(count);
</code>

### .map()
creates a new array populated with the results of calling a provided function on every element in the calling array


## API
Application Programming Interface
- provide a way for creating user code that utilises pre-built code to conduct various tasks.
## API Key & importance of its access
API key is used by multiple web APIs, that provide access control (for identification).
API key usually is related to the identification of API user also different rights (i.e.quota and authorisation area) that are open for access to the key
- applies to HTTPS for example

## Query String
General thumb of rule in URL:
protocal (HTTP/ HTTPS), location of file/ program (in form of host-name/ file-name) and query string

- length limitation
Try to limit the length of query strength (depends on the server ability to handle MAX 2000)
> The HTTP protocol does not place any a priori limit on the length of
   a URI. Servers MUST be able to handle the URI of any resource they
   serve, and SHOULD be able to handle URIs of unbounded length if they
   provide GET-based forms that could generate such URIs. A server
   SHOULD return <b>414 (Request-URI Too Long) status</b> if a URI is longer
   than the server can handle (see section 10.4.15).

## Use of API Key (with examples)

<code>
//use of concatanation to clean code <br>
var apiKey = 'trilogy'; <br>
var queryURL = "https://www.omdbapi.com/?t=dune&y=&plot=short&apikey=" + apiKey;
</code>

## API endpoint
APi endpoint is
Specific digital location where that allows communication and connections between sofeware programs (via exchange of code)
- requests for information are sent by one program to retrieve pre-existing digital resource 

>Sending request for information from web application/ server ➡ Receive response 

<b>Example : Instagram</b>

- business and creators endpoint that measure media and profile interactions
- moderation endpoint that regulate comments and replies
- discovery of hashtagged media 
etc.

## JSON
JavaScript Object Notation
it is a common format that data will be presented via an API.

## AJAX
Asynchronous JavaScript And XML. It is nota programming language but rather a technology <br>
It allows us to update web pages by exchanging data with a web server, without reloading the page

### .then() function

## Break into pieces
User input -> response -> output



