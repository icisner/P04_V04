## Website Performance Optimization portfolio project

### Getting started

####Part 1: Optimize PageSpeed Insights score for index.html

These are some things that I tried to improve speed in **index.html**:

1. Minify CSS files **print.css**, **style.css** using some web base tools like listed bellow:

    * [CSS Minifier](https://cssminifier.com/)
    * [Clean CSS](http://www.cleancss.com/css-minify/)
    * [CSS Compressor](http://csscompressor.com/)
    
      Saving about 338 ms 
      ![/img/CSS_1.jpg]
    
2. Minify JS files **perfmatters.js** using web tools like these:

   * [JS Compress](http://jscompress.com/)
   * [JS Minifier](https://javascript-minifier.com/)
    
      Saving about 172 ms 
      !(A)[../img/JS_1.jpg]
   
3. Copy analytics.js file from (google analytics)[http://www.google-analytics.com/analytics.js] and Minify
   * Moving file and inlining analytics.js saved about 70ms
      !(A)[../img/analytics_js.jpg]

1. Open a browser and visit localhost:8080
1. Download and install [ngrok](https://ngrok.com/) to make your local server accessible remotely.

  ``` bash
  $> cd /path/to/your-project-folder
  $> ngrok http 8080
>>>>>>> origin/master
  ```

Tools to optimzed pictures used was Corel PaintShop Pro X4 using resize menu and Optimizer tool under Filse save us -> options
Tools to minify css https://cssminifier.com/ (I tried grunt but had some issues with addins so decided to use web tools)
Tools to minify js https://javascript-minifier.com/ (I tried grunt as well but had some issues so decided to use web tools)


	Page loaded at GitHub http://icisner.github.io/
	Page speed test 94% for Mobile and 95% in Desktop


####Part 2: Optimizing Frames per Second in pizza.html

	These are some things done to optimze views/js/main.js
	1.- Optimized pizza.jpg to reduce from 49Kb to 24Kb
	2.- Reducing math operations and creating vectors to speed up loop  line 548
	3.- Reducing number of pizza for scrolling in line 551 from 200 to 32
	4.- Optimized images to ~ 5Kb

	Page loaded at GitHub http://icisner.github.io/views/pizza.html

####Part 3 Optimizing speed for size change in pizza.html

	These are some things done to optimze views/js/main.js
	1.- Removing some variables from loop in line 513 to speed up process
	2.- Removing some variables from loop in line 457 to speed up process

	Page loaded at GitHub http://icisner.github.io/views/pizza.html

	These are some things done to optimze index.html


	1.- Inline style.css, print.css 
	2.- Moving in and Inline  analytics.js, perfmatters.js, perfmatters.js
	3.- Copied pizzeria.jpg to pizzeria_v1.jpg reducing to 19Kb
	4.- Optimized images to ~ 5Kb

