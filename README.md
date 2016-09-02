# Performance Optimization 
The goal of this project was to optimize the performance of a [given website](https://github.com/udacity/frontend-nanodegree-mobile-portfolio). 

## Optimizations
The `index.html` file was modified in order to achieve a score of 90 or higher 
when evaluated by [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/).

The optimizations made include:
- Add CSS media queries for special cases (22)
- Inline key CSS (26 - 75)
- Make loading of Google fonts async (78 - 85)
- Make JS Google Analytics async (88 - 97)
- Reduce image size and optimize image (133) 

Before optimization: 

![Alt text](/img/PSBefore.png?raw=true "Optional Title")

After optimization: 

![Alt text](/img/PSAfter.png?raw=true "Optional Title")

The `views/js/main.js` file was modified in order to achieve a consistent frame-rate
of 60fps when scrolling on the views/pizza.html page, and to achieve a time of pizza
resize (when we move the slider to change pizza sizes, it is shown in the the console)
of less than 5 ms.

The optimizations made include: 
- Replace querySelector with getElementById in changeSliderLabel()(419 - 425)
- Replace querySelector with getElementById in determineDx() (438)
- Replace querySelectorAll with getElementsByClassName and move variable 
  PizzaContainerItems out of for loop in changePizzaSizes() (462)
- Place variables dx and newwidth out of for loop in changePizzaSizes() 
  (468 - 469)
- Save array length to local variable in changePizzaSizes() (472)
- Place variable pizzasDiv out of for loop (489)
- Replace querySelectorAll with getElementsByClassName and move items 
  variable out of updatePositions() (520)
- Move bodyScrollTop variable out of the updatePositions() for loop (528)
- Save array length to local variable in updatePositions() for loop (531)
- Move variable movingPizzas out of for loop and Replace querySelector with
  getElementById in updatePositions() (554)
- Reduce limit of for loop, define elem variable at start of loop in 
  in updatePositions() (557)

Before optimization: 

![Alt text](/img/FPSBefore.png?raw=true "Optional Title")

![Alt text](/img/resizeBefore.png?raw=true "Optional Title")

After optimization: 

![Alt text](/img/FPSAfter.png?raw=true "Optional Title")

![Alt text](/img/resizeAfter.png?raw=true "Optional Title")

## To view the optimized website
Open the optimized website [here](https://miguelamartinez.github.io/performance-optimization/). 
