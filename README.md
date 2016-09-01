# Performance Optimization 
The goal of this project was to optimize the performance of a [given website](https://github.com/udacity/frontend-nanodegree-mobile-portfolio). 

## Optimizations
The `index.html` file was modified in order to achieve a score of 90 or higher 
when evaluated by [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/).

The optimizations made include:
- Add CSS media queries for special cases (22)
- Inline key CSS (26 - 75)
- Make loading of Google fonts async (78 - 85)
- Make JS Google Analytics (88 - 97)
- Reduce image size and optimize image (133) -->

Result:

![Alt text](/img/PSAfter.png?raw=true "Optional Title")


The `views/js/main.js` file was modified in order to achieve a consistent frame-rate
of 60fps when scrolling on the views/pizza.html page.

The optimizations made include: 
- Replace querySelector with getElementById (412 - 418)
- Replace querySelectorAll with getElementsByClassName and 
  move variable out of for loop in changePizzaSizes() (454)
- Replace querySelectorAll with getElementsByClassName and 
  move variable out of updatePositions() (506)
- Move bodyScrollTop variable out of the function for loop (514)

Result:

![Alt text](/img/FPSAfter.png?raw=true "Optional Title")

## To view the optimized website
Open the optimized website [here](https://miguelamartinez.github.io/performance-optimization/). 
