# Problem Domain, Objects, and the DOM.

## Problem Domain:
 Understanding The Problem Domain Is The Hardest Part Of Programming:

Programming is easy if you understand the problem domain,
Most of the work at the time was basic waterfall development. 
you can do one of two things:

1. Make the problem domain easier.
1. Get better at understanding the problem domain.

- take a part of the problem and fully understand that part before expanding the problem domain.


## Object Literals:
Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names.

*CREATING·OBJECTS USING
LITERAL NOTATION*

![img](./images/creatingobject.JPG)


## The DOM:
The Document Object Model (DOM) specifies
how browsers should create a model of an HTML
page and how JavaScript can access and update the
contents of a web page while it is in the browser window.<br>
- MAKING A MODEL OF THE
HTML PAGE<br>
When the browser loads a web page, it
creates a model of the page in memory.
- ACCESSING AND CHANG ING
THE HTML PAGE:<br>
The DOM also defines methods and
properties to access and update each
object in this model, which in turn updates
what the user sees in the browser.

-THE DOM TREE IS A
MODEL OF A WEB PAGE:<br>
As a browser loads a web page, it creates a model of that page.
The model is called a DOM tree, and it is stored in the browsers' memory.
![img](./images/DOMtree.JPG) <br>


It consists of four main types of nodes:
1. THE DOCUMENT NODE:When you access any element, attribute, or text
node, you navigate to it via the document node. It is
the starting point for all visits to the DOM tree.
1. ELEMENT NODES:
HTML elements describe the structure of an HTML
page. (The ``<hl > - <h6>`` elements describe what
parts are headings; the`` <p> ``tags indicate where
paragraphs of text start and finish; and so on.)

***Each node is an object with methods and properties.
Scripts access and update this DOM tree (not the source HTML file).
Any changes made to the DOM tree are reflected in the browser.***
1. ATTRIBUTE NODES:
The opening tags of HTML elements can carry
attributes and these are represented by attribute
nodes in the DOM tree.
1. TEXT NODES:
Once you have accessed an element node, you
can then reach the text within that element. This is
stored in its own text node.

**WORKING WITH
THE DOM TREE:**<br>
Accessing and updating the DOM tree involves two steps:
1. Locate the node that represents the element you want to work with.
1. Use its text content, child elements, and attributes.


*SELECTING ELEMENTS
USING ID ATTRIBUTES:*
get El ementByi d() allows you
to select a single element node
by specifying the value of its
id attribute.<br>
![img](./images/getelementbyID2.JPG) <br>

*SELECTING AN ELEMENT
FROM A NODELIST*
- THE item()METHOD: 
![img](./images/nodelistitem.JPG) <br>


- ARRAY SYNTAX:
![img](./images/nodelistarray.JPG) <br>

[Back to homepage](./readme.md)



*SELECTING ELEMENTS
USING CLASS ATTRIBUTES:*
![img](./images/byclassname1.JPG) <br>
![img](./images/byclassname2.JPG) <br>


*SELECTING ELEMENTS
BY TAG NAME:*
![img](./images/bytag1.JPG) <br>
![img](./images/bytag2.JPG) <br>

*SELECTING ELEMENTS
USING CSS SELECTORS:*
![img](./image/scssselectors1.JPG) <br>
![img](./images/cssselectors2.JPG) <br>

*LOOPING THROUGH
A NODELIST:*
![img](./images/loopingnodelist.JPG) <br>
![img](./images/loopingnodelist2.JPG) <br>

*LOOPING THROUGH
A NODELIST:play-by-play*
![img](./images/playbyplay.JPG) <br>

*TRAVERSING THE DOM:*
When you have an element node, you can select
another element in relation to it using these five
properties. This is known as traversing the DOM.
 parentNode, previousSibling
nextSibling, firstChild and
lastChild.

*WHITESPACE NODES:* Traversing the DOM can be difficult because
some browsers add a text node whenever they
come across whitespace between elements.

*ACCESS & UPDATE A TEXT
NODE WITH NODEVALUE*
![img](./images/nodevalue.JPG) <br>


*ACCESSING & CHANGING
A TEXT NODE*
![img](./images/textnode.JPG) <br>
![img](./images/textnode2.JPG) <br>

*ACCESSING TEXT ONLY*
![img](./images/textonly1.JPG) <br>
![img](./images/textonly2.JPG) <br>

*UPDATE TEXT & MARKUP:*


*ADDING AN ELEMENT TO
THE DOM TREE*
![img](./images/add1.JPG) <br>
![img](./images/add2.JPG) <br>

*REMOVING AN ELEMENT
FROM THE DOM TREE*
![img](./images/remove1.JPG) <br>
![img](./images/remove2.JPG) <br>

**ATTRIBUTE NODES**
*CHECK FOR AN ATTRIBUTE
AND GET ITS VALUES*
![img](./images/CHECK1.JPG) <br>
![img](./images/CHECK2.JPG) <br>

*CREATING ATTRIBUTES &
CHANGING THEIR VALUES*
![img](./images/CREATING1.JPG) <br>
![img](./images/CREATING2.JPG) <br>


*REMOVING ATTRIBUTES*
![img](./images/removingattribute.JPG) <br>



[Back to homepage](./readme)