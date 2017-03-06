+++
date = "2016-10-05T18:41:44+05:30"
next = ""
prev = ""
title = "Structuring"
toc = true
weight = 1

+++
Getting your site structure correct from the beginning is vital for any new Sass project. One good approach for this is to use Partials.

<u>Using Partials </u>

<ul>
<li>Using partials allows you to break the CSS up into smaller more manageable blocks of code that are easier to maintain and develop. </li>
<li>Place all mixins, functions, placeholders and variables in their relevant partial file.</li>
<li>A Single Sass file can become really huge and messy, use Partials.</li>
</li>Depending on the complexity of the project, you can have sets of partials into smaller categories.</li>
</ul>

<strong>The 7-1 Pattern </strong>

Basically, you have all your partials stuffed into 7 different folders,and a single file at the root level (usually named main.scss) 
which imports them all to be compiled into a CSS stylesheet.Eg:
<pre style="background: #f0f2f4">
Sass/
|
|– base/
|   |– _reset.scss        # Reset/normalize/colors
|   |– _typography.scss   # Typography rules
|   …                     # Etc.
|
|– components/
|   |– _buttons.scss      # Buttons
|   |– _carousel.scss     # Carousel
|   |– _cover.scss        # Cover
|   |– _dropdown.scss     # Dropdown
|   …                     # Etc.
|
|– layout/
|   |– _navigation.scss   # Navigation
|   |– _grid.scss         # Grid system
|   |– _header.scss       # Header
|   |– _footer.scss       # Footer
|   |– _sidebar.scss      # Sidebar
|   |– _forms.scss        # Forms
|   …                     # Etc.
</pre>
Other folders are abstract, vendors, themes and pages.

You can split these partials into smaller groups based on your project structure. 
Some more details on the above mentioned folders.
<ol>
<li> <strong>Base folder</strong> : The base/ folder holds what we might call the boilerplate code for the project. 
In there, you might find the reset file, some typographic rules, and probably a stylesheet defining some standard styles for commonly used HTML elements. </li>

<li><strong>Components folder</strong> : Components/ folder is more focused on widgets. It contains all kind of specific modules like a slider, a loader, a widget, and basically anything along those lines.</li>

<li><strong>Layouts</strong> : The layout/ folder contains everything that takes part in laying out the site or application.
This folder could have stylesheets for the main parts of the site (header, footer, navigation, sidebar…), the grid system or even CSS styles for all the forms. </li>

<li><strong>Pages</strong> : If you have page-specific styles, it is better to put them in a pages/ folder, in a file named after the page.
 For instance, it’s not uncommon to have very specific styles for the home page hence the need for a _home.scss file in pages/. </li>
 
<li><strong>Themes</strong> : On large sites and applications, there is possibility of having different themes. 
There are certainly different ways of dealing with themes one of which is having themes/ folder.

<li><strong>Abstracts</strong> : When working on a very large project with a lot of abstract utilities, it might be interesting to group them by topic rather than type, for instance typography (_typography.scss). The rule of thumb for this folder is that it should not output a single line of CSS when compiled on its own. These are nothing but Sass helpers.

<li><strong>Vendors</strong> : And last but not least, most projects will have a vendors/ folder containing all the CSS files from external libraries and frameworks – Normalize, Bootstrap, jQueryUI, FancyCarouselSliderjQueryPowered, and so on.
 
 <li><strong>Main file</strong> : Including all these partials in the parent file main.scss.
 The main file (usually labelled main.scss) should be the only Sass file from the whole code base not to begin with an underscore. 
 This file should not contain anything but @import and comments.</li>
 </ol>
 
 






 
