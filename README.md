# easyScrollTo
A small plug-in JS script for nav bars and buttons, allowing links to smooth scroll to sections on single page sites.<br>
easyScrollTo.js links buttons or anchor elements with page sections to facilitate easy smooth (or instant) scrolling.<br>
The script requires strict ID naming conventions for the buttons and the sections those buttons target.<br>
**This was just a fun little problem I wanted to optimise for my own reuse across projects. If it makes your life easier, great!**
<br>
<br>
<h2>Quick Setup</h2>

**Set Button Class**
For each button or link that should initiate a smooth scroll to a section, set

`class="button"`

**Set Button IDs**<br>
For each button or link that should initiate a smooth scroll to a section, set an ID.
The ID should follow the format of button-[sectionName]. The button- prefix will be consistent across all naviagational buttons (or anchor elements), and the [sectionName] prefix should change based on the name of the section we want to link this button to.

`id="button-[sectionName]";` <br> <br>
Eg<br>
`id="button-footer";`

**Set anchor href target to javascript** <br>
If using anchor elements for page navigation, set the href attribute for each:

`href="javascript:;"`

**Set Section IDs** <br>
For each section that should be the target of a smooth scroll, set an ID. As with the button elements, the prefix remains the same across all sections ("section-") and the suffix will change based on the name or function of the section.

`id="section-[sectionName]";` <br>
Eg <br>
`id="section-footer";`

**Incorporate easyScrollTo**
Download easyScrollTo.js and place in your site's script folder
```html
<head>
  <script src="scripts/easyScrollTo.js"></script>
</head>
```

**Done**
You're done! The script will match button IDs with section IDs, and will 

<h2>Implementation Example</h2>
The below sets up a simple page with an anchor link that takes the user to a footer section when clicked.

```html
<html>
  <head>
    <script src="scripts/jquery-3.6.0.js"></script>
    <script src="scripts/easyScrollTo.js"></script>
  </head>

  <body>
    <nav>
      <a class="button" id="button-footer" href="javascript:;">
        Footer
      </a>
    </nav>
    
    // Page Content
    <div style="height:1500px";></div>
    
    <div id="section-footer">
      Footer content
    </div>
  </body>
</html>
```

<h2>Dependencies</h2>
jQuery <a href="https://jquery.com/download/">(install)</a>
