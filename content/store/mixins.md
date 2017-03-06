+++
date = "2016-10-05T18:53:26+05:30"
next = ""
prev = ""
title = "Mixins"
toc = true
weight = 4

+++

Mixins

A Mixin is a block of code that lets us group CSS declarations we may reuse throughout our site.
Some things in CSS are a bit tedious to write, especially with CSS3 and the many vendor prefixes that exist.<br/>
Mixins make groups of CSS declarations that we can reuse throughout our site. Instead of typing the same property over and over we write a mixin once then call that mixin anytime we want to use it. 

A mixin lets you make groups of CSS declarations that you want to reuse throughout your site. You can even pass in values to make your mixin more flexible.<br/>
A good use of a mixin is for vendor prefixes. Here's an example for border-radius.
 

To declare a mixin we use the @mixin keyword. We then give it a name and apply our styles in between curly braces like so:
<br/>
<pre style="color:white">
@mixin box-sizing <br/>
{ 
-webkit-box-sizing: border-box;
-moz-box-sizing: border-box;
 box-sizing: border-box; 
 } 
</pre>
You can include it using @include box-sizing;
<br/>

A mixin is a great way to include sections of code multiple times within a site. But including a mixin is the same as copying and pasting the styles throughout the CSS file. It creates a mass of duplicate code and can bloat your CSS file.
A mixin therefore should only be used if an argument is present, to quickly create modified styles. <br/>
Good Usage of Mixin would be : 
<pre style="color:white">
@mixin border-radius($radius) {
  -webkit-border-radius: $radius;
     -moz-border-radius: $radius;
      -ms-border-radius: $radius;
          border-radius: $radius;
}

.box { @include border-radius(10px); }

</pre>





