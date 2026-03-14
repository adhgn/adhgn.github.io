---
layout: default
title: Numerical Analysis - Polynomial Interpolation
---

# Polynomial Interpolation Project

In this project, I explored how to approximate functions using **Lagrange** and **Newton** basis functions. 

### The Problem
We want to interpolate $f(x) = \sin(2x)$ on the interval $[-\pi, \pi]$. Using a set of nodes, we can construct a polynomial that passes through all points.

### The Math
The Lagrange form of the interpolating polynomial is:
$$P_n(x) = \sum_{i=0}^{n} y_i L_i(x)$$

### MATLAB Implementation
```matlab
% Example of calculating Lagrange basis
for i = 1:n
    L = 1;
    for j = [1:i-1, i+1:n]
        L = conv(L, [1, -x(j)]) / (x(i) - x(j));
    end
end
