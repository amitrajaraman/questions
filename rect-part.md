---
layout: page
title:	Partitioning a rectangle
---

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async
      src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>

**Question.**    
Let \(R\) be an axis-aligned rectangle that can be partitioned into smaller axis-aligned rectangles, each of which has at least one side of integer length. Prove that \(R\) has at least one side of integer length.

<details>
	<summary> <b>Solution</b> </summary>

Consider the function \( f(x,y)=\sin(2\pi x)\cos(2\pi y) \). Observe that the integral of \( f \) over any axis-aligned rectangle is \( 0 \) if and only if it has at least one side of integer length. In particular, the integral of \( f\) over any of the rectangles that \(R\) is partitioned into is \(0\), so the integral of \(f\) over \(R\) is \(0\) as well. The required follows.

</details>