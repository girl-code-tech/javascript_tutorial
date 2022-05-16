# JavaScript Tutorial

1. It is interpreted, client-side (runs on user browser), event-based, OO scripting ( Scripting languages are those interpreted (X not compiled) languages which are directly converted to machine learning code.),  case senseitiv language.  
2. It was invented in 1995 at Netscape Corporation.


## What can Javascript do?
Javascript can:
  1. dynamically modify HTML content
  2. validate user input
  3. be used to create cookies
  4. full featured programming language
  5. not require user interaction with server for communication
  
  
## what makes JS Unique?
  1. Supported by all major browsers.
  2. Complex things are done easier
  3. Full integration with HTML and CSS

## Framework vs Library
Framework and Library has one difference that is 'inversion of Control'.
  1. Library : When we invoke some method from library, we are in control of the method. Let's say your senior developer has to provide Junior developer timer function then he can create a library to provide you that methods to be used.  Example: Angular, Jquery, Ext.js, Node.js, Aurelia.
  2. Framework: But when we use framework, the framework call us and control is inverted. Large code structure is converted to modules. Example: React, Ember.js, Vue.js, Polymer, Backbone.js


## Internal Javascript vs External Javascript
  1- Internal: JS can be inserted into documents using Script tag using which a block is created to write JS programs.
  2- External:  <script src='myscript.js'></script>

## Functions in JS
#### 1- alert()
      //alret user to tell him that something just happended. Example: 
      <script type="text/javascript">
        alert("Namaste Janab");
      </script>
#### 2- confirm()
      //opens up confirm/cancel dialog and returns true/false depending on user's click.
      <script type="text/javascript">
        confirm("Wanna Go Ahead?");
      </script>      
#### 3- console.log()
      //Writes information to the console of the browser. It is mostly used for debugging purpose. 
      <script type="text/javascript">
        console.log("Namaste Janab");
      </script>      
#### 4- document.write()
      //Writes directly to HTML document.
      <script type="text/javascript">
        document.write("Namaste Janab");
      </script>      
#### 5- prompt(msg,default)
      //creates a dialog for user input.
      <script type="text/javascript">
        confirm("Namaste" , "Janab");
      </script>

## Variables in JS
  1. Variables are containers which hold reusable data
  2. It is the basic unit of storage in program
  3. The value stored in a variable can be changed during program execution.

## Put and Get data from the HTML element
#### document.getElementById()
#### document.getElementByClassName()
#### innerHTML()

## String Concatenation
    <script>
      var x = "Hello Everyone"
      var y = "Everyone"
      var z = x+y
      alert(z);
    </script>

## Operators and Types of Operators in JS
##### Operator is a symbol that tells which operation to be performed.
### typeof()
    <p>The typeof operator returns the type of a variable, object, function or expression:</p>
    <p id="demo"></p>
    <script>
      document.getElementById("demo").innerHTML = 
      typeof "John" + "<br>" +
      typeof 3.14 + "<br>" +
      typeof NaN + "<br>" +
      typeof false + "<br>" +
      typeof [1, 2, 3, 4] + "<br>" +
      typeof {name:'John', age:34} + "<br>" +
      typeof new Date() + "<br>" +
      typeof function () {} + "<br>" +
      typeof myCar + "<br>" +
      typeof null;
    </script>

### delete
    <p>The delete operator deletes a property from an object:</p>
    <p id="demo"></p>

    <script>
    const person = {
      firstname:"John",
      lastname:"Doe",
      age:50,
      eyecolor:"blue"
    };

    delete person.age;

### in 
    <p>The in operator returns true if the specified property is in the specified object:</p>
    <p id="demo"></p>
    <script>
    const cars = ["Saab", "Volvo", "BMW"];
    // Objects
    const person = {firstName:"John", lastName:"Doe", age:50};
    document.getElementById("demo").innerHTML =
    ("Saab" in cars) + "<br>" + 
    (0 in cars) + "<br>" +
    (1 in cars) + "<br>" +
    (4 in cars) + "<br>" +
    ("length" in cars) + "<br>" +

    ("firstName" in person) + "<br>" +
    ("age" in person) + "<br>" +

    // Predefined objects
    ("PI" in Math) + "<br>" +
    ("NaN" in Number) + "<br>" +
    ("length" in String);
    </script>
    
### instance of
    <p>The instanceof operator returns true if the specified object is an instance of the specified object.</p>
    <p id="demo"></p>
    <script> 
    const cars = ["Saab", "Volvo", "BMW"];
    document.getElementById("demo").innerHTML =
    (cars instanceof Array) + "<br>" + 
    (cars instanceof Object) + "<br>" +
    (cars instanceof String) + "<br>" +
    (cars instanceof Number);
    </script>

 ### void: The void operator evaluates an expression and returns undefined. This operator is often used to obtain the undefined primitive value, using "void(0)" (useful when evaluating an expression without using the return value).
    <p>
    <a href="javascript:void(0);">Useless link</a>
    </p>

    <p>
    <a href="javascript:void(document.body.style.backgroundColor='red');">
    Click me to change the background color of body to red.</a>
    </p>

## How to get the data using promt function
    <body>
      Name: <i id="result"></i>
      <br/>
      <button onclick="call()">Call</button>
    </body>
    <script type="text/javascript">
      function call(){
      var name = prompt("Hey, what's your name", "");
      document.getElementById('result').innerHTML = name;             
      }
    </script>

## Array in JS
Group of data stored in contiguous memory location.
Declaration of array in JS: 
#### Method1
    var house = []
    var house = ["1BHK", "2BHK", "3BHK"]
    house[0] = "1BHK"
    house[1] = "2BHK"
    house[2] = "3BHK"
#### Method2
    var house = new Array()
    var house = new array("1BHK", "2BHK", "3BHK")
    var house = new array(10,20,30)
#### Code
    <script type="text/javascript">
	var cars = [];
	cars = ["my_car" , "your_car" , "his_car"];
	document.write(cars[1]);
	document.write("<br/>");

	var car = new Array();
	car = ["my_car" , "your_car" , "his_car"];
	document.write(car[2]);
    </script>
   
## Loop in JS
	<script type="text/javascript">
	for (var count=10; count>0; count--)
	{ document.write(count+"<br/>");}
	document.write("Loop Ended");

	</script>
	
## While Loop
	<script type="text/javascript">
	var i = 0;
	while (i < 10)
	{ document.write(i+"<br/>");
	i++;
	}
	document.write("Loop Ended");
	var i = 10;
	while (i > 0)
	{ document.write(i+"<br/>");
	i--;
	}
	</script>
1. execute code block as long as condition is true, but once the condition becomes false, the loop terminates
2. also called entry control loop
	
