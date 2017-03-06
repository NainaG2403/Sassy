+++
date = "2016-10-05T18:53:00+05:30"
next = ""
prev = ""
title = "Variables"
toc = true
weight = 3

+++

Variables in Sass

Variables are used to store information such as color, font-size, CSS styles etc. They can be reused as many times as you wish to in your program.
Variables are defined with dollar sign ($) and ends with semicolon (;) having syntax as shown below :<br/>

<strong style="background-color:yellow;">$variable_name : some value; </strong>

Some examples are : <br/>
$font-stack:    Helvetica, sans-serif;<br/>
$primary-color: #333;

How do variables help :
Sass helps to keep your code non-repetitive, which makes it easy to maintain and change.
When the Sass is processed, it takes the variables we define for the $font-stack and $primary-color and outputs normal CSS with our variable values placed in the CSS. 
This can be extremely powerful when working with brand colors and keeping them consistent throughout the site.<br/>
For example :
You can use $font-stack and $primary-color as shown.

body {
  font: 100% $font-stack;
  color: $primary-color;
}

<strong> Sass Variable Scope </strong>

Sass supports two types of variables: local variables and global variables.

<u>Global Variables:</u>

By default, all variables defined outside of any selector are considered global variables. That means they can be accessed from anywhere in our stylesheets.<br/>
For example,
$font-color: #fff;

<u>Local Variables:</u>

Local Variables are those which are declared inside a selector. If you wish to override the values of the global variables you can do it in the local variables.<br/>
For example,
.section_one {
color: #555;
background-color: $font-color;
}









