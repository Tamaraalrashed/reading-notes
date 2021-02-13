# ** Introductory HTML and JavaScript**

## How the web works:
When you visit a website, the web server
hosting that site could be anywhere in the
world. In order for you to find the location of
the web server, your browser will first connect
to a Domain Name System (DNS) server.

## HTML describeS the Structure of Pages:
1. ` <title> `: Anything written between the
`<title>` tags will appear in the
title bar (or tabs) at the top of
the browser window.
1. `<head>`: Before the `<body>` element you
will often see a `<head>` element.
This contains information
about the page 
1. `<body>`: Anything written between
the `<body>` tags will appear
in the main browser window.
<br>

**Opening tags can carry attributes, which tell us more
about the content of that element, attributes require a name and a value.**

- ``DOCTYPE`` *tell browsers which version of HTML you
are using.*
-  *You can add comments to your code between the
`<!-- and -->` markers.*
-  *The ID and class attributes allow you to identify
particular elements.*
-  *The `<div>` and `<span>` elements allow you to group
block-level and inline elements together.*
-  *<`iframes>` cut windows into your web pages through
which other pages can be displayed.*
-  *The `<meta>` tag allows you to supply all kinds of
information about your web page.*
-  *Escape characters are used to include special
characters in your pages such as <, >, and ©.*
<br>

### *The new HTML5 elements indicate the purpose of different parts of a web page and help to describe its structure.*
- *The new elements provide clearer code (compared
with using multiple <div> elements).*
- *Older browsers that do not understand HTML5
elements need to be told which elements are
block-level elements.*
- *To make HTML5 elements work in Internet Explorer 8
(and older versions of IE), extra JavaScript is needed,
which is available free from Google.*

***WHO IS THE SITE FOR?***

Every website should be designed for the target audience—not just for yourself or the site owner. It is therefore very important to understand who your target audience is.


***WHY PEOPLE VISIT YOUR WEBSITE?***

Now that you know who your visitors are, you need to consider why they are coming. While some people will simply chance across your website, most will visit for a specific reason.
You should know if the website is for individuals or for on company, this helps you to know how you can do your work perfectly many things such as ages or age range of the targeted people, what is the average of their income, the size of the company and their budget. 


- Key Motivations such as:
 Are they looking for general entertainment or do they need to achieve a specific goal?
- Specific Goals:
Are they already familiar with the service or product that you offer or do they need to be introduced to it?

***What Your Visitors are Trying to Achieve?***

It is unlikely that you will be able to list every reason why someone visits your site but you are looking for key tasks and motivations. This information can help guide your site designs.
First you want to create a list of reasons why people would be coming to your site, let’s check two of them:
1.	Jasper had a bad experience staying in a hotel when visiting Sydney, Australia, and wants to make a complaint
1.	Ivy is a picture editor and wants to look at a photographer's site to see examples of his work before deciding whether to commission him.


***What Information Your Visitors Need?***
You know who is coming to your site and why they are coming, so now you need to work out what information they need in order to achieve their goals quickly and effectively.
You may want to offer additional supporting information that you think they might find helpful. Look at each of the reasons why people will be visiting your site and determine what they need to achieve their goals.


***HOW OFTEN PEOPLE WILL VISIT YOUR SITE?***
Some sites benefit from being updated more frequently than others. Some information (such as news) may be constantly changing, while other content remains relatively static.
A website about fashion trends will need to change a lot more frequently than one that is promoting a service that people do not buy regularly (such as domestic plumbing or double glazing).


***SITE MAPS***
Now that you know what needs to appear on your site, you can start to organize the information into sections or pages.
The aim is to create a diagram of the pages that will be used to structure the site. This is known as a site map and it will show how those pages can be grouped.

![image](/home/tamara/Reading-notes/sitemap.PNG)

***WIREFRAMES:***

A wireframe is a simple sketch of the key information that needs to go on each page of a site. It shows the hierarchy of the information and how much space it might require.

# ***Java Script***

## _We need to open a website and use it easily, in other words we need something to interact with us while browsing, the anonymous soldier whose resposibilty is that interactive is JAVA SCRIPT LANGUAGE which we will talk about:_

-  **ACCESS CONTENT**: *You can use JavaScript to select any element attribute , or text from an HTML page .*
- **MODIFY CONTENT**: *You can use JavaScript to add elements , attributes , and text to the page , or remove them . *
- **PROGRAM RULES**: *You can specify a set of steps for the browser to follow ( like a recipe ) . which allows it to access or change the content of a page .*
- **REACT TO EVENTS**: *You can specify that a script should run when a specific event has occurred . For example , it could be run when:*
  - A button is pressed.
  - A link is clicked ( or tapped ) on .
  - A cursor hovers over an element.
  - Information is added to a form.
  - An interval of time has passed.
  - A web page has finished loading.

  ## ***A SCRIPT IS A SERIES OF INSTRUCTIONS A script is a series of instructions that a computer can follow to achieve a goal .***

 *Scripts are made up of instructions a computer can follow step - by - step .* <br>
  *A browser may use different parts of the script depending on how the user interacts with the web page .*<br>
  *Scripts can run different sections of the code in response to the situation around them .*

  ## ***Start with the big picture of what you want to achieve , and break that down into smaller steps:***
   1.  DEFINE THE GOAL First , you need to define the task you want to achieve . You can think of this as a puzzle for the computer to solve.
   1. DESIGN THE SCRIPT: To design a script you split the goal out into a series of tasks that are going to be involved in solving this puzzle . This can be represented using a flowchart . You can then write down individual steps that the computer needs to perform in order to complete each individual task ( and any information it needs to perform the task ) , rather like writing a recipe that it can follow .
   1. CODE EACH STEP: Each of the steps needs to be written in a programming language that the computer understands.In our case , this is JavaScript.

   ## ***EXPRESSIONS***
   <br>
    An expression evaluates into ( results in a single value . Broadly speaking there are two types of expressions :
   <br>
   1. Expressions that just assign a value to a variable.
   <br>
   > For example: var color = ' beige ' ; The value of color is now beige.
   1. expressions that use two or more values to return a single value.
   > For example : var area = 3 * 2 ; The value of area is now 6.
   <br>

   ## ***OPERATORS***
   <br>
    Expressions rely on things called operators ; they allow programmers to create a single value from one or more values

   ### ***ARITHMETIC OPERATORS***

   ![img](mathoperator.PNG) 

   ### ***STRING OPERATOR There is just one string operator : the + symbol . It is used to join the strings on either side of it .***

   >For example , you might have a first and last name in two separate variables and want to join them to show a full name . In this example , the variable called fullName would hold the string ' Ivy Stone'.

   <br>

    ## ***FUNCTIONS & METHODS*** 

    - ***Functions consist of a series of statements that have been grouped together because they perform a specific task . A method is the same as a function , except methods are created inside and are part of an object.***
    - ***Functions let you group a series of statements together to perform a specific task . If different parts of a script repeat the same task , you can reuse the function .***

   

