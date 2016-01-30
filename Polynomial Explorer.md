<style>
.section .reveal .state-background {
    background: LightSlateGrey;}
.section .reveal h1,
.section .reveal p {
    color: white;
    position: relative;
    top: 4%;}
    
.exclaim .reveal ul {
    list-style: none;
    padding:0;
    margin:0;
}

.exclaim .reveal li { 
    padding-left: 1em; 
    text-indent: -.7em;}
    
.exclaim .reveal .state-background {
  background: darkgrey;
} 
.exclaim .reveal h3{color: DarkSlateGrey;}
.exclaim .reveal h1,
.exclaim .reveal h2,
.exclaim .reveal p, 
.exclaim .reveal li{
  color: white;
}
.exclaim .reveal li:before {
    content: "• ";
    color: LightSlateGrey; 
}
.exclaim .reveal .footer{
    position: fixed; top: 85%;
    text-align:center; width:100%;
    margin-left: auto;
    margin-right: auto;
}
.exclaim .reveal .header{
    position: fixed; top: 15%;
    text-align:center; width:100%;
}
.exclaim .reveal .explorer ul{
     margin-top: 35%;
}
.exclaim .reveal .explorer li{
     font-size: 24pt;
}

.reveal .explorer img{
    margin-top: 25%;
    width: 700px;
    height: auto;
}
</style>
Polynomial Explorer
========================================================
author: A Tool for Learning Polynomial Properties 
date: Clyde Tressler

Why Explore Polynomials?
========================================================
type: exclaim

Polynomials are useful functions for linear modeling and
- are suitable for real number valued outcomes with numerical predictors
- arise naturally in many physical systems
<div class="footer"><h2>However: high degree polynomials can **[overfit](https://en.wikipedia.org/wiki/Overfitting)** noisy data.</h2></div>

******

![plot of chunk unnamed-chunk-1](Polynomial Explorer-figure/unnamed-chunk-1-1.png) 

Spotting Trends
========================================================
type: exclaim

- It's easy to distinguish odd degree functions from even degree functions with no noise present
- <b>But</b> noise can quickly overwhelm even simple linear and quadratic relationships

***

![plot of chunk unnamed-chunk-2](Polynomial Explorer-figure/unnamed-chunk-2-1.png) 

Polynomial Explorer
========================================================
type: exclaim
class: explorer
left: 40%
<div class="header">Randomly generates polynomials of the form:<br/>
$$y = ax^5 + bx^4 + cx^3 + dx^2 + x + constant +\epsilon$$</div>

- visualizes polynomials with normally-distributed noise
- familiarizes the user with fitting polynomial curves using R's lm() function.
- shows a key measure of fit: [Residual Sum of Squares](https://en.wikipedia.org/wiki/Residual_sum_of_squares)

***
<img class="explorer" src="poly_exp.png" style="max-width: 300%; max-height: 300%;">


Future Development
========================================================
type: exclaim
class: future
- inclusion of log and trigonometric functions
- 'user-built' polynomials add control to visualization
- transtioning to **Linear Model Explorer**

***

![plot of chunk unnamed-chunk-3](Polynomial Explorer-figure/unnamed-chunk-3-1.png) 

<div class= "footer", style="margin-left: -50%; font-size: 22pt">Visit soon at <a href = "https://amalgamatedclyde.shinyapps.io/polynomial_explorer", target="_blank">Polynomial Trend Spotter</a></br><span>Source code at:<a href="https://github.com/amalgamatedclyde/ddp_shiny"> https://github.com/amalgamatedclyde/ddp_shiny</a>
</div>
