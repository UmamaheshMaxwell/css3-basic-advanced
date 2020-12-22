CSS3   ( css1, css2, css2.1 and css3)
-----
1. Inline
2. Internal
3. External

New Features
-------------
1. new selectors - better selection of HTML elements
2. shadow Effects - box-shadow, text-shadow
3. Rounded corners - Easily round the corner of images and for block level elements
4. Gradients 
5. opacity
6. Transistions
7. Transformations
8. Flex-box
9. mulit-column layout
10. grid

CSS3 is supported in HTML5 browsers

    - IE8 and lesser doesn't support css3
    - IE9 suports css3 but not fully
    - IE10, Edge, chrome, Firefox, safari supports CSS3

Selectors
-----------
Simple selectors - select elements based on name, id and class
combinator selectors - select elements based on specific relationship between them
pseudo-class selectors - select elemnts based on certain state
pseudo element selectors - select elements and style the part of the elemnts
attribute selectors - select elements based on attirbute or attribute-value

Advantages
---------
CSS3 save time
page load faster
easy maintenance
superior style to HTML
multiple device compatibiity
global web standards

@import - will aloow us to import a stylesheet into another one
        - must be at the top of the css document
        - supports media queries

Colors in CSS3
--------------
Color Names    - red, green, yellow, blue, gray
HTML5 Colors   - coral, crimson, blueviolet, darkgoldenrod, darkmagenta
Hexa Decimal Colors - #CCCCCC, #FCFCFC, #FFFFF
RGB - RED GREEN BLUE

crete HTML Shortcuts
--------------------
.class + tab        : will create div with class attribute
div.classname + tab : will create div element with class attribute
div#id + tab        : will create div element with id attribute
div*3.class + tab   : will create 3 div elements with class attribute
div*3#id + tab      : will create 3 div elements with id attribute

shortcut to comment code - ctrl + /

Simple selectors
-------------------
element, class, id

combinator selectors
--------------------
1. descendent selector (space)
2. child selector (>)
3. adjacent sibling selector (+)
4. genreal sibling selector (~)

pseudo-class Selectors (adds special effects)
-----------------------------------------------
A pesudo selector matches components based on an additional condition 
and not neccessarily defined by the document tree.

pseudo class
-------------
Allows you to style the dynamic states of an element such as hover, active
and focus state.

Syntax
-------
selector:pseudo-class {
    property: value
}

Pseudo Element Selectors
--------------------------
Pseudo element is used to style specified parts of an element. 
we don't need javascript or any other script to bring those effects

for e.g.
-----------
1. Style the first letter or first line of the element
2. Insert the content before or after the content of an element

Syntax
----------
selector::pseudo-element {
    property: value
}

double colon syntax is introduced in CSS3 earlier single colon was 
used for both pseudo class and pseudo elements (css2 and css1)

::first-line
::first-letter
::before - Insert content before the content
::after  - Insert content after the content
::select

note: ::first-line, ::first-letter can only be applied to block level elements
-----

Attribute Selectors
--------------------
Select all elements with specified attribute

selector[attribute]
--------------------
a[target]
div[class]

selector[attribute="value"]
-------------------------------
div[class="container]

selector[attribute~="value"]
------------------------------
a[title~="web"]

Background
-----------
Property handles background color, image , position, attachment 

background-image
----------------
background-repeat : repeat-x - repeats the image horizaontally
                    repeat-y - repeats the image vertically
                    no-repeat - will not repeat the image

background-attachment  (scroll, fixed, local)
----------------------
specifies whether the background image should scroll or be fixed

Background Shorthand
--------------------
background-Color
background-image
background-repeat
background-attachment
background-position

background : #fff url no-repeat fixed top right

background-clip
----------------
The background clip property defines how far the background should extend with an element


Fonts
-------
Font-family - used to change the face of the Font
font-style - used to make font italic or oblique
font-variant - used to create a samll caps effect
font-weight - increases or decreases font weight
font-size   - incraeses or decreases the size of the font
font - shorthand to specify other property

Opacity /Tranparency
---------------------
Opacity specifies the opacity or transparency of an element
It can take value from 0.0 to 1.0
Lower the value the more transparent it is


RGBA
-----
RGBA - rgba(red, green, blue, alpha)

alpha specifies opacity of the color

alpha - 0.0 (fully transparent) and 1.0 (fully opaque)


CSS-text
---------
Whe use it to manipulate the text using CSS properties

1. color  - set the color of the text
2. direction - set the direction 
3. letter-spacing - To add or subtract space between a letter that make up a word
4. word-spacing - add or subtract space between the words of a sentence
5. text-indent - Indent the text of a paragraph
6. text-align - align the text of a document
7. text-decoration - To Uderline, overline and  strikethough
8. text-transform - To capitalize the text ot convert text to uppercase or lowercase letters
9. white-space - to control the flow and formatting of the text 
10. text-shadow - To set the text shadow around a text 

CSS-Border
----------
Will allow us to specify the style, width and color of an element's Border

Border-style
------------
Specfies what kind of borders to diplay

dotted - defined dotted borders
dashed - Defines a dashed borders
solid  - Defines a solid borders
double - Defines  a double border
groove - Defines a 3D goorved border; depends on background color;
ridge  - Defines a 3D ridge border; depends on background color;
inset  - Defines a 3D inset border; depends on background color;
outset - Defines a 3D outset border; depends on background color;
none   - Defines no border
hidden - Defines a hidden border

Border-width ( will not work without border style)
--------------------------------------------------
Specifies the width of the border

we can set the width using specific size
we can use pre-defined values - thin , thick or medium

border width can have one to four values


Border-color ( will not work without border style)
--------------------------------------------------
Used to specify the color of the four borders

Border-Sides
------------
used to specify border for each side

border-top
border-right
borer-bottom
border-left

Border-Shortcut
----------------
To Shorten the code, it is alo posszible to specify 
the individual border properties in one property

border - Border width
         Border Style
         Border Color

We can specify all the individual properties for just one side


Rounded borders
----------------
Border Radius property is used to add rounded border to an element.

Margins
---------
Margin used to create space around elements outside of any defined borders

Margin-Shorthand
-----------------
Margin property is a shothand property for the following individial properties

margin-top
margin-right
margin-bottom
margin-left 

auto - The browser calculates the margin
length - specifies a margin in px, pt , cm etc.
% - specifies a margin in % of the width

* Negative values are allowed 

Margin Collapse
---------------
Top and bottom margins of elements are sometimes collapse into a single margin.
which is equal to the largest of the two margins. This only happens with top
and bottom margins.

Padding
--------
Used to generate space around an element's content inside of any defined border.
It has four properties

padding-top
padding-right
padding-bottom
padding-left 

length - specifies a padding in px, pt , cm etc.
% - specifies a padding in % of the width

* Negative values are not allowed 

It is possible to specifiy all the padding properties in one property

Padding and Element width
-------------------------
If an element has a specified width, the padding added to 
that element will be added to the total width of the element


If <div> element is gien width of 300px the actual width of <div> 
element will be (300px + 25px left padding + 25px right padding)

Height and width
----------------
height and width properties are used to set the height and width
of an element

auto - Broswer calculates the width and height
length -  Defines the height in px,cm etc
% - Defines height / width in %

initial - Set height and width to its deafult value
inherit - The height and width will be inherited from its parent value