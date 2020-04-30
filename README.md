# ComputationalPhysics
Implementation and Analysis common Modelling and Simulations techniques used in physics

# Integrals

#### Trapezoidal Integrals
Notable Points:
- Each subdivision of the region of integration evaulated as the area of the trapezoid using the function evalutaion of the points at the ends of the interval (2 evaluations / subdivision)
- Error O(h^3)

#### Simpson's Rule Integrals
Notable Points:
- 3 evaluations / subdivision
- Error O(h^5)
- Exact for cubic polynomials or of lower degree

#### Gaussian Quadrature
Notable Points:
- N-point quadrature rule gives exact result for polynomials of degree upto 2n+1 where n = N - 1
- Very intricate proof using Legrande Polynomials, which are genrated recurcively and are orthogonal polynomials. They are the key since they form a basis for the polynomials

#### Monte Carlo Integration By Rejection (2D)
Notable Points:
- Main idea, random point (x, y) picked from an RNG within a certain square boundary for N times. If the point is below the function(naively), accept it otherwise reject
- Integral = (accepted) * (square_area) / (accepted + rejected)

#### Monte Carlo Integration By Mean (2D)
Notable Points:
- The main idea comes from the Mean Value theorem
- Find the mean value of a function by evaluationg N random points in the integral interval and finding the average
- I = (b - a) * (1 / N) * Sum_1_to_N(f(x_i)) for uniform probability density rng
- I = (1 / N) * Sum_1_to_N(f(x_i) / pdf(X)) for any pdf

#### Importance Sampling using Inverse Transform 

# Ising Model

