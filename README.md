# Monte Carlo Method for Estimating Pi

## Project Overview

This project explores the use of the Monte Carlo simulation technique to approximate the value of π (pi).  
By generating a large number of random points and analyzing their distribution within a geometric space, we can derive a numerical estimate of pi.

## Method Description

The core idea is based on geometry and probability. We use a unit square and a quarter of a circle inscribed within it.

### Steps of the Algorithm:

1. **Random Point Sampling**  
   - Generate `N` random coordinate pairs (x, y) such that both x and y are in the interval [0, 1].

2. **Determining Valid Points**  
   - Check whether each point falls inside the quarter circle using the condition:  
     `x² + y² ≤ 1`

3. **Pi Calculation**  
   - The area of the square is 1 (1x1).  
   - The theoretical area of the quarter circle is `(π * r²) / 4` with r = 1.  
   - The proportion of points that fall inside the circle relative to the total number of points approximates this area ratio.  
   - Rearranging, we estimate π as:  
     `π ≈ 4 * (number of points inside the circle / total number of points)`

## Key Takeaways

- This method provides a stochastic approximation of π.
- The precision improves as the number of sampled points increases.
- Small sample sizes may lead to significant deviation from the actual value of π due to statistical variance.

## Notes

- Monte Carlo methods are useful when analytic solutions are complex or unavailable.
- While simple, this experiment illustrates the power of randomness in numerical estimation.
