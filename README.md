## Trevor's fork for use with GitHub pages

## Website Performance Optimization portfolio project

This is my attempt for Project 4. The main page is in app/index.html.

You can view the html locally, use `grunt serve` for local development, or use `npm install && grunt` to build a version suitable for Production.

The file views/js/main.js has a number of improvements to speed up views/pizza.html
* changePizzaSizes() - pull calculations out of the for loop for faster resize
* updatePositions() - move call to scrollTop to avoid render thrashing and better scroll
* document.addEventListener - create a dynamic number of pizzas instead of 200