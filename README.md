# What is Quasi-Newton method ?
Quasi-Newton methods are optimization algorithms used to find the minimum (or maximum) of a function. These methods belong to the broader class of quasi-Newton optimization algorithms, which are designed for unconstrained optimization problems. The primary goal is to iteratively find the minimum of a scalar function without requiring the calculation of derivatives at each step.

Quasi-Newton methods are iterative and build an approximation to the inverse Hessian matrix of the objective function. The Hessian matrix represents the second-order partial derivatives of the objective function with respect to its variables and plays a crucial role in determining the curvature of the function.

The Newton-Raphson method is a classical optimization algorithm that uses the exact Hessian matrix at each iteration. However, computing the exact Hessian can be computationally expensive and, in some cases, impractical. Quasi-Newton methods offer a more computationally efficient alternative by approximating the Hessian matrix.

The Broyden–Fletcher–Goldfarb–Shanno (BFGS) algorithm and the Davidon–Fletcher–Powell (DFP) algorithm are two well-known examples of quasi-Newton methods. These methods iteratively update their estimates of the inverse Hessian based on the changes in the gradient of the objective function.

Here's a brief overview of the BFGS algorithm, one of the most widely used quasi-Newton methods:

Initialization:

Start with an initial guess for the minimizer and an initial approximation to the inverse Hessian matrix.
Iteration:

At each iteration, compute the gradient of the objective function and update the approximation to the inverse Hessian.
Search Direction:

Determine the search direction by multiplying the negative inverse Hessian approximation by the gradient.
Line Search:

Perform a line search along the search direction to find an optimal step size.
Update:

Update the current estimate of the minimizer using the step size.
Convergence:

Check for convergence criteria, such as a small change in the objective function or gradient.
Repeat:

If convergence criteria are not met, repeat the process.
Quasi-Newton methods are particularly useful when the exact Hessian is challenging to compute, and they have been successfully applied to various optimization problems in fields such as machine learning, numerical optimization, and mathematical modeling. The efficiency of quasi-Newton methods lies in their ability to provide a good approximation of the Hessian without the computational cost of its exact calculation.







https://www.youtube.com/watch?v=UvGQRAA8Yms
