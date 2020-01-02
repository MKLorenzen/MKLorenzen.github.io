---
title: The bounded degree vertex cover problem
---

The bounded degree vertex cover problem is a variation of the vertex cover problem, which is a well studied problem in the field of parametrized complexity. Some applications include use cases in cyber security and in efficient dynamic detection of race conditions.

## What is the vertex cover problem?

This problem comes from graph theory, where in a graph G = (V,E), where V is a set of vertices and E is a set of edges, we want a subset of the V such that all edges in E is connected to a vertex from the subset. This subset is called a vertex cover. 

Now everyone can construct a random subset of an arbitrary size, but we want the smallest possible subset that is still a vertex cover. To be more precise this is the minimum vertex problem.

## The bounded degree version

This is a variation of the original problem where the degree of vertex is bounded by a fixed constant. The degree of a vertex means the number of edges that are connected to a vertex (in a undirected graph). 

math test:

$$
\begin{align*}
  & \phi(x,y) = \phi \left(\sum_{i=1}^n x_ie_i, \sum_{j=1}^n y_je_j \right)
  = \sum_{i=1}^n \sum_{j=1}^n x_i y_j \phi(e_i, e_j) = \\
  & (x_1, \ldots, x_n) \left( \begin{array}{ccc}
      \phi(e_1, e_1) & \cdots & \phi(e_1, e_n) \\
      \vdots & \ddots & \vdots \\
      \phi(e_n, e_1) & \cdots & \phi(e_n, e_n)
    \end{array} \right)
  \left( \begin{array}{c}
      y_1 \\
      \vdots \\
      y_n
    \end{array} \right)
\end{align*}
$$

## Applications

**_This section is under construction_**
