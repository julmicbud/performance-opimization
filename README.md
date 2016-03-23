## Website Performance Optimization portfolio project

This is my Project 4 Website Optimization Project.

This project is online at http://julmicbud.github.io/

I used Chrome dev tools and PageSpeed Insights score to test the optimization of this site.

### Getting started

####Part 1: Optimize PageSpeed Insights score for index.html

PageSpeed Insights are now:

	mobile: 93/100
	desktop: 94/100
	
 - the google font now loads asynchronously.
 - extracted and inlined critical-path CSS from the style.css in index.html
 - added media=print to the link tag for print.css so it does not block page rendering
 - edited the size of the image pizzeria.jpg so it would not take so long to load
 - edited the size of the image profilepic.jpg so that it would have a faster load time
	

####Part 2: Optimize Frames per Second in pizza.html
	
	in updatePositions()
	- changed querySelectorAll to getElementsByClassName for efficency
	- moved phase variable outside of loop
	- moved scrollTop outside of the loop and made it a new variable
	
	DOMContentLoader
	- made a varible maxPizzas to hold the number of rows * cols on the page
	- then used this to maxPizza variable to determine the number of times the to loop the pizzas.
	- this way the number of pizzas is not always 200 it is more specific for the screen size
	


###Part 3: Resizing pizzas

	- determineDx now uses percentages instead of exact pixels. This will make it more fluid for the screen types
	- changePizzaSizes() is now a simple code that called resizePizzas()
		-now there for loop only has one line which assigns a new width to the random pizza containers
		
	-combined changeSliderLabel() and sizeSwitcher() so now they will both happen at the same time
	
###courses used

Website Preformance Optimization
and
Browser Rendering Optimization 