# Images

* we can adding images in website using `<img>` tag This is an empty element (which means there is no closing tag). It must carry the following two attributes:
  * src:This tells the browser where it can find the image file.
  * alt : This provides a text description of the image which describes the image if you cannot see it.
  * title : You can also use the titleattribute with the `<img>` element to provide additional information about the image.
* You will also often see an `<img>` element use two other attributes that specify its size:
  * height: This specifies the height of the image in pixels.
  * width : This specifies the width of the image in pixels .
* Three Rules for Creating Images:
  * Save images in the right format .
  * Save images at the right size .
  * Use the correct resolution .
* Image Formats: JPEG: Whenever you have many different colors in a picture you should use a JPEG .
* Image Formats: GIF :Use GIF or PNG format when saving images with few colors or large areas of the same color.
* Image Resolution :Images created for the web should be saved at a resolution of 72 ppi.
* Photographs are best saved as JPEGs; illustrations or logos that use flat colors are better saved as GIFs.

# Colors

* The color property allows you to specify the color of text inside an element.
* You can specify any color in CSS in one of three ways:
   1. rgb values
   2. hex codes
   3. color names

 ``` css
h1 {
color: DarkCyan;}
/* hex code */
h2 {
color: #ee3e80;}
/* rgb value */
p {
color: rgb(100,100,90);}
```

* It is important to ensure that there is enough contrast between any text and the background color (otherwise
people will not be able to read your content).
* CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as RGBA.
* CSS3 also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA

# Text

* Typeface Terminology:
  * Serif:Serif fonts have extra details on the ends of the main strokes of the letters.
  * Sans-Serif :Sans-serif fonts have straight ends to letters, and therefore have a much cleaner design.
  * Monospace :Every letter in a monospace (or fixed-width) font is the same width. (Non-monospace fonts have different widths.)
* The font-family property allows you to specify the typeface that should be used for any text inside the element(s) to which a CSS rule applies.
* The font-size property enables you to specify a size for the font.
* The font-weight property allows you to create bold text.
* If you want to create italic text, you can use the font-style property .
* The text-transform property is used to change the case of text giving it one of the following values:
  * uppercase
  * lowercase
  * capitalize
* The text-decoration property allows you to specify the following values:
  * none
  * underline
  * overline
  * line-through
  * blink
* The text-align property allows you to control the alignment of text. The property can take one of four values:
   1. left
   2. right
   3. center
   4. justify
* The text-shadow property It is used to create a drop shadow, which is a dark version of the word just behind it and  slightly offset.

* 
