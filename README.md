# Topics

[History](README.md#history)    

# History

- Brendan Eich first created it, it was actually called Livescript, and then Microsoft decided to try and reverse engineer the program and they ended up with something called Jscript.
- The Europeans do best and they standardize the language and that's where you get the ECMAscript from and that stands for European Computer Manufacture Association(ECMA)
- That's what the version name comes up with ES6 or ES7 and not as JS6 or JS7.

# Java vs JavaScript

- Interpreted Language-> JavaScript, Python and Ruby
- Compiled Language-> Java, C/C++, Swift

# Interpreted Languages 

- They weren't so powerful.
- They were very slow and they execute all the instructions line by line.

# Compiled Languages

- They are more serious language and you end up with very fast running programs.

# JavaScript

- High level, interupted programming language.(High level - memory management on the machine, Interupted - no compiler simply a Scripting Language)
- Conforms to the ECMAScript specification.
- Multi-paradigm.(We can write code that in many ways (i.e) Object Oriented, Functional)
- Runs on the client/browser as well on the server(Node.js)
- JavaScript is used for both front end and back end development. 
- While you can use other languages that can be compiled in to JavaScript and run on the browser.

# Why JavaScript

- It is the Programming language of the browser.
- Build very interactive user interfaces with frameworks like React.
- Used in building very fast server side and full stack applications.
- Used in Mobile Development(React Native, NativeScript and Ionic)
- Used in desktop application development(Electron JS) 

# Adding Behaviour to Websites

- Inspect -> console
```ruby
alert("Hello World");
console.log("Hello World");
console.warn("Hello World");
console.error("Hello World");
```
- Sources -> >> -> Snippets -> Create index.html -> Run at the Bottom.
```ruby
alert("Hello");
```
__where,__
- alert -> Function
- Hello World -> Message
- ; -> End

# Data Types

- Primitive data types(i.e)directly assigned to memory.
- Strings, Numbers, Boolean, null, undefined and ES6-> Symbol

```ruby
const name = "Android";
const age = 10;
const rating = 4.5;
const isGood = true;
const x = null;
const y = undefined;
let z;

console.log(typeof name, typeof age, typeof rating, typeof isGood, typeof x, typeof y, typeof z);
console.log(name, age, rating, isGood, x, y, z);
```

# Variables

- var, ES6-> let, const 

# var

- The scope of a variable defined with the keyword “var” is limited to the “function” with in which it is defined. 
- If it is defined outside any function, the scope of the variable is global.
- var is “function scoped”.

```ruby
var age = 20;

age = 22;

console.log(age);
```

# let

- The scope of a variable defined with the keyword “let” or “const” is limited to the “block” defined by curly braces i.e. {} .
- “let” is “block scoped”.

```ruby
let age = 20;

age = 22;

console.log(age);
```

# const 

- The scope of a variable defined with the keyword “const” is limited to the block defined by curly braces. - However if a variable is defined with keyword const, it cannot be reassigned.
- In other words, “const” cannot be re-assigned to a new value. However it can be mutated.
- “const” are “block scoped”.

```ruby
const age = 20;

age = 22;

console.log(age);
```

# Block Scope

- In Javascript you can define a code block using curly braces i.e {}.

```ruby
{
    var a=10;
    console.log(a);
  } //block 1
  {
    a++;
    console.log(a);
  } //block 2
```

# Function Scope

- In Javascript you limit the scope of a variable by defining it within a function. This is known as function scope.

```ruby
{
    var a=10;
    console.log(a);
  } //block 1
  {
    a++;
    console.log(a);
  } //block 2
```

# String Concatenation

```ruby
const name = "Android";

console.log("My Name is"+ " "+name);

```

# Template String

```ruby
const name = "Android";

console.log(`My Name is ${name}`);

```
# String Length

```ruby
const name = "Android";

console.log(name.length);
```

# String UpperCase

```ruby
const name = "Android";

console.log(name.toUpperCase());
```

# SubString

```ruby
const name = "Android";

console.log(name.substring(0,2));

```

# Split Array

```ruby
const name = "Android";

console.log(name.split(''));
```

# Split by using Comma Space

```ruby
const name = "Android, iOS, Flutter";

console.log(name.split(', '));
```

# Slicing

```ruby
const name = "Android";

console.log(name.slice(0,3));
```

# Array

- Variable that hold multiple values.

```ruby
const mArrayNames = new Array('Android', 'Flutter', 'iOS', 'ReactNative');

console.log(mArrayNames);
```

- JavaScript is not a Statically typed Language.

```ruby
const mArrayNames = new Array('Android', 'Flutter', 'iOS', 'ReactNative', 5, true);

console.log(mArrayNames);
```
```ruby
const mArrayNames = new Array('Android', 'Flutter', 'iOS', 'ReactNative', 5, true);

console.log(mArrayNames[1]);
```

```ruby
const mArrayNames = new Array('Android', 'Flutter', 'iOS', 'ReactNative', 5, true);

mArrayNames[2] = 'Java';
```

- The push() method adds new items to the end of an array, and returns the new length.

```ruby
const mArrayNames = new Array('Android', 'Flutter', 'iOS', 'ReactNative');

mArrayNames.push = 'Java';
```

- The unshift() method adds new items to the beginning of an array, and returns the new length.

```ruby
const mArrayNames = new Array('Android', 'Flutter', 'iOS', 'ReactNative');

mArrayNames.unshift = 'Python';
```

- The pop() method removes the last element of an array, and returns that element.

```ruby
const mArrayNames = new Array('Android', 'Flutter', 'iOS', 'ReactNative');

mArrayNames.pop();
```

- To check the Array List is Available

```ruby
const mArrayNames = new Array('Android', 'Flutter', 'iOS', 'ReactNative');

console.log(Array.isArray(mArrayNames));
```
- To get the index of ArrayList

```ruby
const mArrayNames = new Array('Android', 'Flutter', 'iOS', 'ReactNative');

console.log(mArrayNames.indexOf('Flutter'));
```
- The includes() method determines whether an array contains a specified element.

```ruby
const mArrayNames = new Array('Android', 'Flutter', 'iOS', 'ReactNative', 5, true);

console.log( mArrayNames.includes('Android'));
```

# For Round-Off  Values

```ruby
const rating = 4.5;

console.log(Math.floor(rating));
```
```ruby
const rating = 4.5;

console.log(Math.round(rating));
```

# Functions


# Random Number Generation

- For, Random Number Generation(0 - 0.999999999999)

```ruby
var n = Math.random();
```

- Simple Random Number calculation for roll dice,

```ruby
var n = Math.random();
n = n * 6;
n = Math.floor(n) + 1;
console.log(n);
```

# Control Statements

- Using if, else

```ruby
if(condition){

}else{

}
```
- Using while Loops

```ruby
var i = 1;

while (i < 20) {
  console.log(i);
  i++;
}
```

- Using For Loops

```ruby
for(var i = 1; i < 20; i++){
    console.log(i);
}
```
# Comparators and Equality

```ruby
=== - Is equal to ( === this will compare different data types)  
!== - Is not equal to  
>   - Is greater than  
<   - Is lesser than  
>=  - Is greater than or equal to  
<=  - Is lesser than or equal to  
```

# Combining Comparators

```ruby
&& - AND  
|| - OR  
!  - NOT  
```

# DOM Events

- The onload event occurs when an object has been loaded.

```ruby
object.onload = function(){myScript};
```

# Inline JavaScript

```ruby
<body onload="alert('Hello');">
    <h1>Hello</h1>
</body>
```

# Internal JavaScript

```ruby
<body>
    <h1>Hello</h1>
    <script type="text/javascript">
        alert('Hello');
    </script>
</body>
```

# External JavaScript

__In index.html__

```ruby
<body>
    <h1>Hello</h1>
    <script src="index.js" charset="utf-8"></script>
</body>
```
__In index.jss__

```ruby
alert('Hello');
```

# DOM(Document Object Model)

- Dominating the DOM to add functionality to HTML Elements.
- In Simple terms, JavaScript can access all the elements in a webpage making use of Document Object Model (DOM).
- It basically the web page converted in to the individual objects that we can select and manipulate.
- Converting HTML file in to the DOM is done by the browser when you load the web page.
- It turns each of the elements and their associated data in to a tree structure with a whole bunch of objects that you can select and Manipulate.


- The above tree model is usually how you'll DOM represented.
- You can see all of the elements in our HTML has been converted in to Objects, and their relationships to each other in the tree diagram.

- In JavaScript everything is under document.

```ruby
document
```
- html section,
```ruby
document.firstElementChild;
```
- head section,
```ruby
document.firstElementChild.firstElementChild;
```
- body section,
```ruby
document.document.firstElementChild.lastElementChild;
```
- To change the Text of the Element,
```ruby
document.document.firstElementChild.lastElementChild.innerHTML = 'Good Bye';
```
- To change the Text color of the Element,
```ruby
document.firstElementChild.lastElementChild.firstElementChild.style.color = 'red';
```
- To click button Element using querySelector,
```ruby
document.querySelector('button').click;
```
- Objects inside the DOM(Eg: Button) have Properties and Methods
- Here, Properties describes something about the object.
- Methods are the things that the object can do.


# Knowledge Transfer

# High Level Language

- It is programmer friendly language.
- High level language is less memory efficient.
- It is easy to understand.
- It can run on any platform.
- It is simple to maintain.
- It is simple to debug.
- Java, JavaScript, Python

# Low Level Language

- It is a machine friendly language.
- Low level language is high memory efficient.
- It is tough to understand.
- It is machine-dependent.
- It is complex to maintain comparatively.
- It is complex to debug comparatively.
- Machine, Assembly and Compiler

# Program for Fibonacci Series

```ruby
var n = 99;

function fibonacciGenerator(n) {
  var output = [];
  if (n === 1) {
    output = [0];
  } else if (n === 2) {
    output = [0, 1];
  } else {
    output = [0, 1];

    for (var i = 2; i < n; i++) {
      output.push(output[output.length - 1] + output[output.length - 1]);
    }
  }

  return output;
}

output = fibonacciGenerator(n);
console.log(output);
```
# Program for Leap Year

```ruby
function isLeap(year) {
  if (year % 4 === 0) {
    if (year % 100 === 0) {
      if (year % 400 === 0) {
        return console.log('Leap Year');
      } else {
        return console.log("Not Leap Year");
      }
    } else {
      return console.log("Not Leap Year");
    }
  } else {
    return console.log("Not Leap Year");
  }
}

output = isLeap(2000);
```

# Note

- We can disable JavaScript in browser -> Settings -> In Search Bar type javascript -> Site Settings ->
JavaScript(Allowed) -> dis-allowed over there.

# Reference

- https://github.com/rwaldron/idiomatic.js/ (For Code Styling)
- https://chrome.google.com/webstore/detail/html-tree-generator/dlbbmhhaadfnbbdnjalilhdakfmiffeg (HTML Tree Genarator)





