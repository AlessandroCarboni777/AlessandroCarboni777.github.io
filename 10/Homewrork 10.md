___

## Riemann Integration
Riemann integration begins by partitioning the *domain* (the $x$-axis) into subintervals. Within each subinterval, one evaluates the function at a chosen point (often a midpoint or endpoint). Summing these values, each multiplied by the subinterval width, approximates the total area. In the limit as the partition gets finer (i.e., the width of the intervals $\to 0$), the Riemann sums converge if the function has certain regularity properties—chiefly, it must not be *too* discontinuous. Conceptually, one can picture adding up infinitely many vertical “strips.” 

## Lebesgue Integration
Lebesgue integration adopts a different lens by focusing on the *range* of the function, partitioning the *values* of $f(x)$ instead of partitioning the $x$-axis. Then it measures the set of $x$-values mapping into each slice of the range. This method follows from measure theory and is more powerful than Riemann’s approach because it can handle complicated discontinuities. One can define a Lebesgue integral even when a function fails to be Riemann-integrable.

## Continuous vs. Discontinuous Functions
When $f(x)$ is continuous on a given interval, both Riemann and Lebesgue integration typically yield the same result. However, a function with too many discontinuities (or certain kinds of “wild” behavior) may lack a Riemann integral but still have a Lebesgue integral. 

## Features
Comparing Riemann and Lebesgue frameworks showcases key developments in modern analysis. Riemann’s sums are intuitive and suffice for most elementary calculus, while Lebesgue integration extends integrability to a broader class of functions. Crucially, Lebesgue’s construction unifies integration with measure theory, offering profound insights into convergence, the definition of measurable sets, and the generalization of “area under the curve.”
