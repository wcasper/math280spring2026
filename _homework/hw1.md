---
layout: page
title: Homework 1
permalink: /homework/hw1
---

### Directions
Solve the following problems and type up your solutions.  Your solutions should be provided in one of the following formats (in order of preference)
* typed up in $$\LaTeX$$ and submitted as a PDF on Canvas
* written legibly on blank paper, scanned into a PDF and then uploaded on Canvas
* written on ancient parchement with a quill and then flown to the instructor via owl post like in Harry Potter

If you go with the first strategy, you may wish to check out Overleaf which is a free and intuitive website for generating $$\LaTeX$$ documents online.
If you wish to use the second method and don't own a scanner at home, you can check out the numerous scanning apps available for smartphones.

**Problem 1:**

One of the most frequently used identities in undergraduate mathematics is the **geometric sum:**

For all real numbers $$r\neq 1$$ and all integers $$n\geq 0$$,

$$1 + r + r^2 + r^3 + \dots + r^n = \frac{r^{n+1}-1}{r-1}.$$

* (a) Prove this identity using mathematical induction
* (b) Find another proof which doesn't rely on induction

<details>
  <summary>Reveal hint</summary>

  Let $$s = 1 + r + r^2 + r^3 + \dots + r^n.$$

  Try to find s hidden inside the larger sum

  $$1 + r + r^2 + r^3 + \dots + r^n + r^{n+1}$$

  in two different ways.  Then use the two different expressions to solve for s.

</details>

**Problem 2:**

Consider the product

$$p_n = \left(1+\frac{1}{2}\right)\left(1+\frac{1}{4}\right)\left(1+\frac{1}{8}\right)\dots\left(1+\frac{1}{2^n}\right).$$

* (a) Work out the values of $$p_1,p_2,p_3,$$ and $$p_4$$
* (b) Use (a) to work out a pattern and conjecture for the value of $$p_n$$ for all $$n\geq 1$$
* (c) Use induction to prove your guess in part (b) is correct
* (d) Find another proof which doesn't rely on induction

<details>
  <summary>Reveal hint</summary>

  Try simplifying the value of 

  $$\left(1-\frac{1}{2}\right)p_n.$$

</details>

**Problem 3:**

* (a) Use Pascal's triangle to figure out the value of $$\binom{8}{4}$$ fast by hand
* (b) What is the coefficient of $$x^3$$ in $$(1+2x)^5$$
* (c) How many subsets are there of the set $$\{1,2,3,4,5,6,7\}$$ with $$3$$ elements?

**Problem 4:**

For this problem, assume that $$p$$ is a prime number.
We say that $$m$$ **is equivalent to** $$n$$ **modulo** $$p$$ and write

$$m\equiv n\mod p$$

if the difference $$m-n$$ is divisible by $$p$$.

* (a) Prove that for any integer $$0 < k < p$$, the binomial coefficient $$\binom{p}{k}$$ is divisible by $$p$$.
* (b) Use the binomial theorem to prove the **Freshman's Dream:** for any integers $$x$$ and $$y$$ 

$$(x + y)^p\equiv x^p + y^p\mod p.$$


**Problem 5:**

Prove that for any integers $$0\leq m \leq n$$

$$\binom{m}{0}\binom{n}{0} + \binom{m}{1}\binom{n}{1} + \binom{m}{2}\binom{n}{2} + \dots + \binom{m}{m}\binom{n}{m} = \binom{m+n}{m}.$$

<details>
  <summary>Reveal hint</summary>

  Consider the factorization

  $$(1+x)^{m+n} = (1+x)^m(1+x)^n$$

  and compare the coefficients of the m'th power of x on both sides.

</details>






