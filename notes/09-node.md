# Node

bcw create
auth0

middleware Auth checks for bearer token

middleware body-parser checks if they are bringing anything with them, like adding a cat

if your knight is looking for something that isn't there they move down the hall ot the middleware default error handler

run and debug, makes powershell run a server that can test your data

you can extend classes, does everything the base class does + the new functionality of the new class

controller builds the door
super calls the controllers constructor 
'api/name' puts the name on the door
router is the hallway

extends baseController
if it extends it has to have super('example/branch')

******you have to restart your server to make changes update, it can take a few seconds to refresh
you have to refresh the server before it will show on the webpage too

console logs show up in your server, not on the browser console

IN THIS ORDER EVERY TIME: request, response, next      
you don't need all 3 to make it work

the router will take the first option

.get('/branch', this.differentGetRequest)
empty '' get will branch on the api url that it was on, if you want more locations they have to extend that url

route parameters, extend url with variable
.get('/:color')

next keeps them moving, if they were checking a route & they put in a search for something not there, next puts them back into the hallway where they keep moving & hit the 404

controllers return information from the service instead of the AppState for a server

request in the controller to the service, then service returns to the controller

*****  www.postman.com allows you to make requests to your api as if its a front end client
go-to tool for testing out API

logger.log to get console logs in debug console when testing an api. It is in the utility folder. 
it requests specifically to the debug console, whereas the console logs can get lost

raw JSON

adoptCat is removeCat in the example



.env
connection string=(paste the mongodb string with the password)

.gitignore will ignore files when you upload them to github. it ignores .env so your password doesn't get posted on github
other ignore is so that it doesn't try to save your extra tools like bootstraps 

mongo is the database
mongoose talks between the database & our projects

new schema (schema is an import from mongoose)

In your model you need to elaborate on what information will be input 

enum creates a list of acceptable answers 

request.body is the payload

dbContext gives context for talking to the server. you need to go into the DbContext file to set up your context
Cars = mongoose.model('car', CarSchema) 

find() has no filter & gets everything

/example/:somethingElse
: allows it to take in a new value that you can use in your functions to find an object/array that matches your search

params checks the url. looks for exchangeable pieces of the url : makes it a parameter 

originalCar.make = updateData.make ?    updateData.make : originalCar.make           uses truthy falsy logic
you need                             ^ !=undefined    if you are checking booleans 

for Greg'sList we will need to make out own .env

{timestamps: true} will give you created at & updated at timestamps 


when you turn virtuals on you can add them to the schema          they only exist if you tell them to exist
{toJSON: {virtuals: true}}

populate('virtualsName')   tells mongoose to retrieve data for the virtual
if you have a space it separates multiple inputs

it will try to bring in an object with an array in it, unless you say just one & then it will be an object

in postman, get, Auth (dropdown) bearer token

if you get back an empty object it is a promise that was never awaited 

express-mcv has a client & a server, so you can login with auth credentials to get a user token
initialize repository right in the beginning BEFORE OPENING WORKSPACE        after initializing then open workspace
demo.code-workspace Open workspace 

you only get debug server if you are in a workspace

           need to update env in two locations
client-> app -> .env    &      server -> .env

if you are working on someone elses file you need to    npm i    because node modules are excluded from git uploads

pojo = plain old javascript object




ctrl + p opens where you can choose from your files
