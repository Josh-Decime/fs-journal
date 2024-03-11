# Vue


When you start a new vue file!
vt (brings up list of starting code, imports brings in your basic imports of vue components)

in vue you can @click.prevent   to prevent default on a form where it tries to refresh the page

:key="" ins necessary but is good practice

target blank to make a tag open in a new tab

:class=" 'custom-css' : ifConditionalValue.isItTrue"      you can conditionally render styles if conditions are met

{...AppState.account}     ... is "spread operator"  makes it so values in AppState.account aren't being changes, it is only giving us the data inside 

{ immediate : true }  will run on page load, can be put into a watch so you don't have to do onMounted as well


*********************
you can call functions in the AuthService after you have logged in

in router
authSettled is the best thing, cant believe they didn't teach us that sooner




Vue cant be deployed without building it first
when you want to deploy, npm run build