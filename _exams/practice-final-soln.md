---
layout: page
title: Practice Final Solution
permalink: /exams/practice-final-soln
---

Solve each of the following problems.
If the problem asks for a proof, be sure to carefully justify your work, including any theorems from class.

Note: you may NOT use a theorem or result from class to prove something when it makes the problem entirely trivial.  If you are unsure whether a particular theorem or result is allowed, just ask!

## Problem 1 (True or False)
For each of the following, write TRUE if the statement is true and FALSE if the statement is false.  NO explanation is needed.

* (a) If $$A\subseteq B$$ and $$A\neq B$$ then $$\lvert A\rvert < \lvert B\rvert$$
* (b) $$\varnothing =  \{\varnothing\}$$
* (c) $$\{\mathbb R\}$$ is an open cover of $$(-1,1)$$
* (d) If $$A\subseteq \mathbb R$$, then $$A$$ is either open or closed
* (e) The Well-Ordering Principle says that any nonempty collection of positive numbers has a minimal element.


**Solution:**

F,F,T,F,F

## Problem 2

Use a **truth table** to decide whether or not $$\sim(A\Rightarrow B)$$ is equivalent to $$A\wedge (\sim B)$$.

**Solution:**

$$\begin{tabular}{|c|c|c|c|c|c|}
A & B & \sim B & A\wedge (\sim B) & A\Rightarrow B & \sim(A\Rightarrow B)\\\hline
T & T & F      & F                & T              & F\\
T & F & T      & T                & F              & T\\
F & T & F      & F                & T              & F\\
F & F & T      & F                & T              & F\\
\end{tabular}$$

Therefore they are equivalent.
## Problem 3

Let $$A$$ be a set and $$R$$ be a relation on $$A$$.

* (a) What does it mean for $$R$$ to be an equivalence relation on $$A$$?
* (b) Prove that if $$R$$ and $$S$$ are equivalence relations on $$A$$, then $$R\cap S$$ is also an equivalence relation on $$A$$.

**Solution:**

* (a) It's a relation that is reflexive, symmetric, and transitive.
* (b) We must show all three properties.
 - reflexive: since $$R$$ and $$S$$ are reflexive, we know that $$aRa$$ and $$aSa$$ for all $$a\in A$$.  Therefore $$(a,a)\in R$$ and $$(a,a)\in S$$ for all $$a\in A$$.  It follows that $$(a,a)\in R\cap S$$ for all a\in A$$.  Thus $$a(R\cap S)a$$ for all $$a\in A$$.
 - symmetric: since $$R$$ and $$S$$ are symmetric, we know that $$aRb\Rightarrow bRa$$ and $$aSb\Rightarrow bSa$$ for all $$a,b\in A$$.  Now suppose that $$a(R\cap S)b$$ for some $$a,b\in A$$.  Then $$(a,b)\in R\cap S$$.  Therefore $$(a,b)\in R$$ and $$(a,b)\in S$$.  It follows that $$aRb$$ and $$aSb$$.  Therefore $$bRa$$ and $$bSa$$.  This means $$(b,a)\in R$$ and $$(b,a)\in S$$.  Therefore $$(b,a)\in R\cap S$$.  Hence $$b(R\cap S)a$$.  Thus $$a(R\cap S)b\Rightarrow b(R\cap S)a$$ for all $$a,b\in A$$.
 - transitive: Suppose that $$a(R\cap S)b$$ and $$b(R\cap S)c$$ for some $$a,b,c\in A$$.  Then $$(a,b)\in R\cap S$$ and $$(b,c)\in R\cap S$$.  This means that $$(a,b),(b,c)\in R$$ and $$(a,b),(b,c)\in S$$.  Hence $$aRb$$ and $$bRc$$ and $$aSb$$ and $$bSc$$.  Since $$R$$ and $$S$$ are transitive, we know that $$aRc$$ and $$aSc$$.  Therefore $$(a,c)\in R$$ and $$(a,c)\in S$$.  It follows that $$(a,c)\in R\cap S$$, so that $$a(R\cap S)c$$.  Thus $$a(R\cap S)b$$ and $$b(R\cap S)c$$ implies $$a(R\cap S)c$$ for all $$a,b,c\in A$$.

## Problem 4

* (a) Write down the definition of a finite set and of an infinite set.
* (b) Write down the Pidgeonhole Principle.
* (c) Prove that if $$j,k\in\mathbb N$$ with $$j\neq k$$ then $$\mathbb N_j$$ and $$\mathbb N_k$$ have different cardinality.
* (d) Prove that $$\mathbb N$$ is an infinite set.

**Solution:**

* (a) A set is finite if it is empty or equivalent to $$\mathbb N_k$$ for some $$k\in\mathbb N$$.  A set is infinite if it is not finite.
* (b) The Pidgeonhole Principle says that if $$f: \mathbb R_m\rightarrow\mathbb R_n$$ with $$m>n$$ then $$f$$ cannot be injective.
* (c) Without loss of generality, we may assume $$j > k$$.  Then by the Pidgeonhole Principle, no function $$f: \mathbb N_j\rightarrow\mathbb N_j$$ can be injective, so no bijection exists.  Therefore they have different cardinalities.
* (d) We will do a proof by contradiction.  Suppose that $$\mathbb N$$ is finite.  Since $$1\in \mathbb N$$, we know it is non-empty.  Therefore there must exist an integer $$n$$ and a bijection $$f: \mathbb N\rightarrow\mathbb N_n$$.  However, $$\mathbb N_{n+1}$$ is a subset of $$\mathbb N$$.  The restriction of $$f$$ to this subset defines an injection from $$\mathbb N_{n+1}$$ to $$\mathbb N_n$$.  This contradicts the Pidgeonhole Principle.


## Problem 5

* (a) Write down the definition of a relation from $$A$$ to $$B$$
* (b) Write down the definition of a function $$f: A\rightarrow B$$
* (c) Write down the definition of $$f$$ being injective, surjective, and bijective.
* (d) Consider the relation $$f$$ from $$(0,1)$$ to $$(1,\infty)$$ defined by $$afb\Leftrightarrow ab=1$$.  Prove that $$f$$ is a function from $$(0,1)$$ to $$(1,\infty)$$.
* (e) Prove that the function $$f$$ from part (d) is a bijection.


**Solution:**

* (a) A subset of $$A\times B$$
* (b) A relation $$f$$ from $$A$$ to $$B$$ with two properties: $$\forall a\in A\exists b\in B$$ such that $$afb$$ and $$\forall a\in A\forall b,c\in B$$ if $$afb$$ and $$afc$$ then $$b=c$$.  Notice we don't adopt function notation UNTIL we know it's a function.  So we write $$afb$$ instead of $$f(a) =b$$ for this proof.
* (c)
  - injective: for all $$a_1,a_2\in A$$ if $$f(a_1)=f(a_2)$$ then $$a_1=a_2$$.
  - surjective: for all $$b\in B$$ there exists $$a\in A$$ such that $$f(a) =b$$.
  - bijective: both injective and surjective
* (d) In this case $$A=(0,1)$$ and $$B = (1,\infty)$$.  If $$a\in (0,1)$$ then $$1/a\in (1,\infty)$$ and $$af(1/a)$$.  Thus for all $$a\in (0,1)$$, there exists $$b\in (1,\infty)$$ (namely $$b=1/a$$) satisfying $$afb$$.  Lastly if $$afb$$ and $$afc$$, then $$ab=1$$ and $$ac=1$$.  This implies $$ab=ac$$, so that $$b=c$$.  This proves $$f$$ is a function.  Specifically the one given by the formula $$f(x) = 1/x$$.
* (e) If $$f(a_1) = f(a_2)$$ then $$1/a_1=1/a_2$$, so $$a_1=a_2$$.  This proves injectivity.  Moreover, if $$b\in (1,\infty)$$ then $$1/b\in (0,1)$$ and $$f(1/b) = b$$.  This proves surjectivity.  Hence it is bijective.

## Problem 6

* (a) Write down the definition of $$\binom{n}{k}$$ from class.

* (b) Determine the value of $$\binom{7}{3}$$.  Show your work.

* (c) Prove that $$\binom{n}{k} = \binom{n}{n-k}$$ for all integers $$0\leq k\leq n$$


**Solution:**

* (a) It's the coefficient of $$x^k$$ in the expansion of $$(1+x)^n$$.
* (b) Do the Pascal triangle thing.
* (c) Use Pascal's Identity.

## Problem 7

Use induction to prove that for any integer $$n\geq 0$$

$$1^3 + 2^3 + \dots + n^3 = \left(\frac{n(n+1)}{2}\right)^2.$$

**Solution:**

 - Base case: $$n=1$$

$$1^3=\left(\frac{1(1+1)}{2}\right)^2$$.

 - Inductive assumption: We will assume that for some integer $$k\geq 1$$ 

$$1^3 + 2^3 + \dots + k^3 = \left(\frac{k(k+1)}{2}\right)^2.$$

 - Inductive step: Now consider the case when $$n=k+1$$.  Then 

$$\begin{align*}
1^3 + 2^3 + \dots + k^3 + (k+1)^3
  & = \left(\frac{k(k+1)}{2}\right)^2 + (k+1)^3\\
  & = \frac{k^2(k+1)^2 + 4(k+1)^3}{4}\\
  & = \frac{(k+1)^2(k^2 + 4(k+1))}{4}\\
  & = \frac{(k+1)^2(k+2)^2}{4}\\
  & = \left(\frac{(k+1)(k+2)}{2}\right)^2
\end{align*}$$

Thus by the Principle of Induction, the statement is true for all integers $$n\geq 1$$.

## Problem 8

* (a) State the definition of a supremum of an open set $$A$$

* (b) State the completeness axiom of $$\mathbb R$$

* (c) Give an example of a subset of $$\mathbb R$$ with no supremum.  Explain why.

* (d) Let $$A\subseteq \mathbb R$$ and suppose that $$A$$ has supremum $$s$$.
  Prove that for all $$\epsilon > 0$$ there exist $$a\in A$$ such that $$\lvert s-a\rvert < \epsilon$$.

**Solution:**

* (a) A supremum of $$A$$ is a real number $$s$$ with two properties:
  - it is an upper bound for $$A$$, meaning $$a\leq s$$ for all $$a\in A$$
  - if $$b$$ is any upper bound for $$A$$, then $$s\leq b$$

* (b) Every nonempty set of real numbers which is bounded above has a supremum

* (c) The set $$\mathbb N$$ is not bounded above and therefore has no supremum.

* (d) Let $$s$$ be a supremum for $$A$$.  Then for all $$\epsilon > 0$$, we know $$s-\epsilon < s$$ and therefore it cannot be an upper bound of $$A$$.  Hence there exists $$a\in A$$ such that $$s-\epsilon < a$$.  This means $$s-a < \epsilon$$.  Moreover $$a < s$$.  Therefore 

$$\lvert s-a\rvert = s-a < \epsilon.$$

## Problem 9

* (a) State the Heine-Borel Theorem

* (b) State the Bolzano-Weierstrass Theorem

* (c) Give an example of an open cover of $$\mathbb Z$$ with no finite subcover

* (d) Give an example of an open cover of $$(3,5)$$ with no finite subcover

**Solution:**

* (a) A subset of the real numbers is compact if and only if it is closed and bounded.
* (b) Any infinite bounded set of real numbers has an accumulation point.
* (c) Take the open cover $$\{U_i: i\in\mathbb Z\}$$ where here $$U_i = (i-1/2,i+1/2)$$.  If we throw out any $$U_j$$, then we no longer cover the integer $$j$$.  Therefore this has no finite subcovers.
* (d) We can take the open cover $$\{U_i: i\in\mathbb N\}$$ where here $$U_i = (3+1/i,5)$$.  This is the usual nested cover argument like we did in class.

