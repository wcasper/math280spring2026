---
layout: page
title: Homework 5
permalink: /homework/hw5
---

### Directions
Solve the following problems and type up your solutions.  Your solutions should be provided in one of the following formats (in order of preference)
* typed up in $$\LaTeX$$ and submitted as a PDF on Canvas
* written legibly on blank paper, scanned into a PDF and then uploaded on Canvas
* written on ancient parchement with a quill and then flown to the instructor via owl post like in Harry Potter

If you go with the first strategy, you may wish to check out Overleaf which is a free and intuitive website for generating $$\LaTeX$$ documents online.
If you wish to use the second method and don't own a scanner at home, you can check out the numerous scanning apps available for smartphones.

**Problem 1:**

Let $$f: \mathbb{N}_m\rightarrow\mathbb{N}_n$$ be a function.
Without using any theorems from class, prove that if $$m < n$$ then $$f$$ cannot be surjective.


<details>
  <summary>Reveal hint</summary>

  Proceed by induction on n.
</details>

**Problem 2:**

Prove that if $$A$$ and $$B$$ are finite *disjoint* sets, then

$$\lvert A\times B\rvert = \lvert A\rvert \cdot \lvert B\rvert.$$

<details>
  <summary>Reveal hint</summary>

  Assume that $$A\approx\mathbb N_m\quad\text{and}\quad B\approx\mathbb N_n$$.  Then build a bijection from $$N_m\times N_n$$ to $$N_{nm}$$.
</details>

**Problem 3:**

Prove that if $$A$$ and $$B$$ are finite *disjoint* sets, then

$$\lvert A\cup B\rvert = \lvert A\rvert + \lvert B\rvert.$$

<details>
  <summary>Reveal hint</summary>

  Assume that $$A\approx\mathbb N_m\quad\text{and}\quad B\approx\mathbb N_n$$.  Then build a bijection from $$A\cup B$$ to $$N_{n+m}$$.
</details>

**Problem 4:**

Prove the **inclusion-exclusion principle** states that if $$A$$ and $$B$$ are finite sets then

$$\lvert A\cup B\rvert = \lvert A\rvert + \lvert B\rvert - \lvert A\cap B\rvert.$$


<details>
  <summary>Reveal hint</summary>

  Use the previous problem to write

  $$\lvert A\cup B\rvert = \lvert A\rvert + \lvert B-A\rvert$$

  Then add and subtract $$\lvert A\cap B\rvert$$

</details>


**Problem 5:**

Let $$A$$ be an infinite set.

* (a) Prove that there is an injective function $$\mathbb N\rightarrow A$$
* (b) Prove that

$$A\approx A\cup \{x\}.$$












