---
layout: page
title:	Evaluating a polynomial
---

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async
      src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>

**Question.**    
Let $$p$$ be a polynomial with non-negative integer coefficients. You are given access to a machine that, given any $$n\in\mathbb N$$, returns $$p(n)$$. Give an algorithm to evaluate $$p$$.    
Assume that any other mathematical operations to be performed take no time and that the dominating factor is the number of calls you make to the machine.

<details>
	<summary> <b>Hint</b> </summary>

It is possible to evaluate it with just \(2\) calls to the machine.
</details>

<p></p>

<details>
	<summary> <b>Solution</b> </summary>

Use the machine to get \(p(1)\) and \(p(p(1)+1)\). Observe that when the latter is represented in base \(p(1)+1\), the digits correspond to coefficients of the polynomial (since any coefficient is at most \(p(1)\)). The required follows.

</details>