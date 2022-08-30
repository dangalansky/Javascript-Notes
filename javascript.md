javascript!

	keywords/methods

	•	var —> defines variable, stores data
	⁃	ex) var myName = ‘Angela’
	⁃	ex) var yourName = prompt(‘What’s your name?’)

	•	console.log()—for developer! prints something inside console
	⁃	for developer to see

	•	alert() —> creates a popup with message
	⁃	for user to see
		ex) alert(‘Hello World’);

	•	prompt() —> popup that requires user input

	•	typeof()—>returns datatype

	•	.length —>returns integer with number of characters in a string
	⁃	ex) myName.length - returns(6)

	•	.slice(start, stop)—> does not include stop
	⁃	ex) myName.slice(0,3) —> “Ang”

	•	.toUpperCase()//.toLowerCase()—>when applied to string, changes to uppercase/lowercase
	⁃	ex) myName.toUpperCase() —> ANGELA

	•	setTimeout(ms)

  •	onload —> when page loads…something happens
	⁃	<body onload=“alert(‘Hello’);”>


	mathematics
	•	precedence determined by parenthesis
	•	* multiply
	•	/ divide
	•	+ addition
	•	- subtraction
	•	% modulo —> returns only the remainder

	•	++ —> increment expression
	⁃	ex) x = 5; x++; —> 6 (means x = x+ 1)
	⁃	C ++ (meant to be a joke! C + 1)
	•	- - —> decrement expression
	⁃	ex) x = 5; x - -; —> 4 (means x = x - 1)
	•	+= —> on it’s own, + 2 but also can be used to add another value
	⁃	ex) x = 5; x+=; —> 7
	⁃	ex) x = 5, y = 3; x += y; —> 8
	•	-=, *=, /= —> all the same!!!


	•	parseFloat() —> converts string to floating point

	•	Number() —> converts string to integer

	•	Math.floor() —> rounds number down to nearest integer 

	•	Math.pow(base, exponent) —> for exponents
	⁃	ex) Math.pow(2, 4) —>16

	•	Math.round(number) —> rounds up or down if decimal is higher or lower than 5. 

	•	Math.random()—> returns a 16 digit number between 0 and 0.9999999999
	⁃	ex) to return random number between 1 and 6?
	⁃	
	⁃	* +1 because it will never hit 6!!! 



	
	if/else (conditionals/control flow)
	format:
	•	if (track  ===  “clear”) {
		goStraight();
	} 
	else if {
		turnRight();
	} else {
		turnLeft();
	}

	comparators 

	•	=== is equal to (checks for equality in value and datatype)
	⁃	vs. == (checks for equality, doesn’t care about datatype)
	•	!== is NOT equal to
	•	> is greater than
	•	< is less than	
	•	>= is greater or equal to
	•	<= is lesser or equal to

	combining comparators
	•	&& and
		ex) if (loveScore > 30 && loveScore <= 70) {
	alert(“Your love score is ” + loveScore + “ %”);
                 }
	•	|| or
	⁃	ex) if (loveScore > 30 || loveScore <= 70) {
	alert(“Your love score is ” + loveScore + “ %”);
                 }

	•	! NOT	

	While Loops:
	* checks for a state; WHILE something is true

while (something is true) {
	//Do something
}
	
	For Loops:
	* used to iterate code over a fixed number of times

for (i=0; i<2; i++) {
	//Do something
}
	-i=0; —> start
	-i<2; —> end
	-i++; —> change

	Switch Statement
* like if/else, for more complex variables

switch —> what is switched on
case—> what should happen
break —> code is exited if case occurs
default —> what happens else wise?

ex)
var buttonInnerHTML = this.innerHTML;

switch (buttonInnerHTML) {

      case “w”:
		var audio = new Audio(“sound/tom-1.mp3”);
		audio.play();       
        	break;

      default: console.log(buttonInnerHTML);
		        
}


	arrays

	•	var array = [ ]; 
	⁃	establish empty array

	•	array.push(1, 15, 82, 25);
	⁃	add element(s) to array
	⁃	pushes to end of array

	•	array.pop();
	⁃	removes last element from array

	•	var fifteen = array[1];
	⁃	pull element from array

	•	array.length; —> 4
	⁃	return length of array

	•	console.log(array) —> (4) [1, 15, 82 ,52]
	⁃	print array in console
	 *printing in console always gives length first!

	•	array.includes(83) —> returns Boolean
	⁃	in this case false!!!

	•	checking if value NOT in array!
	⁃	if(!array.includes(83)) 




	functions

creating the function:
function getMilk() {
	alert(“leave house”);
	alert(“turn right”);
	alert(“go straight”);
}
	-note: semi-colon not used to close a function def!

calling the function:
getMilk();

functions with INPUTS:
function getMilk(bottles) {
	alert(“leave house”);
	alert(“turn right”);
	alert(“buy” + bottles + “of milk”)
	alert(“go straight”);
}

calling the function:
getMilk(2); —> “buy 2 bottles of milk”

functions the return an OUTPUT:
function getMilk(money) {
	return money % 1.5; 	
}
	*this function will return the amount of change one would receive after buying a certain amount of milk

calling the function and saving it in variable:
var change = getMilk(4); —> 1


	Higher order functions

ex)
function add (num 1, num 2) {
	return num1 + num 2; 
}
function calculator (num 1, num 2, operator) {
	return operator (num 1, num 2);
}
calculator(2, 3, add);

ex) 
document.addEventListener(“keydown”, respondToKey(event));

function respondToKey(event) {         <———— *callback function
	console.log(“Key Pressed”);
}

		




	datatypes
	•	string—> text, not interpreted as code. denoted by “string”
	•	number
	•	boolean—> true, false

	syntax
	•	concatenation—> to add strings to variables use “” and +
	⁃	ex) alert(‘My name is’ + myName + “, welcome” + yourName);
	•	notes —> add 2 forward slashes before code
	⁃	ex) //Hey look i am a note


	variable naming conventions

	1.	give variables meaningful names
	2.	assume someone else will need to read code and understand!
	3.	no keywords (ex. var)
	4.	cannot begin with number
	5.	no spaces
	6.	can only contain letters, numbers, $, and _ (no other symbols!)
	7.	camel casing (first letter lowercase, every next word begins with uppercase letter)

	DOM (Document Object Model)
		*catalogs website into individual objects to be manipulated

	•	Objects have:
	⁃	properties
	⁃	getting —> car.color;
	⁃	setting —> car.color = “red”;
	⁃	methods
	⁃	a function but specific to an object!
	⁃	calling —> car.drive();

	•	getElementsBy…
	⁃	Tag
	⁃	Class
	⁃	returns array but can be tapped into using []
	⁃	ex) document.getElementsByTag(‘li’)[3].style.color = “red”;

	•	querySelector()
	⁃	just like CSS styles
	⁃	only returns first element
	⁃	Elements —> just name
	⁃	ex) document.querySelector(‘h1’);
	⁃	Classes —> .
	⁃	ex) document.querySelector(‘.btn’);
	⁃	Id’s —> #
	⁃	ex) document.querySelector(‘#title’);
	⁃	or…can combine!
	⁃	ex) document.querySelector(‘li.item’);
	⁃	no space if within same element
	⁃	ex) document.querySelector(‘li a’);
	⁃	must space between selectors if not within same element!

	•	querySelectorAll()
	⁃	returns array of all occurrences

	Text Manipulation

	•	innerHTML; —> affects all html inside elements selected
	⁃	ex) document.querySelector(“h1”).innerHTML = “<em>Hello</em>;

	•	textContent; —> only affects the text. Better for targeting if you don’t want to affect stylings!
	⁃	ex) document.querySelector(“h1”).textContent; —> “Hello”

	Attribute Manipulation
		*everything inside HTML tag besides tag itself: “href”, “src”, “class”, “type” etc…

	•	attributes —> returns list of attributes for an element
	⁃	ex) document.querySelector(‘a’).attributes; —> NamedNodeMap {0: href, href: href, length: 1}

	•	getAttribute(“attribute”) —> returns specified attribute
	⁃	ex) document.querySelector(‘a’).getAttribute(‘href’); —> “https://www.google.com”

	•	setAttribute(“attribute”, “newContentForAttribute) —> changes attribute content to specified
	⁃	ex) document.querySelector(‘a’).setAttribute(“href”, https://www.bing.com”);


	Separation of Concerns (Keeping CSS to itself)
		*how to keep CSS outside javascript

	•	classList —> returns list of CSS classes
	⁃	ex) document.querySelector(“button”).classList; —> DOMTokenList [“btn”, value: “btn”]

	•	create CSS classes to trigger certain behaviors!
	⁃	classList.add(“className”)
	⁃	classList.remove(“className”)
	⁃	OR
	⁃	classList.toggle(“className”)
	⁃	returns true or false each time it’s triggered

	Event Listeners

	•	addEventListener(“eventToListenFor”, functionWithoutParentheses);
	⁃	ex) document.querySelector(“button”).addEventListener(“click”, handleClick);

		OR

	•	anonymous functions
	⁃	ex) document.querySelector(“button”).addEventListener(“click”, function ( )  {
				alert(“I got clicked!”);
			} ); <— for anonymous functions! don’t forget this closing parenthesis + semi colon!!!

	•	this
	⁃	returns identity of trigger
	⁃	ex) document.querySelector(“button”).addEventListener(“click”, function ( )  {
	⁃	console.log(this); —> <button class=“a drum”>a</button>
	⁃	console.log(this.InnerHTML); —> a
	⁃	 OR in LOOP of a list of elements
	⁃	this.style.color = “white”;

		JS Objects

* create an object
var bellBoy1 = {
	name: “Timmy”,
	age: 19,
	hasWorkPermit: true,
	languages: [“French”, “English”]
}

* tap into specific properties
alert(“Hello, my name is ” + bellBoy1.name)

* Constructor Function —> creates objects!, 
	**denoted by use of double capital letters, just like Classes in PY

function BellBoy (name, age, hasWorkPermit, languages) {
	this.name = name;
	this.age = age;
	this.hasWorkPermit = hasWorkPermit;
	this.languages = languages;
	this.pickUpLuggage = function() {
		alert(“Luggage being moved!”);
	}
}

* Initialize Object from function!

var bellBoy1 = new BellBoy(“Timmy”, 19, true, [“French”, “English”])

* Calling method or property from object

bellBoy1.pickUpLuggage(); —> alert(“Luggage being moved!”)
bellBoy1.name —> “Timmy”

