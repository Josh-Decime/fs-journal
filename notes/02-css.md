# CSS

instead of height, min-height

* make utilities *
.w-50 {
    width: 50%;
}
.d-flex{
    display: flex;
}

to contain image
img{
    object-fit: cover;
    object-position: center;
    width: 100%;
}

get familiar with css selectors 
nav>span 
footer>div:nth-of-type(2)>p

changing flex to colum changes axis, which flips justify & align

you can target elements within its parent... .left-section>p

usually opt for padding vs margin to make space
padding padding padding padding padding.. & sometimes margin


create new repository; copy ; ctrl+`(tilda) ; paste in terminal?

<!-- Croc Till U Drop -->

look into position absolute. position absolute takes it out of its regular bounding & nothing knows where is is anymore? 
"be wherever you want to be"
using relative can bound it with a start location (relative is in HTML)
magic-card {
    top: (moves the amount of pixels needed from relative) (vw = view width)
    position: absolute;
    width: 100%;
}
to help with overspilling on smaller view be aware of the direction it is pouring.. you can also adjust its width based on screen size

you can copy paste some styling code out of Figma

you can change hover color on a button! MAKE IT GLOOOOWWWW!!!!!!!

you can apply hover to everything!!!

to stop a sticky top from running into the top of the screen add top: (X)px; in its style

ctrl+space bar brings up intellicense (pulls up list of fonts)

when setting fonts use , to create backup text font options if the one before it is unavailable.
linking the font in CSS will allow the site to have the font even if it isn't native on their device

display: block brings the invisible back from exile when adjusting screen size