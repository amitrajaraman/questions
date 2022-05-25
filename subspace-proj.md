---
layout: page
title: Projection of a subspace
---

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async
      src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>

**Question.**
Given a $$k$$-dimensional subspace $$V$$ of $$\mathbb{R}^n$$, show that there exist indices $$i_1,\ldots,i_k$$ such that on defining $$W = \operatorname{span}(e_{i_1}, e_{i_2}, \ldots, e_{i_k})$$, the function $$\pi : V \to W$$ that maps any $$v \in V$$ to $$\sum_{j = 1}^{k} \langle v,e_{i_j}\rangle e_{i_j}$$ under the standard inner product $$\langle\cdot,\cdot\rangle$$.


<details>
	<summary> <b>Solution</b> </summary>

Let \(v_1,\ldots,v_k\) be a basis of \(V\). Consider the \(n \times k\) matrix \(M\) with \(M_{ij}\) equal to the \(i\)th coordinate of \(v_j\). Because the \(v_i\) are linearly independent, \(M\) has column rank \(k\). Consequently, it has row rank \(k\) so there are indices (row numbers) \(i_1,\ldots,i_k\) such that the \(k \times k\) submatrix of \(M\) with these rows is full-rank. As a result, the projections of these basis elements (onto the \(W\) corresponding to these indices) are linearly independent, so \(\pi\) is an injection and we are done.

</details>