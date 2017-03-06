+++
date = "2016-10-05T19:00:26+05:30"
next = ""
prev = ""
title = "Looping"
toc = true
weight = 7

+++

Looping in SASS :

Looping in Sass provide flow and logic and give you a finite level of decision making required by mixins and functions.
They can be implemented easily and make Sass look like a real programming language.

When and Why to use SASS : <br/>
Unless there is some medium to complex logic in the code, there is no need for conditional statements in everyday stylesheets. 
Actually, they mainly exist for libraries and frameworks.
However, while using the conditional statements please follow the guidelines given below: <br/>
<ul>
<li>No parentheses unless they are necessary;</li>
<li>Always an empty new line before @if; </li>
<li>Always a line break after the opening brace ({); </li>
<li>@else statements on the same line as previous closing brace (}). </li>
<li>Always an empty new line after the last closing brace (}) unless the next line is a closing brace (}). </li>
</ul>

Different types of looping in Sass:

<h5>For Loop: </h5>
The @for loop makes it possible to repeat a block of code n times, from a start index to an end index. 
The usual syntax for this loop is:
<pre style="color:white;">
@for $i from 1 through 20 {
    // your Styles here
}
</pre>

<h5>Each Loop:</h5>
The @each loop is the ideal ally when having to loop over a list or a map. Indeed, this loop gives the ability to iterate over all items from a list or all pairs from a map using a variable to refer to the current item. <br/>
The usual syntax for this loop is:
<pre style="color:white;">
@each $heading, $size in $headings {
// your Styles here
}
</pre>


<h5>While Loop:</h5>
While the @while loop might look like a weird tool, it actually makes perfect sense when you think about it. In everyday life, it is not uncommon to tell “do something until something else happens”, such as “wash it until it’s clean” for instance. This is exactly what the @while loop does.<br/>
The usual syntax for this loop is:
<pre style="color:white;">
while $num > 0 {
// your Styles here
}
</pre>


