# JavaScript

*** import javascript with <script src="app.js"></script>
place inside <body>

methods are fancy functions. exists on an object.

first letter of first word lower cased, any subsequent word first letter is capitalized. example: turkeysGobbled

everything is an object in javascript

in booleans 0 is falsy and any other number is truth
anything undefined is falsy

null is for purposefully not assigning a value

reference data-types, vs primitive
in primitive: 0, null, undefined = falsy
empty array or objects are still truthy

arrays are a collection of things

push changes the value 

key value pairs is like a hashmap

objects and parameters are black magic

event listener (on click)

***start every function with a console.log can help with debugging

don't forget to evoke a function () without that, it wont do anything

if you get undefined, there might be a typo in the variable/function name between your HTML vs Javascript 

+ doesn't reassign value += does

{} object 
[] array

function(variable) variable can get defined this way, acts as if we said let variable

return ends it at that point in the code line so it wont continue on
return instead of else is actually most efficient for checking conditions

const nameOfCopy = { ...whatsBeingCopied} copies another const without changing variables to the original if changes are made to the copy

concatination

functions must be evoked ()

find is like a for-loop with an if statement

'' string.. no quotes it looks for a variable


** multiply multiple squares the number

p tag around animal emoji

window + v gives your paste history clipboard

|| creates an or statement


in querySelector
'#' grabs by id
. is a selector

setInterval to make time counters
setTimeout delays the execution of a function by the time that is set (in milliseconds) once

localStorage to save information, for a scoreboard  ((can check on storage in Application))

parseInt converts string into integer
toString makes integer into string

shift moves one over in the array. You can shift to change across an array (takes something off the front)
push adds an item to the end... create a change function, give their health back & push them to the back of the array with updated stats

uniqueInfoFromArr.find    (find grabs the whole object out of an array by the unique identifying aspect)

******for testing you cant adjust your code

research more about =>

document.getElementById(array.identifier)

classList allows you to edit within a class tag in the element that you have grabbed 
personElm.classList.remove('d-none')
instead of remove you can toggle

math.round rounds a number so you wont have decimals


*ANCHOR MVCS Pattern:
Model; blueprint of what data will look like
View; html representation of the data.. interacts with the controller
Controller; takes in actions from user draws data to dom,,, interface between view & project
service; any thing that modifies data goes here. determines what controller input does
appstate; single source of truth, where all apps data will be stored

*****bcw create
mvc      (first one)
name it
yes to initialize git repository

html, app.js, assets->style->style.css  
models (create new file.js)
appstate

settings import with .js

Export class to make it accessible by other JS documents. to link, go to JS you want it, type out the name of the class & its the orange one

can import & export whatever. but putting it in a class bundles it

app.js is the JS that interacts with the HTML. everything imports to that. it talks to the other JS files. so to console log a function in a JS other than app will have to reference app.otherJSfile.yourFunction() 
example from lecture: app.charactersController.testFunction()

changing data is confined to the business layer 
controller; flexible
service; not flexible

new is how you invoke a class, so when you input data for a character its a new character
creating an instance of a class

app -> controller -> function were calling

service uses but doesn't change info
bring in, but don't change in the controller

talking to code inside your score requires this.

app is what is there when the page starts, opens the door
appState is the current state


html -> controller -> 
appState -> controller

<!-- SECTION more MVC -->

|| is or
this.color = color || 'normal'
your custom value needs to come first

step 1 what does out data look like.. Models, make your class
step 2 create data.. AppState, new (classname) build out data for the class
step 3 draw data.. controller, build constructor -> app.js 


router houses the 😎 button
can set view in router that links the button to null so it wont load anything, but the about page wornt work anymore

# in URL makes it a new section in the webpage, not a brand new webpage


activeGachamon = null (set as no starting value becasue it will be added later when button is clicked)

service exports a const of itself
controller & model export the class

controller can take in & then pass function without changing it
when passing references it is a good practice to use the same name, it can be changed but makes it confusing

'get' accessor must 'return' 

when you operate on null you wont have intellicense because the code doesnt know that they will be code there later
@type {gachamon} tells the function what it is going to be after data is put into it, so you have intellicense again

under utils -> generateId; generateID() 
 you must open the file or it wont know it exists

get a getter runs when it is gotten. calculates as you get it.. good for values that fill in templates

observer pattern, lets you watch something & trigger something else when the observed changes.
set up controller to watch & then alert draw to run on its own when code that needs drawn changes
appState.on('activeGachamon', this.draw)  it is just giving instructions, dont invoke instructions

splice can be used to swap info in an array with the 3rd value input

splice is destructive because it can change the origional

emit forces observer to witness an event, even if it didnt occur


Change state in the service!!

view is a container for your html buildout of what it should look like

views can be real HTML

for forms use onsubmit, not onclick
you have to set button type="submit"

when you submit a form it tries to take you to a new page. to stop it
event.preventDefault()

you can allow the code to know what form its intaking by doing a name tag name="className"

if its a number it wont have "" if its a string it will have ""

utils -> store.js
saveState('yourInfo', AppState.yourInfo)

json stringify; string that looks like an object. put objects into a string & pull it out of the string as an object

utils -> Pop.js makes a nice popup that looks better than the window.confirm

windows pauses code before it continues, but Pop doesn't

async functions have the ability to wait
await; will have the code wait until it has recieved input before it continues
you can await anything that has a promise 

<input class="stuff here" required              (required makes it so you cant submit a form until that is filled out)

ON GitHub, fork creates a copy of their repository into yours
click green code dropdown -> HTTPS -> copy -> powershell -> your project forlder -> git clone (paste URL (has to be your username))
Run the git clone <paste the URL here> command and paste the URL you copied from GitHub without the angle brackets


/** 
* @typedef somethingSomething
* @property {string} variable that will be input
* @property {date} name in the class
ctrl + space will pull up what was set as @property, when you are on a different .js referencing the class

if you make the function outside of the exported class then it cant be accessed in the console. It can only be reached by other actions in the same file. It becomes a private function. it is best practice to put an _ at rhe start of the name to signify it is a private function

on submit goes on the form

can't create proxy from date object? 

this.checkingState ? (if its true) this.doThisThing : (or) this.doThatThing

emit makes the observer recognize a change

