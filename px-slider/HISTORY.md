v0.6.4
=================
* Update dependencies

v0.6.3
=================
* Made positioning work with shadow DOM
* made value default to min if not init; removed throw error
* added check to flip max and min if max < min

v0.6.2
=================
* added support for negative values

v0.6.1
=================
* made it so disabled actually does something
* added unit tests
* fixed issues in demo (description, resize)
* cleaned up and simplified code (comments, reflect, public to private API, event complexity)

v0.6.0
=================
* uprev

v0.5.9
=================
* added codepen

v0.5.8
=================
* fixed demo bugs

v0.5.7
=================
* updated mega demo styles and bower px-demo-snippet to ^

v0.5.6
=================
* updated demos-snippets

v0.5.5
=================
* removed broken example

v0.5.4
=================
* added image to readme, removed watch, added view on github

v0.5.3
=================
* updated gh-pages script to vulcanize demo

v0.5.2
=================
* Enabled api viewer

v0.5.1
=================
* Updated to new demo

v0.5.0
=================
* Upgrade to Polymer 1.5.0

v0.4.3
=================
* added oss_notice to bower ignore

v0.4.2
=================
* added pull request test for travis and updated OSS Notice

v0.4.1
=================
* added auto github pages functionality

v0.4.0
=================
* Upgrade to Polymer 1.4.0

v0.3.2
=================
* updated README and put a link to full API on the GH-pages.

v0.3.1
=================
* edited readme

v0.3.0
=================
* implemented the iron-resizable-behavior behavior

v0.2.4
==================
* Updated License

v0.2.3
==================
* fixed a bug where sometimes, moving a multihandle to match the value of the other handle caused the other handle to jump
* removed obsolete "demo bugs" from the demo page.
==================
v0.2.2
==================
* fixed a bug in Firefox which allowed the user to drag the image of the handle instead of the handle
* fixed a bug in IE where ClassList (which is called by Polymer in toggleClass) cannot be used on an SVG element.
==================
v0.2.1
==================
* implemented redesign of the multi-slider to prevent overlapping handles
* fixed a strange rounding error when floating point numbers that caused value to flicker in input box
* improved displayed rounding in input box to match number of decimals in the step attr
==================
v0.0.1
==================
* Initial release
