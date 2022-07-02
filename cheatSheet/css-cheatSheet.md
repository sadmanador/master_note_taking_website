css shorthands

background-image set an img to an element like div
background-image: url("path")

background-repeat take no-repeat, repeat-x and repeat-y value

background-attachment takes fixed and scroll value when a background-image is added


background shorthand
background: color image repeat position;
border: borderWidth(px) borderStyle color;


border shorthand
border-style: topBottomStyle leftRightStyle;
border-style: topStyle leftRightStyle bottomStyle;
border-style: topStyle rightStyle bottomStyle leftStyle;





margin shorthand
margin: auto;      centered the element by adding equal margin at left and right.
margin: allFourSides;
margin: topBottom leftRight;
margin: top leftRight bottom;
margin: top right bottom left;
margin collapse= only incase of one elements bottom margin and next elements top margin collapse into each other. they don't adds into each other but apply the bigger margin. suppose bottom of h1 is 20px and h2 is 20px. in this case they don't adds up like 40px, they simply have 20px margin between them. this however doesn't happened incase of right and left margin.




padding shorthand
padding: allFourSides;
padding: topBottom leftRight;
padding: top leftRight bottom;
padding: top right bottom left;




height and width values
max-width: px/rem       adds width which can be minimize but can't exceed the given value.
auto = default
% = percentage of the containing box, browser calculate the size for %. 100% width means the available whole width of the browser. % works best with width.
px/rem = specified length
initial = sets to default value
inherit = inherit from parent element.



outline
outline is a line drawn outside of the border of an element. outline is similar as border.
outline-style
outline-color
outline-width
outline-offset: adds space between border and outline of an element.
shorthand outline: width style color;



text
color: apply color on text.
text-align: left center right;
text-align: justify;        make line stretched to make every line same width.
direction & unicode-bidi
direction: rtl
unicode-bidi: bidi-override;        this properties change the text direction.
vertical-align      apply to single words with span tags and take 5 values.
baseline            which is default
text-top
text-bottom
sub
super



text-decoration        take values as follows
overline        adds line above the text line
underline       adds line below the text line
line-through    adds line that crossed the text middle
text-decoration: overline line-through underline;        to add all line to the same text.


text-transform      takes 3 values
text-transform: uppercase lowercase capitalize;

text-indent: px/rem
text-spacing: px/rem
line-height: 1 is default
word-spacing: px/rem
white-space: nowrap     doesn't break text line and add horizontal scrollbar.
text-shadow: horizontal vertical;        takes negative and positive
text-shadow: horizontal vertical color;
text-shadow: horizontal vertical blur color;
text-shadow: horizontal vertical blur color, horizontal vertical blur color;



list-style-type: none circle square upper-roman lower-roman
list-style-position: outside(default) or inside
list-style-image: url('path')
list-style shorthand
list-style: type position image;


CSS table
border-collapse: collapse;      to get rid of double border of table



display: none       doesn't take up the space of the element
display: hidden     takes up the space of the element
display: block      acts like a block element
display: inline-block       acts like a block element but inside a line
display: inline     acts like an inline element
display: grid       enable grid view
display: inline-grid       enable grid view but inline
display: flex       enable flex view


position: static        default
position: relative      relative to its origin, top, bottom, left, right value will cause transform from its origin.
position: absolute      relative to the relative parent
position: fixed         fixed to the viewport
position: sticky (-webkit-sticky)       sticky to the position when scroll, top, bottom, left, right value must be used


overflow: hidden
overflow: visible
overflow: scroll
overflow: auto
overflow-x: hidden      to hide the horizontal scrollbar.



float: left right none(default) inherit;
element which need to appear below the floating element should use clear property.
clear: left right both inherit none(default)


align
margin: auto        make an element horizontally centered.
text-align: center      make the text horizontally centered.

image align center
display: block
margin: auto        margin-left & margin-right:auto;

left/right align without float
position: absolute
right: 0px;


clearfix
when an element is taller than the container, clearfix can be used.
container {
    display: table;
    clear: both;
    content: "";
}
img{
    float: right;
}

vertically aligning content
add top & bottom-padding

both vertically & horizontally centering
padding: 50px 0;
text-align: center;

opacity: 0.0 - 1;

border-radius: px/rem;

border-image: url('path') num/% round/stretch;

background-image: url();
background-position: right bottom ;
background-repeat: no-repeat ;

double background image
background-image: url(), url();
background-position: right bottom, left top ;
background-repeat: no-repeat, repeat ;

background-size     specify the size of the image in lenght or percentile or in cover and contain.
background-size: contain;     scales the img to best fit it's container     
background-size: cover;     stretch the img so that the img will cover the whole container, img might be a lill cropped to cover the container.

object-fit: fill/cover/contain/none/scale-down;
object-position: hori% verti%;

background-origin       specifies the position of the background-image
background-origin: border-box;      img start from the upper left corner of the border.
background-origin: padding-box;     (default)img start from the upper left corner of the padding edge.
background-origin: content-box;     img start from the upper left corner of the content.

background-clip     specifies the background printing area(from where the background will start)
background-clip: border-box;        (default) background will start from the edge of the border.
background-clip: padding-box;       background will start from the edge of the padding.
background-clip: content-box;       background will start from the edge of the content.


color keyword
color: inherit;
color: transparent;
border: currentcolor;       will take transparent from the color:.


gradient
linear-gradient
background-image: linear-gradient(to right/left/top/bottom, colorName, colorName);
background-image: linear-gradient(deg, colorName, colorName);
background-image: repeating-linear-gradient(to right/left/top/bottom, colorName %, colorName %);


radial-gradient
background-image: radial-gradient(colorName, colorName);
background-image: radial-gradient(colorName %, colorName %);
background-image: radial-gradient(circle/ellipse, colorName, colorName);
background-image: radial-gradient(closest-side at hori% verti%, colorName, colorName);
background-image: radial-gradient(farthest-side at hori% verti%, colorName, colorName);
background-image: radial-gradient(closest-corner at hori% verti%, colorName, colorName);
background-image: radial-gradient(farthest-corner at hori% verti%, colorName, colorName);
background-image: repeating-radial-gradient(colorName, colorName %, colorName %);


conic-gradient
background-image: conic-gradient(colorName, colorName, colorName);
background-image: conic-gradient(colorName deg, colorName deg, colorName deg);
background-image: conic-gradient(colorName startDeg endDeg, colorName startDeg endDeg, colorName startDeg endDeg);
background-image: conic-gradient(from 90deg, colorName, colorName, colorName);
background-image: conic-gradient(at hori% verti%, colorName, colorName, colorName);
background-image: conic-gradient(from 90deg at hori% verti%, colorName, colorName, colorName);

box-shadow
box-shadow: horiPX vertiPX;
box-shadow: horiPX vertiPX colorName;
box-shadow: horiPX vertiPX blurPX colorName;
box-shadow: horiPX vertiPX blurPX spreadPX colorName;
box-shadow: horiPX vertiPX blurPX spreadPX colorName inset(shadow inside the box);
box-shadow: horiPX vertiPX blurPX spreadPX colorName, horiPX vertiPX blurPX spreadPX colorName;
box-shadow: horiPX vertiPX blurPX spreadPX rgba(0, 0, 0, 0.3); (transparent color)

text-overflow: clip/ellipse;        clip cuts the text, ellipse adds three dot before cutting.
word-wrap: break-work/break-all/keep-all;
writing-mode: horizontal-tb/vertical-rl;


@font-face{
    font-family: myFirstFont;
    src: url();
}
div {
    font-family: myFirstFont;
}


transform
transform: translate(horiPX, vertiPX);
transform: rotate(+/-deg);
transform: rotateX(+/-deg);
transform: rotateY(+/-deg);
transform: rotateZ(+/-deg);
transform: scale(horiNUM, vertiNUM);
transform: scaleX(NUM);
transform: scaleY(NUM);
transform: skew(horiDEG, vertiDEG);
transform: scaleX(deg);
transform: scaleY(deg);
transform: matrix(scaleX(),skewY(),skewX(),scaleY(),translateX(),translateY());

transition
transition: property duration;
transition-delay: numSEC;
transition-duration: numSEC;
transition-property: width/height/color/background-color/transform;
transition-timing-function: ease/linear/ease-in/ease-out/ease-in-out/cubic-bezier(n,n,n,n);



animation property
background-color
color
top, right, bottom, left        when position: relative;

@keyframes animationName {
    from{}
    to{}
}

div {
    animation-name: animationName;
    animation-duration: numSEC;
    animation-timing-function: ease/linear/ease-in/ease-out/ease-in-out/cubic-bezier(n,n,n,n);
    animation-delay: numSEC;
    animation-iteration-count: numTimeanimationRun/infinite;
    animation-direction: normal/reverse/alternate/alternate-reverse;
    animation-fill-mode: none(default)/forwards/backwards/both;
}
animation shorthand
animation: name duration timing-function delay iteration-count direction;

@keyframes animationName {
    0%{}
    25%{}
    50%{}
    75%{}
    100%{}
}

-webkit-box-reflection: above/left/below/right gapPX linear-gradient();


flex-box

.container
display: flex;
flex-direction: row/row-reverse/column/column-reverse;
flex-wrap: wrap/nowrap/reverse-wrap;        flexItem with break when necessary.
flex-flow: direction wrap;
justify-content: flex-start/center/flex-end/space-around/space-between;     horizontal alignment
align-items: flex-start/center/flex-end/stretch/baseline;     vertical alignment
align-content: flex-start/center/flex-end/stretch/space-around/space-between;     align flex lines.


.item
order: num;
flex-grow: num;     similar as span column
flex-shrink: num;       1(default) higher than 1 will shrink the item.
flex-basis: px/rem;     width of an individual item.
flex shorthand
flex: grow shrink basis;
align-self: flex-start/center/flex-end;     override the align-item of container and item height.





grid layout

.container
display: grid/inline-grid;
gap: px/rem;        defines the gap between items.
grid-template-column: auto/%/px/rem     auto/%/px/rem   auto/%/px/rem;      for three column layout.
grid-template-row: auto/%/px/rem     auto/%/px/rem   auto/%/px/rem;      for three row layout.
justify-content: space-evenly/space-around/space-between/center/start/end;      horizontally adding space.
align-content: space-evenly/space-around/space-between/center/start/end;      vertical adding space.


.item
grid-column: 1 / 3;     start at grid column line 1 and ends at line 3.
grid-column: 1 / span 3;     start at grid column line 1 and span 3 columns.
grid-row: 1 / 3;     start at grid row line 1 and ends at line 3.
grid-column: 1 / span 3;     start at grid row line 1 and span 3 rows.
grid-area: grid-row-start / grid-column-start / grid-row-end / grid-column-end;
grid-area: 1 / 1 / span 3 / span 4;     also supports span.
grid-area: myGridName;      also be use to assign a name of grid item.
.container
grid-template-areas: 'myGridName myGridName myGridName';    to span gridItem myGridName to span 3 columns.
