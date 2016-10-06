+++
date = "2016-10-05T18:41:44+05:30"
next = ""
prev = ""
title = "Structuring"
toc = true
weight = 1

+++

Structuring in Sass

Getting your site structure correct from the beginning is vital for any new Sass project. 
Using partials allows you to break the CSS up into smaller more manageable blocks of code that are easier to maintain and develop.
Place all mixins, functions, placeholders and variables in their relevant partial file. <br/>
<u>The 7-1 Pattern</u>
Basically, you have all your partials stuffed into 7 different folders, and a single file at the root level (usually named main.scss) which imports them all to be compiled into a CSS stylesheet. Eg :

<img src="..\Tree.png" ></img><br/>
Other folders are abstract, vendors, themes and pages.

<b>What have we learnt, what do we know : </b> <br/>
A Single Sass file can become really huge and messy, use Partials.<br/>
Depending on the complexity of the project, you can have sets of partials into smaller categories.<br/>




 
