# HTML

link css
<link rel="stylesheet" href="style.css">

use header, main, footer.. instead of all div

<nav> to group together navigation elements

highlight (text) ctrl+d to highlight other (text)

<span> makes the elements span left to right
add style padding to space elements 
button can be inside <p> 

.container {
display: flex; 

section is just fancy div

h1,2,3,4,5 signifies the importance of the text. always in descending order 

after <img src="image.url"> add alt="explanation" to help with captioning 

div*3 will make 3 div 

lorem generates latin fill text

alt+click makes 2 cursors 

(BCW.code-snippets)
link:

linked last has highest precedence

control+shift+t opens old closed tabs

<i class="icon i want to use"> for icon

<hr> line break

<!-- * BOOTSTRAPS * -->

link:b5 references bootstraps assets

container-fluid goes edge to edge | container is bounded within | row goes to the edge (framework of the house?) 
you can set breakpoints for the rows, sm md lg xl xxl (size or larger) when it gets below that size it removes its sizing & takes over the whole space

text-end could be useful | btn sets button style defaults w/ bootstraps | ps, padding start; or offset-(number/12) | 
font size class="fs-(x)" 

* title tag sets text that comes up when you hover over

background-image: works like a background color with a picture, have to set height or it defaults to 0; you can put content over it
background-size: cover; (contain for tiling images)

to make slightly transparent, opacity makes whole thing including text transparent, put in custom color that has opacity set 
class"--bs-bg-opacity: .5" | bg-opacity-50

** class="img-fluid" makes image scale to space given, so inside a row column. it tries to fill whole space. wrap image in div class="w-50" or you can class the image itself w-50... if you wrap in div you can add padding so text isn't so close
you can make a colum display fex d-flex

script usually goes to the bottom, style debug gets differed so it can go in header
style debug creates an outline and grid for elements

ctrl/ to comment out
use anchor tags to easily differentiate sections for ease of navigating code

.(the code you want) tab will fill out the code chain 
example: section.row.bg-primary+div.bg-primary tab can build out code structure very quickly

breakpoints allow you to implement changes in code based on screen size. so if screen gets smaller you can make elements vanish
d-none turns off displaying. d-md-flex turns it visible once it is over medium size | d-none d-md-flex
code it for mobile size first & then the exception is for medium/larger screens

order-0 makes it first, order-1 2nd etc.. order-o order-md-1 ; to make it 1st on mobile but 2nd on desktop  
order is best on columns, not rows

<!-- Crock Till U Drop -->

* to move a box between the bounds of 2 spaces *
Absolute is set in CSS, but position-relative is placed within the class in HTML
col-11 col-md-7 to adjust magic card width when the screen shrinks

you can nest rows into columns 
you can also put a column in a column, or row in row, but it isn't recommended. it breaks stuff

"forms are the closest thing to hell you will find in web development"-Mick
class="form-control" keeps the form more contained so it fills the space but doesn't exit the space
form-range allows the slider to be a slider & not try to be a text box

selected means it it starts with that & you cant choose it from a dropdown

class="sticky-top" it will stick to the top of the screen as long as it is within its row/column.
if you want the top bar of the website to stay, put it above the header

when importing fonts or other styles, put them before bootstraps so that it can reference them


in html if there aren't '' on ${thing} it will look for a variable. but if you '${thing}' it will look for a string

marquee allows elements to move