# easyScrollTo
A small plug-in JS script for nav bars and buttons, allowing links to smooth scroll to sections on single page sites.
easyScrollTo.js links buttons or anchor elements with page sections to facilitate easy smooth (or instant) scrolling.
The script requires strict ID naming conventions for the buttons and the sections those buttons target.
<br>
<br>
<h2>Quick Setup</h2>
Set Button/Link IDs
For each button or link that should initiate a smooth scroll to a section, set an ID using the following format
`id="button-[sectionName]";`
Eg

`id="button-contact";`
<ul>
  <li>The buttons or anchor elements used for navigating must;</li>
  <li>These buttons/a elements must each have a unique id in the following format - "button-[sectionName]"</li>
  <li>Each of the page is contained within an element with a unique id formatted - "section-[sectionName]"</li>
</ul>
<br>
Once buttons/anchor elements and page sections have been marked up as described above, clicking on a button/a element will smooth-scroll the viewport to the corresponding section.

<h2>Dependencies</h2>
jQuery <a href="https://jquery.com/download/">(install)</a>





#TODO - more
