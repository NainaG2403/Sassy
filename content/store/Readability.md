+++
date = "2016-10-05T19:00:50+05:30"
next = ""
prev = ""
title = "Readability"
toc = true
weight = 9

+++

Indentation & Readability <br>
Sass initially described a syntax of which the defining characteristic was its indentation-sensitivity.<br>
Soon enough, Sass maintainers decided to close the gap between Sass and CSS by providing a CSS-friendly syntax called SCSS for Sassy CSS. <br>

•	Two (2) spaces indents, no tabs <br>
•	Ideally, 80-characters wide lines <br>
•	Properly written multi-line CSS rules <br>
•	Meaningful use of whitespace. <br>

 // That's Right !! <br>
 <pre style="color:white">
.foo {
  display: block;
  overflow: hidden;
  padding: 0 1em;
}
</pre>

// Not a Good one <br>
<pre style="color:white">
.foo {
    display: block; overflow: hidden;
			padding: 0 1em;
}
</pre>

