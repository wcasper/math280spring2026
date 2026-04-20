---
layout: page
title: Practice Exam 2 Solutions
permalink: /exams/practice-exam2-soln
---

Solve each of the following problems.
If the problem asks for a proof, be sure to carefully justify your work, including any theorems from class.

Note: you may NOT use a theorem or result from class to prove something when it makes the problem entirely trivial.  If you are unsure whether a particular theorem or result is allowed, just ask!

## Problem 1 (True or False)
For each of the following, write TRUE if the statement is true and FALSE if the statement is false.  NO explanation is needed.

* (a) A set $$A$$ is countable if there is a bijection from $$\mathbb N$$ to $$A$$.

FALSE! Could be finite.
* (b) The sets $$\mathbb Q$$ and $$\mathbb N$$ have the same cardinality.

TRUE!  We proved it in class.
* (c) If $$A$$ is any set, then $$\lvert A\rvert < \lvert \mathcal P(A)\rvert$$, where here $$P$$ Is the power set of $$A$$.

TRUE!  Cantor proved this.
* (d) The Cantor-Schroeder-Bernstein Theorem says that if $$\lvert A\rvert < \lvert B\rvert$$ and $$\lvert B\rvert < \lvert C\rvert$$, then $$\lvert A\rvert < \lvert C\rvert$$.

FALSE!  While the statement is true, it isn't the content of the CSB Theorem.
* (e) The Well-Ordering Principle says that any nonempty collection of positive numbers has a minimal element.

FALSE!  We need it to be positive integers.

## Problem 2

Consider the family of sets $$\mathcal F = \{U_k: k\in \mathbb N\}$$
where here

$$U_k = \left[\frac{1}{k},\frac{k+1}{k}\right)$$

Determine, with proof, intervals describing the following sets

* (a) $$\bigcup_{k=1}^\infty U_k$$

We claim that $$\bigcup_{k=1}^\infty U_k = (0,2)$$.

To see this, first suppose that $$x\in \bigcup_{k=1}^\infty U_k$$.  Then by definition, there exists an integer $$k$$ such that $$x\in U_k$$.  It follows that $$x\in [1/k,(k+1)/k)$$, so that $$1/k\leq x < (k+1)/k$$.  Since $$0 < 1/k$$, this says $$0 < x$$.  Also since $$1/k < 1$$, we get $$(k+1)/k = 1 + 1/k < 2$$, so that $$x < 2$$.  It follows that $$x\in (0,2)$$.  This proves $$\bigcup_{k=1}^\infty U_k \subseteq (0,2)$$.

Conversely, suppose $$x\in (0,2)$$.  We consider two cases:
**Case 1:** ($$x \geq 1$$).  If $$x \geq 1$$, then $$x\in U_1$$, so that $$x\in \bigcup_{k=1}^\infty U_k$$.
**Case 2:** ($$x < 1$$).  If $$x < 1$$, then since $$\mathbb N$$ is not bounded above, we can choose $$k\in \mathbb N$$ with $$k > 1/x$$.  It follows that $$\frac{1}{k} < x$$.  Moreover, $$x < 1 < 1 + 1/k = (k+1)/k$$.  Therefore $$x\in U_k$$, so that $$x\in\bigcup_{k=1}^\infty U_k$$.

Combining the two inclusions, this proves $$\bigcup_{k=1}^\infty U_k = (0,2)$$.

* (b) $$\bigcap_{k=1}^\infty U_k$$

We claim that $$\bigcap_{k=1}^\infty U_k = \{1\}.$$

Since $$1/k < 1$$ for all $$k\in\mathbb N$$ and $$1 < 1 + 1/k$$ for all $$k\in\mathbb N$$ we get $$1\in U_k$$ for all $$k\in \mathbb{N}$$.  Therefore $$1\in\bigcap_{k=1}^\infty U_k$$.  This proves $$\{1\}\subseteq \bigcap_{k=1}^\infty U_k$$.  Thus it suffices to prove the opposite inclusion.

To complete the proof it suffices to show that $$1$$ is the ONLY element in $$\bigcap_{k=1}^\infty U_k$$.  To see this, we will assume otherwise and arrive at a contradiction.  Assume $$x\in\bigcap_{k=1}^\infty U_k$$ with $$x\neq 1$$.
Then $$x\in U_k$$ for all $$k\in \mathbb N$$.  For $$k=1$$, this says $$x\in [1,2)$$, so $$1\leq x < 2$$.  In particular $$1\leq x$$. Since $$x\neq 1$$, we must have $$x > 1$$.  Then since $$\mathbb N$$ is not bounded above, we can choose $$j\in \mathbb N$$ with $$j > \frac{1}{x-1}$$.  It follows that $$\frac{1}{j} < x-1$$, so that $$1 + \frac{1}{j} < x$$.  This would mean $$(j+1)/j < x$$, so that $$x\notin U_j$$.  Since $$x\in U_k\forall k\in\mathbb N$$, this is a contradiciton.  Thus the only elementin $$\bigcap_{k=1}^\infty U_k$$ is $$1$$.  

This proves $$\bigcap_{k=1}^\infty U_k = \{1\}$$.

## Problem 3
* (a) Write down what it means for a relation $$R$$ on a set $$A$$ to be reflexive, symmetric, transitive, and an equivalence relation.

A relation $$R$$ on $$A$$ is:
 - reflexive if $$aRa$$ for all $$a\in A$$
 - symmetric if $$aRb\Rightarrow bRa$$ for all $$a,b\in A$$
 - transitive if $$aRb\ \text{and}\ bRc\Rightarrow aRc$$ for all $$a,b,c\in A$$
 - an equivalence relation if it is reflexive, symmetric, and transitive.
* (b) Let $$A$$ be the set of all positive integers, and define a relation $$R$$ on $$A$$ by $$mRn$$ if and only if $$\lvert m-n\rvert < 10$$.  Is $$R$$ an equivalence relation?

This is NOT an equivalence relation, since $$1R9$$ and $$9R13$$ but $$1R13$$ is FALSE.  Therefore we're not transitive.  We are reflexive and symmetric, though!
* (c) Let $$A$$ be the set of all positive integers, and define a relation $$R$$ on $$A$$ by $$mRn$$ if and only if $$3$$ divides $$m-n$$.  Is $$R$$ an equivalence relation?

YES!  To see, this we can check the properties.
  - Reflexive: $$3\vert 0$$ so $$3\vert a-a$$ for all $$a\in A$$.  Therefore $$aRa$$ for all $$a\in A$$.
  - Symmetric: If $$aRb$$, then $$3\vert a-b$$.  Therefore $$3\vert -(a-b)=b-a$$, so that $$bRa$$.
  - Transitive: If $$aRb$$ and $$bRc$$, then $$3\vert a-b$$ and $$3\vert b-c$$.  Therefore there exist integers $$m$$ and $$n$$ with $$a-b=3m$$ and $$b-c= 3n$$.  It follows that $$a-c = a-b + b-c = 3m + 3n = 3(m+n)$$.  This proves $$3\vert a-c$$ so $$aRc$$.

## Problem 4

* (a) Write down the definition of a partial ordering on a set $$A$$.

A partial ordering on a set $$A$$ is a relation that is reflexive, anti-symmetric, and transitive.  Here, anti-symmetric means that if $$aRb$$ and $$bRa$$ then $$a=b$$.
* (b) Let $$A$$ be the power set of $$\mathbb N$$.  Prove that the relation $$R$$ defined on $$A$$ by $$X R Y$$ if and only if $$X\subseteq Y$$ is a partial ordering.
  - Reflexive: If $$X\in A$$, then $$X\subseteq N$$.  Since any set is a subset of itself $$X\subseteq X$$.  Therefore $$XRX$$.
  - Anti-symmetric: Suppose $$X,Y\in A$$ with $$XRY$$ and $$YRX$$.  Then $$X$$ and $$Y$$ are subsets of $$\mathbb N$$ with $$X\subseteq Y$$ and $$Y\subseteq X$$.  It follows that $$X=Y$$.
  - Transitive: If $$X,Y,Z\in A$$ with $$XRY$$ and $$YRZ$$, then $$X,Y,Z$$ are subsets of $$\mathbb N$$ with $$X\subseteq Y$$ and $$Y\subseteq Z$$.  It follows that $$X\subseteq Z$$ so therefore $$XRZ$$.

This proves that $$R$$ is a partial ordering.

* (c) If $$X,Y\in A$$, prove $$X\cap Y$$ is a greatest lower bound of $$\{X,Y\}$$

Remember, the greatest lower bound $$B$$ of a subset $$S\subseteq A$$ satisfies
  - it is a lower bound, meaning $$BRX$$ for all $$X\in S$$
  - if $$C$$ is another lower bound, then $$CRB$$

Now take the specific case that $$S = \{X,Y\}\subseteq A$$.
Then $$X\cap Y\subseteq X$$ and $$X\cap Y\subseteq Y$$, so $$(X\cap Y)RX$$ and $$(X\cap Y)RY$$.
Therefore $$X\cap Y$$ Is a lower bound of $$\{X,Y\}$$.
Moreover, if $$C$$ is another lower bound of $$\{X,Y\}$$, then $$CRX$$ and $$CRY$$.
This means $$C\subseteq X$$ and $$C\subseteq Y$$, so that $$C\subseteq X\cap Y$$.
It follows that $$CR(X\cap Y)$$.  Thus $$X\cap Y$$ satisfies the definition of being a lower bound.

## Problem 5

* (a) Write down the definition of a relation from $$A$$ to $$B$$

It is a subset of the Cartesian product $$A\times B$$.
* (b) Write down the definition of a function $$f: A\rightarrow B$$

It is a relation $$R$$ from $$A$$ to $$B$$ satisfying two properties:

 - for all $$a\in A$$ there exists a $$b\in B$$ with $$aRb$$
 - if $$a,c\in A$$ and $$b\in B$$ satisfy $$aRb$$ and $$cRb$$, then $$a=c$$.
* (c) Write down the definition of $$f$$ being injective, surjective, and bijective.

A function $$f: A\rightarrow B$$ is called
 - injective if $$f(a) = f(c) \Rightarrow a=c$$ for all $$a,c\in A$$.
 - surjective if for all $$b\in B$$ there exists $$a\in A$$ with $$f(a) = b$$.
 - bijective if both injective and surjective
* (d) Prove that the function $$f: \mathbb N\rightarrow\mathbb Z$$ defined by

$$f(x) = \left\lbrace\begin{array}{cc}
n/2, & n\ \text{even}\\
(1-n)/2, & n\ \text{odd}\\
\end{array}\right.$$

is a bijection.

**Proof:**

To prove injectivity, suppose that $$a,c\in \mathbb N$$ with $$f(a) = f(c)$$.  We consider two cases.
  **Case 1:**  ($$f(a) > 0$$).  In this case, $$a$$ and $$c$$ must be even, since otherwise the output of $$f$$ would not be positive.  Therefore $$f(a) = a/2$$ and $$f(c) = c/2$$.  Since $$f(a) = f(c)$$, it follows that $$a/2=c/2$$ and therefore $$a=c$$.
  **Case 2:**  ($$f(a) \leq 0$$).  In this case, $$a$$ and $$c$$ must be odd, since otherwise the output of $$f$$ would be positive.  Therefore $$f(a) = (1-a)/2$$ and $$f(c) = (1-c)/2$$.  Since $$f(a) = f(c)$$, it follows that $$(1-a)/2=(1-c)/2$$.  Multiplying by $$2$$, we get $$1-a=1-c$$ and simplifying we find $$a=c$$.

In either case, we have $$a=c$$ and this proves injectivity.

To prove surjectivity, suppose instead that $$b\in \mathbb Z$$.  We consider two cases.
  **Case 1:**  $$b > 0$$.  In this case, take $$a = 2b\in\mathbb N$$.  Then $$a$$ is even, so $$f(a) = f(2b) = 2b/2 = b$$.
  **Case 1:**  $$b \leq 0$$.  In this case, take $$a = (1-2b)\in\mathbb N$$.  Then $$a$$ is odd so $$f(a) = f(1-2b) = (1-(1-2b))/2 = b$$.

In either case, there exists $$a\in \mathbb N$$ with $$f(a) = b$$.  This proves surjectivity.  Thus we have bijectivity.

## Problem 6

* (a) Write down the definition of a finite set.

A set is called finite if it is the empty set or congruent to $$\mathbb N_k$$ for some $$k\in\mathbb N$$.
* (b) Prove that any subset of $$\mathbb N_k$$ is finite.

**Proof:**
We proceed by induction on $$k$$.

The base case is $$k=1$$. In this case, $$\mathbb N_k = \{1\}$$, so the only subsets are $$\varnothing$$ and $$\mathbb N_k$$.  In either case, we are finite by definition.

As an inductive hypothesis, assume that there exists a positive integer $$m\geq 1$$ such that any subset of $$\mathbb N_m$$ is finite.
Then we claim that any subset of $$\mathbb N_{m+1}$$ is also finite.  To see this, suppose that $$A\subseteq \mathbb N_{m+1}$$.
We consider two cases.
  **Case 1:**  ($$m+1\notin A$$).  In this case $$A\subseteq \mathbb N_m$$, so $$A$$ is finite by our inductive hypothesis!
  **Case 1:**  ($$m+1\in A$$).  In this case $$A-\{m+1\}\subseteq \mathbb N_m$$, so $$A-\{m+1\}$$ is finite by our inductive hypothesis!  Therefore it is congruent to some $$\mathbb N_j$$ for some $$j\in\mathbb N$$.  That means that there exists a bijection $$f: A-\{m+1\}\rightarrow\mathbb N_j$$.  Define a function $$g: A\rightarrow\mathbb N_{j+1}$$ by

$$g(x) = \left\lbrace\begin{array}{cc}
f(x), & x\neq m+1\\
j+1, & x=m+1
\end{array}\right.$$

It is easy to see that $$g$$ is a bijection, and therefore $$A$$ and $$\mathbb N_{j+1}$$ are congruent.  Hence $$A$$ is finite.

In either case, $$A$$ is finite.  Since $$A$$ was an arbitrary subset of $$\mathbb N_{m+1}$$, this proves that every subset of $$\mathbb N_{m+1}$$ is finite.  Hence by the Principal of Mathematical Induction, we have that every subset of $$\mathbb N_k$$ is finite for all $$k\in\mathbb N$$.

* (c) Prove that any subset of  a finite set is finite.

Let $$A$$ be a finite set and $$S\subseteq A$$.  We wish to prove that $$S$$ is finite.  If $$S=\varnothing$$, then it's finite and we're done.  Assume otherwise.  Then $$S\neq\varnothing$$, so $$A\neq varnothing$$.  Since $$A$$ is finite, this means that there exists $$k$$ such that $$A$$ is congruent to $$\mathbb N_k$$.  That means that there exists a bijection $$f: A\rightarrow\mathbb N_k$$.

The image $$f(S)$$ of $$S$$ is a subset of $$\mathbb N_k$$, so it's a finite set by part (b).  Therefore there exists an integer $$j$$ with $$f(S)$$ congruent to $$\mathbb N_j$$ for some $$j\in\mathbb N$$.  In other words, there exists a bijection $$g: f(S)\rightarrow \mathbb N_j$$.  Define a function $$h: S\rightarrow \mathbb N_j$$ by

$$h(x) = g(f(x)).$$

Then $$h(x)$$ is a bijection and thus $$S$$ is congruent to $$\mathbb N_j$$.  Hence $$S$$ is finite.  Since $$S$$ was an arbitrary subset of $$A$$, this proves that all subsets of $$A$$ are finite.  Since $$A$$ was an arbitrary finite set, this proves that any subset of a finite set is finite.


## Problem 7

Use the axioms of the real numbers to prove

* (a) $$0\neq 2$$, where $$2=1+1$$.
* (b) Prove that if $$0 < x < y$$ then $$x^2 < y^2$$.

**Proof:**

* (a) We proved in class that $$0 < 1$$.  Therefore $$0+1< 1+1$$ by Axiom 7.  Therefore $$1 < 2$$ by Axiom 1b.  Since $$0 < 1$$ and $$1 < 2$$, transitivity tells us $$0 < 2$$.  Then the trichotomy says $$0\neq 2$$.

* (b) Since $$0 < x$$ and $$x < y$$, Axiom 8 says $$x^2 < xy$$.  Also since $$0 < y$$, Axiom 8 says $$xy < y^2$$.  Then by transitivity, we get $$x^2 < y^2$$.

## Problem 8

Let $$A\subseteq R$$ be nonempty sets of real numbers which is bounded below and set

$$C=\{-a: a\in A,\ b\in B\}$$

* (a) Write down the Completeness Axiom.

The Completeness Axiom says that any nonempty set of real numbers which is bounded above has a supremum.

* (b) Prove that $$m$$ is a lower bound for $$A$$ if and only if $$-m$$ is an upper bound of $$C$$.

$$\begin{align*}
m\ \text{is a lower bound of}\ A\\
\Leftrightarrow m \leq a\ \forall a\in A\\
\Leftrightarrow -a\leq -m\ \forall a\in A\\
\Leftrightarrow c\leq -m\ \forall c\in C\\
\Leftrightarrow -m\ \text{is an upper bound of}\ C
\end{align*}$$

* (c) Prove that $$m$$ is an infimum for $$A$$ if and only if $$-m$$ is a supremum of $$C$$.

Suppose that $$m$$ is an infimum of $$A$$.  Then $$m$$ is a lower bound for $$A$$.  Therefore $$-m$$ is an upper bound of $$C$$.
Moreover, if $$p$$ is another lower bound of $$A$$ then $$p\leq m$$.  If $$q$$ is an upper bound of $$C$$, then $$-q$$ is a lower bound of $$c$$ so -q\leq m$$.  Therefore $$-m \leq q$$.  It follows that $$-m$$ is a supremum of $$C$$.

Conversely, suppose that $$-m$$ is a supremum of $$C$$.  Then $$-m$$ is an upper bound of $$C$$, so $$m$$ is a lower bound of $$A$$.  Moreover, if $$q$$ is another upper bound of $$C$$, then $$-m \leq q$$.  Now suppose that $$p$$ is a lower bound of $$A$$.  Then $$-p$$ is an upper bound of $$C$$ and therefore $$-m\leq -p$$.  It follow sthat $$p\leq m$$.  Therefore $$m$$ is an infimum of $$A$$.

* (d) Prove that any nonempty set of real numbers which is bounded below has an infimum.

Suppose that $$A$$ is nonempty and bounded below.  Then $$C$$ (as defined in part (b)) is nonempty and bounded above.  By the Completeness Axiom, $$C$$ has a supremum.
Therefore $$A$$ has an infimum by part (c).

## Problem 9

Let $$A,B\subseteq R$$ be nonempty sets of positive real numbers which are bounded above and set

$$C=\{a\cdot b: a\in A,\ b\in B\}$$

* (a) Write down the definition of an upper bound of $$A$$

An upper bound of $$A$$ is a real number $$b$$ such that $$a\leq b$$ for all $$a\in A$$.

* (b) Write down the definition of a supremum of $$A$$

A supremum of $$A$$ is a real number $$s$$ such that
  - $$s$$ is an upper bound of $$A$$, and
  - if $$b$$ is another upper bound of $$A$$, then $$s\leq b$$

* (c) Prove that $$C$$ is bounded above and

$$\sup(C)\leq\sup(A)\sup(B)$$

Let $$s=\sup(A)$$ and $$t=\sup(B)$$ (which exist by the Completeness Axiom.  Then $$s$$ and $$t$$ are both upper bounds of $$A$$ and $$B$$, respectively.  If $$c\in C$$, then there exists $$a\in A$$ and $$b\in B$$ such that $$ab=c$$.  It follows that

$$c = ab\leq at\leq st.$$

Thus $$st$$ is an upper bound of $$C$$.
In particular, $$C$$ is bounded above and has a supremum $$r=\sup(C)$$.  Since $$st$$ is an upper bound of $$C$$, the definition of a supremum implies that 

$$r \leq st.$$

Therefore 

$$\sup(C)\leq\sup(A)\sup(B).$$


