## Website Performance Optimization portfolio project

How to Run the Application:
============================

Viewing the Live Site:
=======================
1. Point your browser to [https://contactron.github.io/web-optimization-project/index.html]


Optimizations Made:
=======================

Part 1: Optimize PageSpeed Insights score for index.html
 - Resized/compressed image files (multiple times)
 - Separated out the CSS for printing from the main CSS
 - Added asynchronous loading of all analytics scripts
 - Used webfont loader to load Google Fonts
 - Minified Index.html, print.css, and perfmatters.js
 - Inlined style.css

Part 2: Reduce time to resize pizza to 5ms or under (changes made to main.js)
 - Removed redundant code by having one function update the pizza size label and calculate the percentage width.
 - Moved pizza size dx and newwidth calcuations out of the for loop
 - Created new object to hold all the pizzas that need to be changed so they don't have to be called within the loop

Part 3: Optimize Frames per Second in pizza.html (changes made to main.js)
 - Moved code to capture the amount of scrolling (scrolltop) out of the loop that updates pizza positions
 - Used transformX functions to improve efficiency of pizza repositioning
 - Created new img for background pizzas (pizza_small.png) and scaled it to the correct size. Removed code to dynamically resize when created from main.js
 - Moved updatePositions into window.requestAnimationFrame to reduce paint cycles
 - Use.getElementByClassName to more efficiently parse the DOM for the mover class.

