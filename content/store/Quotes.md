+++
date = "2016-10-05T19:01:12+05:30"
next = ""
prev = ""
title = "Using Quotes ?"
toc = true
weight = 8

+++

Using Quotes is not necessary in Sass. <br>
But there is no valid reason to not quote strings.
It is recommended to use quotes to maintain consistency with other languages, including CSS's cousin JavaScript.<br>

There are several reasons for this choice: <br>
•	CSS color names are treated as colors when unquoted, which can lead to serious issues <br/>
•	Most syntax highlighters will choke on unquoted strings <br>
•	It aids general readability <br>

<strong style="font-style:italic"> Some examples 
</strong><br>

// Good Practise 	<br>
$direction: 'left'; <br>

// Bad Practise		<br>
$direction: left;






