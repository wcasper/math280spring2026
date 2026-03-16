---
layout: page
title: Homework 4
permalink: /homework/hw4
---

### Directions
Solve the following problems and type up your solutions.  Your solutions should be provided in one of the following formats (in order of preference)
* typed up in $$\LaTeX$$ and submitted as a PDF on Canvas
* written legibly on blank paper, scanned into a PDF and then uploaded on Canvas
* written on ancient parchement with a quill and then flown to the instructor via owl post like in Harry Potter

If you go with the first strategy, you may wish to check out Overleaf which is a free and intuitive website for generating $$\LaTeX$$ documents online.
If you wish to use the second method and don't own a scanner at home, you can check out the numerous scanning apps available for smartphones.

**Problem 1:**

Consider the partial ordering $$\vert$$ on the set $$A = \{k\in\mathbb{Z}: k\geq 0\}$$ of positive integers.  Remember $$a\vert b$$ means $$a$$ divides $$b$$, ie. that there exists an integer $$k$$ with $$b=ka$$.

* (a) Let $$x$$ and $$y$$ be integers.  Prove that the supremum of $$\{x,y\}$$ exists and is equal to the least common multiple of $$x$$ and $$y$$.
* (b) Let $$x$$ and $$y$$ be integers.  Prove that the infimum of $$\{x,y\}$$ exists and is equal to the greatest common divisor of $$x$$ and $$y$$.

**Problem 2:**

For each of the following relations, determine the domain, codomain, and range.  Also explain whether the relation is or is not a function.

* (a) $$f\subseteq \mathbb Z\times\mathbb Z$$, $$f = \{(x,y): 2x=3y\}$$
* (b) $$g\subseteq \mathbb Z\times\mathbb Z$$, $$f = \{(x,y): x<=y\}$$
* (c) $$g\subseteq \mathbb Z\times\mathbb Z$$, $$f = \{(x,y): 0 \leq y-x/2 < 1 \}$$

**Problem 3:**

Let $$k$$ and $$n$$ be integers with $$n>0$$.
The **equivalence class** of $$k$$ modulo $$n$$ is the set

$$[k]_n = \{j: j\in\mathbb{Z},\ \text{and $n$ divides $j-k$}\}.$$

We write $$\mathbb Z_n$$ to mean the set of all equivalence classes of integers modulo $$n$$, ie.

$$\mathbb Z_n = \{[k]_n: k\in\mathbb{Z}\}.$$

Prove the following

* (a) For any integers $$x$$ and $$y$$, $$[x]_n=[y]_n$$ if and only if $$n$$ divides $$(x-y)$$.
* (b) For any integer $$k$$, there exists a unique integer $$0\leq r < n$$ with $$[k]_n = [r]_n$$.  Hint: use the division algorithm.
* (c) Prove that $$\mathbb Z_n$$ has exactly $$n$$ elements and in fact

$$\mathbb Z_n = \{[0]_n, [1]_n, [2]_n,\dots, [n-1]_n\}.$$

**Problem 4:**

For each of the following functions, determine whether the function is well-defined.  Carefully explain.

* (a) $$f: \mathbb Z_{6}\rightarrow\mathbb Z_{12}$$ defined by the rule $$f([k]_6) = [k]_{12}$$
* (b) $$f: \mathbb Z_{6}\rightarrow\mathbb Z_{3}$$ defined by the rule $$f([k]_6) = [k]_{3}$$
* (c) $$f: \mathbb Z_{6}\rightarrow\mathbb Z_{12}$$ defined by the rule $$f([k]_6) = [2k]_{12}$$

**Problem 5:**

Let $$f: A\rightarrow B$$ be a function and suppose that $$\mathcal F = \{X_i: i\in I\}$$ and $$\mathcal G = \{Y_j: j\in J\}$$ are indexed families of subsets of $$A$$ and $$B$$, respectively.
Prove that
* (a)

$$f\left(\bigcup_{i\in I}X_i\right) = \bigcup_{i\in I}f(X_i).$$

* (b) 

$$f\left(\bigcap_{i\in I}X_i\right) \subseteq \bigcap_{i\in I}f(X_i).$$

* (c)

$$f^{-1}\left(\bigcup_{j\in J}Y_j\right) = \bigcup_{j\in J}f^{-1}(Y_j).$$

* (d) 

$$f^{-1}\left(\bigcap_{j\in J}Y_j\right) = \bigcap_{j\in J}f^{-1}(Y_j).$$













