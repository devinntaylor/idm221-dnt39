#Working With Text
---
##Special Characters 
- < 
  - code reacts to this symbol as beginning of a tag 
- special entity to represent characters
  - name 
  - numeric value 
  - <a href="https://www.w3schools.com/html/html_symbols.asp">List of Special Characters</a> 

---

##Typography
- The 5 Generic Families
  - serif 
    - "tails" 
  - sans serif
    - no tail 

---

<b> Web Safe Typefaces </b>
- Most Safe 
  - Arial
   - Times New Roman / Times
   - Courier New / Courier
   - Palatino
   - Verdana 
   - Georgia 

Font-Family Property:

p {
    font-family: Arial, Helvetica, sans-serif;
    font-family: 'Times New Roman', Times, serif;
    font-family: 'Courier New', Courier, monospaced;
}

---

Setting Font Size:
p {
  font-size: 12px;  /* in pixels */
  font-size: 150%;  /* as a percentage of the parent element */
  font-size: 1.5em; /* desired / parent */
}

 on modern browsers - starting font size if user hasnt tweaked preferences  - roughly <b> 16 pixels </b>

---

Calculating ems:

1em = 100% of parent font

body { font-size: 16px; }
h1 { font-size: 2em; /* 32px */ }
h2 { font-size: 1.5em; /* 24px */ }
<b> desired px value / parent px value </b> 
$$24/16 = 1.5$$

<b> size you want / parent size </b> 
- parent is 1 line above 

---
##Homework Example: 

body { font-size: 16px; }
main { font-size: 0.88em; /* 14px */}
main p {
  /* font-size: 12px; */
  font-size: ??em;
}

---
body { font-size: 16px; }
main { font-size: 0.88em; /* 14px */}
main p {
  /* font-size: 12px; */
  font-size: 0.86em;
}
$$12/14 = 0.86$$

---
Calculating rems 

- calculation based on root element 
  - <b> desired px value / root px value </b>



html { font-size: 100%; /* ~16px */}
body { font-size: 1rem; }
main { font-size: 0.88rem; /* 14px */}
main p {
  /* font-size: 12px; */
  font-size: 0.75rem;
}
desired px value / root px value
$$12/16 = 0.75$$

- references back to root every time, saves time doing math
  <b> - html is the root element </b>

---
##Font Styles
p {
  font-style: italic;
  font-style: normal; /* remove style */
  font-variant: small-caps;
}

##Font Weights 
p {
  font-weight: 700;
  font-weight: bold;    /* same as 700 */
  font-weight: normal;  /* same as 400 */
  font-weight: lighter; /* relative to parent element */
}

##Line Height
- use relative units 

p {
  line-height: 14px;
  line-height: 140%;
  line-height: 1.4em; /* same as 140% */
  line-height: 1.4;   /* same as 140% and 1.4em */
}

- good starting point = 1.5 / 1.4

<b> Example Font Code: </b>

p {
  font-family: Arial, Helvetica, sans-serif;
  font-style: normal;
  font-variant: normal;
  font-weight: 500;
  line-height: 1.4;
}

- Shorthand: 
  - font: [style] [weight] [variant] size[/line-height] family;
    - can skip anything you dont want to declare 

---
##Formatting Text in CSS 

  - think about accessibility issues 
    - keep underlines under links 

---
##Text Shadows 

text-shadow: horizontalOffset, verticalOffset, blurRadius, shadowColor;

h1 {
  text-shadow: 4px 4px 8px rgba(0,0,0,0.3);
}
h2 {
  text-shadow: -2px -2px 4px red;
}

---
#CSS Comb **

---
@font-face { 
    font-family: 'ChunkFiveRegular';
    src: url ('fonts/chunkfive.eot'); }

h1, h2 {
  font-family: ChunkFiveRegular, Georgia,
     serif; }

###Tools 

<a href="https://www.web-font-generator.com/">Web Font Generator</a> 
<a href= "https://www.fontsquirrel.com/tools/webfont-generator"> Font Squirrel </a> 

### Online Font Servies
<a href= "https://fonts.google.com/"> Google Fonts </a> 


- when importing fonts, have to use correct path to folders (../../)

---
Mobile device icon in browser code 
- responsive design mode for mobile size 
  - firefox 