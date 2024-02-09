# CSharp


instead of saying let or const you set the variable type, string, int, double, float, decimal, char, bool, 

if you add ? after it becomes null-able

there is no undefined... no truthy & no false-y

arrays have to have defined lengths (fixed length) 
if you want an array, use List instead

dictionary are key value pairs

almost everything exists as a class.. or an interface

set accessors,,, public or private
can readonly so that value cant be changed
readonly is like const
internal is only accessible to what is in the top level namespace

can define controller
[ApiController]
[Route("api/location")]

must inject repo & service into startup cs     .... register the dependencies     if you get an error that says dependency injection you forgot this step
repo goes above service because it must be created since it will be called


every service will only have one repo

$ before " " to string interpolate    $"interpolated data is {interpolateData}"
if you put $@  then it supports multi line strings

singleton vs scope: Singleton makes a repository that is shared, never deleted. Scoped is created per need/request, once its no longer needed its deleted, saves memory storage overhead

error squiggly underline warning that happened on compile might stay even after it is fixed until you compile the code again

IDbConnection is a dependency that is already registered in the template 

repository executes SQL statements
string sql = @ "SELECT * FROM (tableName)"

IEnumerable & IDbConnection are interface 
loop-able collection 

how to make a table into usable objects?
List<Car> cars = db.Query<Car>(sql).ToList();
database I am asking you for cars in a list

there is a difference between VSCode being connected to the database & your application being connected 

appsettings.Developer
"CONNECTION_STRING': "server=(server);database=(database);

database does construction for you, data needs to be accessed in the same order as it is in the MySQL database

when building in the model, say prop (tab) will fill out the private int thing = thing {get; set;}

look into making your own snippets

you tell it which tw tables its accessing, then the 3rd is you telling it which one you want back
db.Query<Album, Account, Album>

new folder Interfaces 
> IRepository.cs
setting up an interface makes it faster to build out & implement

[Authorize] makes it check for authorization before running that function, can also be added to the entire controller

.net mostly handles await for us when its internal
when you reach out to the Auth provider it is going to another service so you must tell it to await
if it is async the return type has to be wrapped in a task
Task<ActionResult<Album>> 

HttpContext is a request

abstract is a class you can never instantiate 
lets the code know it cant be used on its own, its meant to extend another class

what is `abstract` preventing?

when making the save favorite recipes, return the recipe with the collaborator Id attached to it