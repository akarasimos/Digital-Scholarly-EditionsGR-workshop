TEI Customization - ODD and schema
========================================================
author: DiXiT Workshop 'Scholarly Digital Editions and Modern Greek Studies'
date: Athens, 24-28 April 2017
autosize: true



CHAPTER 0
=========

# Have we met before?

<img src="images/metbeforeveg.png"/><br/><small><small><small><small>[laundrysoapman25.deviantart.com](http://laundrysoapman25.deviantart.com/art/Have-we-met-before-432485592)</small></small></small></small>


Well formed and valid
========================
<br/>
Remember?
<br/><br/>
- An XML document is well formed when it complies with the XML syntax
<br/><br/>
- An XML document is valid against a **schema**
<br/><br/><br/><br/><br/><br/>


========================
<img src="images/metbeforeveg.png" width="30%"/>
<br/><br/><br/><br/>
## ... Where ?


=======================
<img src="images/teiall.png">

=========================
<img src="images/metbeforeveg.png" width="30%"/>
<br/><br/><br/><br/>
## ... Why ?


A schema
========================
<br/>
## defines **vocabulary** and **grammar**
<br/>
### which elements and attributes are to be used, where and how 
<br/>
e.g. which element you can use inside another element, which values you can give to an attribute


Chapter 1
======================
# TEI Customization


Associate schema to a document
=======================

<img src="images/teiall.png">

***

<img src="images/help.jpg">

Schema helps you!

Suggestions, code completion, pop-up descriptions ...



Associate schema to a document
=========================
<img src="images/teiall.png">


***

<img src="images/angryfingershe.jpg" width="30%">&#8195;
<img src="images/angryfingerhe.jpg" width="30%">

Schema controls you!

Red square, error messages, invalid document ...



===============

<img src="images/angryfingershe.jpg" width="23%">&#8195;&#8195;
<img src="images/help.jpg" width="30%">&#8195;&#8195;
<img src="images/angryfingerhe.jpg" width="23%">
<br/>
<br/>

The good news is . . .
<br/>

## that you can create or adjust the schema !


TEI customization
===================
<img src="images/tei_areas.jpg">

***

Customization of the TEI is motivated by two really important things:

- the **diverse disciplinary needs and concerns** of the TEI community

- The goal of reconciling the need for a **common encoding language** with the need for **expressiveness**


Community-maintained TEI schemas
=========================
<br/>

- **tei\_all** 
- **tei\_lite** (light and basic encoding)
- **tei\_drama** (performance texts)
- **tei\_speech** (speech and spoken texts)

<small>
More at <http://www.tei-c.org/Guidelines/Customization/>
</small>
<br/><br/><br/>
Have you met them before?


Community-maintained TEI schemas
=========================
<br/>

- **tei\_all** 
- **tei\_lite** (light and basic encoding)
- **tei\_drama** (performance texts)
- **tei\_speech** (speech and spoken texts)

<small>
More at <http://www.tei-c.org/Guidelines/Customization/>
</small>
<br/><br/><br/>
Have you met them before? <br/>Yes, they are available in **oXygen** through its TEI framework.


Recap (theory)
========================
<br/>
## A schema defines **vocabulary** and **grammar** 
#### which elements and attributes are to be used, where and how 

# &#8679;

#### it represents in a structured and formalized way
## your **understanding of** and **approach towards** 
## the text to be encoded (scientific choices)

Recap (practice)
=========================
<img src="images/teiall.png">

What happens if you change the schema?



Chapter 2 
=============================
# ODD (One document does it all)


============================
## A TEI Customization
## comes in the form of / is referred as 
## an ODD
<br/><br/><br/>
... What is an ODD?


=========================
## **ODD** (One Document Does it All) 
<br/>

- TEI document (that is a XML document)
- schema (for the machine)
- documentation (for the user, like the Guidelines)

<br/>

=========================
## **ODD** (One Document Does it All) 
<br/>

- TEI document (that is a XML document)
- schema (for the machine)
- documentation (for the user, like the Guidelines)

<br/>

#### E.g. ***tei\_dixit.xml*** or you can change the extension to ***tei\_dixit.odd***


The ODD tree
=============
<img src="images/odd-tree.png">


========================
<img src="images/odd_stack.png">
<small>[A view of the whole system](http://www.wwp.northeastern.edu/outreach/seminars/_current/presentations/basic_odd/basic_odd_simple_tutorial_13.xhtml)</small>
<br/><small><small><small><small>From: Syd Bauman, Julia Flanders, and the Women Writers Project</small></small></small></small>


========================
<img src="images/tei_odd_customization_detail_iconed.png"/>
<small>[TEI customization under the hood (in a nutshell)](http://www.wwp.northeastern.edu/outreach/seminars/_current/presentations/customization/customization_overview_tutorial_12.xhtml)</small>
<br/><small><small><small><small>From: Syd Bauman, Julia Flanders, and the Women Writers Project</small></small></small></small>



Chapter 2
===============
# The TEI bricks


The TEI is ...
===========
<br/><br/>
not only a [big list of elements](http://www.tei-c.org/release/doc/tei-p5-doc/en/html/REF-ELEMENTS.html) ...
<br/><br/><br/>
They are structured in modules and classes

Elements
==============
<br/>
<img src="images/tei_as_lego.png">

***

+/- 550 elements and a very large number of attributes!

Grouped into:

- **modules**

- **classes** 


Modules = lego kits
===================
left: 30%
<br/>
<img src="images/TEI_modules_simple.png">

***
<br/>
- Basic and specialized kits

- Each module corresponds to [a **chapter** in the TEI guidelines](http://www.tei-c.org/release/doc/tei-p5-doc/en/html/index.html)

- Each element belongs to one and only one module


The class system
============================
<br/><br/>
### A class groups elements or attributes that **behave in the same way** and that tend to **go in the same place**.
<br/><br/>
- Classes of elements are named model.*the class* (e.g. **model.global**)

- Classes of attributes are named att.*the class* (e.g. **att.global**)


Examples
============================
<img src="images/tei_classes_conceptual4.png">


The class system
=========================

And now ... [exercise time](https://github.com/DiXiT-eu/Digital-Scholarly-EditionsGR-workshop/blob/master/session09/exerciseClasses.pdf) (3 mins :)


Chapter 3
================
# Customizing the TEI


=====================
## Customization options
<br/>
- Select modules
- Remove unnecessary elements
- Add new elements or attributes
- Change element or attribute names
- Constrain attribute values
- Constrain structure
- Manipulate functional groupings of elements (classes)
- Produce an internationalized version of the TEI


==================================
left:40%

## 1. Create the ODD 
<br/>
- manually writing it
- using [Roma](http://www.tei-c.org/Roma/)

***

============================
left:40%

## 1. Create the ODD 
<br/>
- manually writing it
- using [Roma](http://www.tei-c.org/Roma/)

***

## 2. Generate the schema
(ODD ---> RNG, RNC, DTD, etc.)

- web app  [Roma](http://www.tei-c.org/Roma/)
- oXygen's built-in stylesheets
- Oxford University's [OxGarage](http://oxgarage.oucs.ox.ac.uk:8080/ege-webclient/) multi-transformer
- roma: a command-line tool
- Complete list with links and instructions at WWP [ODD Processors page](http://www.wwp.northeastern.edu/outreach/seminars/_current/presentations/customization/customization_overview_tutorial_13.xhtml)


Let's go to Roma!
=========================
<img src="images/teiRoma.png"/>


Recap
==========================

- ODD Customization reflects your scientific choices, reinforces consistency, documents your work


Recap
==========================

- ODD Customization reflects your scientific choices, reinforces consistency, documents your work

- For creating an ODD Customization <--- manipulate (delete, add, change) the TEI bricks (elements, attributes, modules, classes)



Recap
==========================

- ODD Customization reflects your scientific choices, reinforces consistency, documents your work

- For creating an ODD Customization <--- manipulate (delete, add, change) the TEI bricks (elements, attributes, modules, classes)

- From an ODD Customization ---> generate documentation and schema


Recap
==========================

- ODD Customization reflects your scientific choices, reinforces consistency, documents your work

- For creating an ODD Customization <--- manipulate (delete, add, change) the TEI bricks (elements, attributes, modules, classes)

- From an ODD Customization ---> generate documentation and schema

- A TEI document should be well formed (XML rules) and valid (schema rules)


Credits and links
==============
<small>

These slides reuse materials from

- the TEI-C resources, and in particular
  - <http://www.tei-c.org/Guidelines/Customization/odds.xml>

- the Women Writers Project educational resources, and in particular
  - <http://www.wwp.northeastern.edu/outreach/resources/customization.html>

  Please visit these links if you want to know more!
</small>

==========
<small>Elena Spadini</small>

DiXiT Workshop ['Scholarly Digital Editions and Modern Greek Studies'](https://dixit-eu.github.io/Digital-Scholarly-EditionsGR-workshop/)

Athens, 24-28 April 2017

<small>Licence: [CC-BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)</small>

