---
layout: page
title: Satisfying Assignment of 3-SAT
---

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async
      src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>

**Question.**    
Given any $$3$$-SAT instance with $$m$$ clauses, show that there is an assignment that satisfies (at least) $$7m/8$$ of the clauses.


<details>
	<summary> <b>Solution</b> </summary>

Let $$X$$ be a uniform random variable on the set of possible assignments. Consider the random variable $$f(X)$$, where for any model $$m$$, $$f(m)$$ represents the number of true clauses under it.    
The probability of a particular clause being true under an assignment chosen from $$X$$ is $$7/8$$. The linearity of expectation implies that the expectation of $$f(X)$$ is $$7m/8$$. The required follows.

</details>

<p></p>
<p></p>

**Question.**    
Given any $$3$$-SAT instance with $$m$$ clauses, give a quadratic time algorithm to find an assignment that satisfies (at least) $$7m/8$$ of the clauses.

<details>
	<summary> <b>Hint</b> </summary>

Try splitting into cases and using the above result.
</details>

<p></p>


<details>
	<summary> <b>Solution</b> </summary>

Let $$x_1$$ be a variable in the formula. Consider $$\mathbb{E}[f(X)\mid x_1 = 0]$$ and $$\mathbb{E}[f(X)\mid x_2 = 0]$$. Since the arithmetic mean of the two is at least $$7m/8$$, one of the two must be at least $$7m/8$$. Further, both of them can be computed quite easily. We then recurse on the corresponding smaller subproblem. The required follows.
</details>

<p></p>

**An Interesting Follow-up.**    
Assuming $$\mathsf{P}\neq\mathsf{NP}$$, for any $$\varepsilon>0$$, there is no polynomial time algorithm that, for any $$3$$-SAT instance, finds an assignment that satisfies (at least) $$(7/8 + \varepsilon)m$$ of the clauses.

The proof of the above is _far_ more non-trivial compared to the previous two. Interested readers can learn more in [this paper](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.16.5701&rep=rep1&type=pdf) by Johan Håstad.