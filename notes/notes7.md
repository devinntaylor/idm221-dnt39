#The Box Model

<B> Calculate Height </b> 

top margin
    + top border
    + top padding
    + height
    + bottom padding
    + bottom border
    + bottom margin

<b> Calculate Width </b> 

left margin
    + left border
    + left padding
    + width
    + right padding
    + right border
    + right margin

<b> Height and Width </b> 

- by default, if not specified, values will be auto adjusted

<b> Height and Width Values: </b> 

div {
  width: 450px; /* absolute width */
  width: 75%;   /* relative width */
  width: auto;  /* default */

  height: 125px;  /* absolute height */
  height: 50%;    /* relative height */
  height: auto;   /* default */
}

<b> Min and Max </b> 

div {
  min-width: 450px;
  max-width: 600px;
  min-height: 120px;
  max-height: 160px;
}

---
<b> Viewport Unit </b> 

div {
  height: 100vh;
  width: 100vw;
}

1vw = 1% viewport width 
1vh = 1% viewport height

---
<b> Margin </b> 

div {
  margin-top: .5em;
  margin-right: 1em;
  margin-bottom: 2em;
  margin-left: 1em;
}

<b> Margin Shorthand: </b> 

div {
  margin: 1em; /* all four sides */
  margin: 0 1em; /* top and bottom 0, right and left 1em */
  margin: .5em 1em 2em; /* top: .5em, right and left 1em, bottom 2em */
  margin: .5em 1em 2em 1em; /* clockwise starting at top */
}

values are specified clockwise : top, right, bottom, left

can also specift keyword <b> auto </b> :

div {
  margin: 0 auto;
}

<b> set left and right margins to audto and declare width for auto to work </b> 

---

<b> Padding </b>

div {
  padding-top: 0;
  padding-right: 1em;
  padding-bottom: .5em;
  padding-left: 1em;

  padding: 1em;
  padding: 0 1em;
  padding: 0 1em .5em;
  padding: 0 1em .5em 1em;
}

---

<b> Reset </b> 

* {
  margin: 0;
  padding: 0;
}

ul {
  margin: 0 0 1.5em 1.25em;
}

---

<b> Box Sizing: Border Box </b> 

###highly recommended way to start style sheet 

* {
  box-sizing: border-box;
}

^ Apply the box-sizing property to the universal selector with a value of "border-box" and the browser will now do the math for you and maintain your width/height values even when margin/padding/borders are applied. The browser will calculate the totals and dynamically adjust the width value so that your container with a width value of 200px will actually be 200px even if there's 20px of margins, a 2 pixel border and 10 pixels of padding applied.

---

<b> Borders </b> 

border
border-side
border-width
border-style
border-color
border-side-width
border-side-style
border-side-color

<b> Border Shorthand </b> 

div {
  border: [width] [style] [color];
  border: 2px solid black;
}
^ The border property has a shorthand for specifying all of the properties in a single rule. The order of the values must be width, then style, then color.

<b> Rounded Corners and Shadows </b> 

div {
  border-radius: [radius]; /* applies to all four sides */
  border-radius: [topLeft] [topRight] [lowerRight] [lowerLeft];
  box-shadow: [horizontalOffset] [verticalOffset] [blurRadius] [spread] [color];
}

--- 

<b> Background </b> 

background
background–color
background–image
background–repeat
background-attachment
background–position
background-size

<b> Background color </b>  is a color value with the word that specifies the color of an elements background. You can also specify the "transparent" keyword if you want the elements behind the element to be visible. This is the default.

div {
  background-color: blue;
  background-color: #808080;
  background-color: transparent;
}


<b> Background Image </b> : 
div {
  background-image: url('images/texture.png');
}

- related to style sheet, NOT html file 

---

##EXAMPLE 

</head> 

<body> 

<div class="wrapper">
    <div class="card">
        <div class="card__img"></div> 
            <img> 
            src="link"
            alt="some delicious food" 
            <img/>
    </div> 
</div> 

</body> 

</html> 