# HTML5 Layout
* The new HTML5 elements indicate the purpose of  different parts of a web page and help to describe 
its structure.
* The new elements provide clearer code (compared 
with using multiple ``` <div> ``` elements).
* Older browsers that do not understand HTML5 
elements need to be told which elements are 
block-level elements.
* To make HTML5 elements work in Internet Explorer 8 
(and older versions of IE), extra JavaScript is needed, 
which is available free from Google.
## Headers & Footers:
The ``` <header>``` and ```<footer>```
elements can be used for:
* The main header or footer 
that appears at the top or 
bottom of every page on the 
site.
* A header or footer for an 
individual ```<article> ```or 
```<section>``` within the page.
## Navigation ```<nav>```:
 is used to 
contain the major navigational 
blocks on the site such as the 
primary site navigation.
## Articles```<article>```
The <article> element acts as 
a container for any section of a 
page that could stand alone and 
potentially be syndicated.
## Asides ```<aside>```
When the ```<aside>``` element 
is used inside an ```<article>```
element, it should contain 
information that is related to the 
article but not essential to its 
overall meaning. <br>
When the ```<aside>``` element is 
used outside of an ```<article>```
element, it acts as a container 
for content that is related to 
the entire page.
## Sections ```<section>```
The ```<section>``` element groups 
related content together, and 
typically each section would 
have its own heading.
## To make HTML5 elements work in Internet Explorer
``` html 
<!--[if lt IE 9]>
<script src="http://html5shiv.googlecode.com/svn/
 trunk/html5.js"></script>
<![endif]-->
```
