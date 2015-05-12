Melvin's JavaScript Studies
===

# Overview:

JavaScript is a programming language that is **interpreted** ...
  
#Structure:

* JavaScript is case sensitive
* 
* Always end with a semi colon;
* 
* Position of javascript really matters
* 
* Execution Order
* 
* Javascript reads from top to bottom


# Variables


## Variable Declaration & Initialization


````javascript
var name = "Melvin";
````
`````
var money = "Dollars"; 
````


Variables are:

* Like a container that holds food
 
* the way we hold things in memory 

# 6 different types of variable data

#### text string
#### arrays
#### objects
#### floating number point 
#### boolean value
#### dates


### conditional code:



Must evaluate if true or false


Ex.

  if (condition){
  
  (what we will do if true);
  
 
  }
  
  else {


### operators and expressions:

- =  means assigning a value 
- ==  equality
- ===  strict equality, not just equal also identical



#### unairy operation prefix and postfix 

a++ increments by 1

--- one thihng to act on a++, 




### Tenary Operator

Ex.

condition ? true : false 


var player1 = 500;
var player2 = 600; 


var highscore

if 
(player1 > player2){
    highscore = player1;
}
 else{highscore = player2;
 }

var highscore = (player1 
> player2) ? player1 : player2; 



## console.log 
 - not apart of js language 
 - something firebug brought tot the table
 - we can write a message to the cconsole ass well as a string or variables
 
 



## loops 

check conditions before entering the loops.

Ex. 

var a = 1;
while (a<10) {
console.log(a);
}
}
* adding a++ will evalute to false and go to the nextline of code

## Functions 

function name () {
 console.log("we're in the function");
 
 function Myotherfunction(){
        ///lots of code
        ///lots of code
        }
 }
 
 ##Ex.
var a = 100

do{

 
 
 

function myfunction();

function myfunction(x,Y){
   my var = x



for (var i =l; i<10; i++{
//some code//
////
}





















## Arrays

 - To tell javascript that theres an arrays 
 use brackets.
- [ ] indicate that array.

- Zero based index 
- First number is 0 not 1






## Strings 

- strings can have either double quotes or single qoutes
"" or ''.

* console.log (phrase.length);

 split
 
 Ex. 
  
  var phrase="this is a simple phrase.";
  var words= phrase.split("");
  
  var position = phrase.index("")
  var segment = phrase.slice(6,5);
  var phrase = "yet another phrase".; 



* sort order means all uppercase letters are less than lower case.





##Numbers

-Javascript numbers are 64 bit floating numbers

can be 



Math.max()
math.min()
math.random()
math.log()
math.pi()
math.sqrt()




Dates

### Date commands

- today.getMonth(); // returns 0-11
- today.getFullYear(); // 2015
- today.getDate(); // 1-31
- today.getDay(); // 0-6 days of the week. 0 === sunday
- today.getHours; // 0-23
- today.getTime; // milliseconds since 1970



## Objects 

* arrays can be ojects a new date 
functions belong to objects 

* container that gathers together some data and some behaviors
*

####Object Creations

--outside of objects id considered a variable
inside is called properties




# The (Dom)
 --- dom stands for document object model
  -- agreed upon set of terms that describes exactly how to interact with pieces of a webpage.
 
 
 ##The dom allows us to:
 
* get the title text
* get the second paragraph tags
* get the third link in the menu and set its css to display:none
* get all the (li) elements in the last ordered list
 
* the way to reach into the page from out script
 and the way our page can reach into our script.
 
 
 
 ## Get Elements
 
-getElementById("someid")
 
 -to grab hold of id, use the statement above.
 
 This is an example of of 
 
 Var MyElement=document.getElementById()
 
 
 Don't have an Id for the element im after/ or want more than one Element.
 
  *document.getElementsByTagName("a"); *
 
If the a above doesn't exsit, will return an array, but the array will be empty.
 

 *var limitedList=myFirstLisst.getElementsByTagName("li")*
 
#### To grab code from inspect element

Var mainTitle=document.getElementById("mainTitle");

console.log (This is an Element of sometype: mainTitle.innerHTML);)
 console.log("childnodes:",mainTitle)
 
 
 ## Changing Dom Content
 
 - Create the Element
 - add it to the document
 
 
     var my NewElement=document.createElement("li");
     
     myElement.appendchild(myNewElement);
     
     myNewElement.innerHTML="Newitemtext";
 
 ---creating text nodes--
 
  varMytext=document.createTextNode("NewListItemText")
  MyNewElement.appendChild(mytext);
  
  alternatives to appendChild

parent.insertBefore(newElement,existingElement);

(
 
 
 
  ### Step One
  
     get element , change attribute
     myElement.getAttribute("align");
     myElement.setAttribute("align", "left");
 
 

     
 
 
 # Events and Event Listeners
 
 What is an Event ?
 
 -Something thats already happening
 --Move of mouse or Clicking on the browser
 
 ###Event Names
 
* onload
* onclick
* onmouseover
* onblur

Ex. 
 
 Handling Events Methods1
 
 <button onclick="alert("hello,world;")>Run Some Javascript</button>
 
 Handling methods 2
 
 myelement.onclick=function(){
  // your event code handler code
  //
 };
 
 
 Handling methods 3
 
 document.addEventListener
 ("click, myfunction, false");
 
 document.addEventListener('click,anotherfunction, false')
 document.removeEventListener('click, anotherfunction, false);
 
 
 ## Click N Load
 
 Ex.
 
 document.onclick=function(){
  alert("you clicke somewhere in the document");
  
 }

 
 Ex. for image
 
 var myImage=document.getElementById("mainImage");
 myImage.onclick=function(){
 alert("you clicked the image");
  }
  
  
  ## Focus Blur
  
  
 
* onfocus means check into  it
* onblur means to click out always called

* onchange onkeypress onkeydown or onkeyup 

  
  <inputtype="text" value="youremail" name="email" id="email"
  tabindex="20"/>
  
  var emailField=document.getElementById("email");
  
   emailField.onfucus=function(){
    if(emailField.value=="youremail"){
    emailField.value=" ";
    }
   };
   
   the value is your email, leaves qoutes blank
   
   
   emailField.onblur=function(){
   if(emailField.value==""){
   emailField.value="your email";
    }
   };
   
   
#Timers

- Working with timers in Javascript really boils down to these
four methods:

setTimeout
  --perform single acton after delay
  
setInterval
  --Repeat after fdelay and jsut keep on repeating
   
cleaTimeout
clearInterval



setTimeout(simpleMessage,5000);
just happens once

setInterval(changeImage5000);
changes image every 5 seconds


var myImage=document.getElementById("mainImage")
var imageArray=["images/overlook.jpg",];

var imageIndex=0;


function changeImages(){
myImage.set Attribute("src"imageArray[imageIndex]);
imageIndex++;
if(imageIndex>= imageArray.length){
  imageIndex=0;
  }
}  

 * Once Set Interval was set it continues to repeat its function.
 
 var internalHandle=setInterval(changeImage,5000);
 
 myImage.onclick=function(){
 
 clearInterval(intervalHandle);
 
 }

#Enhancing forms with javascript

working with forms we care about

- field values
- field events

The most common form Element is

Textfield

 - has a value property, either get it or set it
 main property
 myTextField.value
 
 
 dealing with select list 
 
 Myselect.type
 (selcet-one or select-multiple)
 
 myselect.selectedIndex 
 
 mySelect.Opton[x].selected
 (true or false)
 
 main event on change
 
 #Form Events
 
one main event of the form is onsubmit/ in other words
" send or submit " 

# Prevent Submit

window.onload=function(){
 prepareEventHandlers();
}


// handle the form submit event

funtion prepareEventHandlers(){
 document.getElementById("fromContact").onsubmit=function(){
 //prevent a form from submitting if no email
if(document.getElementById("email").
document.getElementById("errorMessage").innerHTML=please provide at least 
an email address!";
//to stop the form from submitting
return false;
}else{
//reset and allow the form to submit
document.getElementById("errorMessage").innerHTML="";
return true;


#Style Intro


myElementStyle.color="red";
myElement.Style.left="40px";

myElement.Style.backgroundRepeat="repeat"-x;

''example
  {
 width:230px;
 color:#fff;
 font-weight:bold;
 background-color:#193742;

}
