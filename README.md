
## Steps to Run the Application ##

1. Clone the git repository https://github.com/jeska10/frontend-nanodegree-mobile-portfolio.git
2. Navigate to index.html in the prod directory 
3. Right click index.html and select open in and select a browser to open the file
4. To navigate to the pizza page click on the Cam's Pizzeria link



## Website Performance Optimization portfolio project

This a website that has been optimized to render as quickly as possible. the optimization steps are listed below.

*reduced size and minified pizzeria.jpg

*minified profilepic.jpg
*minified perfmatters.js
*minified main.js

*index.html 
	inlined google font script
	inlined css files
	made google analytics async

*views/css/style.css - added backface-visibility: hidden

*main.js
	global variable var moverItems = document.getElementsByClassName('mover');. 	
	
	used getELementsByClassName instead of querySelectorAll

	changedPizzaSizes
		removed the variables dx and newwidth from the for loop to reduce the amount of work performed for each iteration of the loop.

	updatePositions 
		removed the calculation of the scroll top value from the for loop
	
		added array phase that stores the 5 different values used for determining style left for the moving pizzas

		added variable to store a collection of pizzas to be referenced each time the page is scrolled.  this code was moved from inside update position to eliminate repeated calls to get the elements.

*views/pizza.html
	inlined css/style.css
	inlined bootstrap-grid.css

