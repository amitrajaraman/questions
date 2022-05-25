---
layout: 	page
title:	Crossing Number Inequality
---

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async
      src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>

**Question.**    
Let $$G$$ be a graph. Define its _edge crossing number_ $$cr(G)$$ to be the least number of edge crossings in a planar drawing of it. Prove that if $$G$$ has $$n$$ vertices and $$m>4n$$ edges,
$$\operatorname{cr}(G) \geq \frac{m^3}{64n^2}.$$

<details>
	<summary> <b>Hint</b> </summary>

To start, try showing that the edge crossing number is at least \(m-3n\).
</details>

<p></p>

<details>
	<summary> <b>Solution</b> </summary>

First, we shall prove that the edge crossing number is at least \(m-3n\). To do so, we show that for any planar graph with \(n\geq 3\) vertices and \(m\) edges, \(m\leq 3n-6\). Indeed, observe that any face borders at least \(3\) edges and each edge borders at most \(2\) faces. As a result, the number of faces is at most \(2m/3\). We may then use Euler's formula to conclude that \(m = n+f-2 \leq n - 2 + 2m/3\), where \(f\) is the number of faces. It follows that \(m\leq 3n-6\). <br>
Now, suppose we draw the graph \(G\) such that the number of crossings is equal to \(\operatorname{cr}(G)\). Observe that any crossing can be removed by deleting one of the two edges involved. Doing so, we obtain a planar graph. Therefore, \(m-\operatorname{cr}(G) \leq 3n-6\), proving the result (the case with \(n<3\) is easily shown).
<p></p>
Let \(0<p<1\), which we shall fix later. Consider a random subgraph \(H\) such that each vertex of \(G\) is in \(H\) with probability \(p\) and an edge in \(G\) is present in \(H\) iff both its vertices are present.    
The bound above implies that
\[ \operatorname{cr}(H) \geq m_H - 3n_H. \]
Observe that a crossing in \(G\) is present in \(H\) only if all of the \(4\) vertices involved are chosen. Taking the expectation of either side, we get
\[ p^4\operatorname{cr}(G) \geq p^2m-3pn. \]
Setting \(p = 4n/m < 1\) completes the proof.
</details>