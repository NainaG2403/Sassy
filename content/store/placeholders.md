+++
date = "2016-10-05T18:53:35+05:30"
next = ""
prev = ""
title = "Placeholders"
toc = true
weight = 5

+++

Placeholders -- The Extend Keyword
<ol>
<li>Unlike mixins, placeholders can be used multiple times without adding any duplicate code.This makes them a much friendlier option for outputting DRY CSS</li>
<li>Including a mixin is the same as copying and pasting the styles throughout the CSS file. It creates a mass of duplicate code and can bloat your CSS file.</li>
<li>The repeated code in the placeholder is output only once with only the unique styles being applied to the individual selectors.</li>
<li>If unused, the placeholder styles are not output at all.
</ol>

Take an example of usage of  Extend keyword & how it works 
<pre style="color:white;">
%center {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
</pre>

<pre style="color:white;">
.container {
  @extend %center;
}
</pre>

Placeholders and Mixins together help to reduce code duplication.

