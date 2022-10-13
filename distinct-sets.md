---
layout: 	page
title:	Distinct subsets
---

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async
      src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>

**Question.**
Let $$A_1,\ldots,A_n$$ be distinct subsets of $$[n]$$. Prove that there always exists $$i \in [n]$$ such that the sets $$(B_i)$$ defined by $$B_i = A_i \setminus \{i\}$$ are distinct.

<details>
	<summary> <b>Solution</b> </summary>

Suppose otherwise. What this means is that for each \(i\), there are sets \(C_i\) and \(C_i \setminus \{i\}\), both of which are in the \((A_k)\). Consider the \(n\) edges of the poset of subsets defined by these \(C_i\). Clearly, all \(n\) edges are distinct. Further, the subgraph of the poset with these \(n\) edges has at most \(n\) vertices (because there are \(n\) \(A_k\)). As a result, there must be a cycle in the subgraph, which is seen rather easily to yield a contradiction.

</details>