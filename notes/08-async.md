# Async

<!-- SECTION API -->

MVC-Auth

on an API site look for requests.. typically HTTP. will open a page of code

fetch()     is 'built in' in javascript.. technically its an api tho..? mysterious!
fetch(http:// the api url)
to see if it loaded in, check the network tab 
click on what was brought in -> headers -> response (gives raw code) -> preview gives an array preview

let response = fetch(https://.....)

your code will have to stop to wait for the fetch to load in. async await on getMonsters() in service
async    .... await response          later added   .json()
response should say {all the info that is loaded in by the API}
if it says promise fulfilled then it didn't wait, to impatient!

.json() parses the data from a string to an array of objects.. now console can display object/array of all objects
just makes it readable

in order to use the data you have to make it fit your array      in service
let bananaWord = body(your banana word).data.map(bananaData => new ModelName(bananaData))

snake casing uses _                example: common_locations
camel casing has 2nd word capital, example: commonLocations

<!-- awesome tip!!! -->
ctrl + . on a non declared method to declare it in the file as a placeholder

utilities has a writer.. setHTML('id', content)
basically the same as document.getElementById but shorter & will tell you if you misspelled anything, with a pop up 

<!-- NOTE super helpful tip for changing all names at once -->
f2 can change the name of a variable/function everywhere all at once!! But it wont change the listener

if your data isn't loaded in because you are on a different page, you have to load that data onto that page as well. 


** were now using mvc-auth template ..... not mcv

env.js environment, for static variables your project might need
copy paste auth0 login link
for these logins it can be fake info

id_token is given after you log in & the expiration date is set by the website

axios pulls information from environment variables.. you don't need the full url, you set the url in the environment, just needs the specific location after the base url

get request takes in info
post request allows you to send to the api

payload is the object you sent

https://http.cat/        shows all # error


you can catch uncaught errors
try (to do the thing)      catch    (if it fails)

you can attach listener to the user, so it recognizes when they log in
needs listener for when you start on the page, just drawing function for when you navigate to the page

if you do try   catch but don't do anything after catch it will eat your error... you have to console.log the error

api includes methods for get, post, put, delete

you can use @type to tell the AppState what will fill it

static in front of members of a class it doesn't exist on those things, it exists on the blueprint... (no clue what that means)

typeof

middleware runs between. in example it makes it so you have to log in to use the page

put request is the most complex. put needs to know where it is & give it new information. like what push & delete need combined

turrinary is ? :    (maybe? look that up)


if you change colors in scss it wont actually change unless you compile it. 
open terminal & run: npm i   
after that run: npm run sass
lol jk nvm it doesn't work

there is a drop down for changes under commit button 

token, user info & accounts
