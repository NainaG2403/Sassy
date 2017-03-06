+++
date = "2016-10-05T19:00:15+05:30"
next = ""
prev = ""
title = "Nesting"
toc = true
weight = 6

+++

Nesting in Sass : <br/>
While nesting upto certain level perfectly makes sense, it should not be made as a default option.
To ensure the CSS output is clean and reusable, we need to avoid misuse of nesting.

Overusing nested rules in Sass can cause a lot of issues, from complex code to over-specificity and too much reliance on the HTML structure of a page. <br/>
These things can cause issues further down the line and potentially increase the need for the inclusion of !important, which should generally be avoided.
<br/>

Here are some golden rules for nesting:
<ul>
<li>Never go more then 3 levels deep. </li>
<li>Ensure the CSS output is clean and reusable.</li>
<li>Use nesting when it makes sense to, not as a default option.</li>
</ul>

Hence Nesting should be limited to 3 levels. 






