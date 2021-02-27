---
layout: page
title:	Partitioning a rectangle
---

**Question.**    
Let $$R$$ be a rectangle that can be partitioned into smaller rectangles, each of which have at least one side of integer length. Prove that $$R$$ has at least one side of integer length.

<details>
	<summary> **Solution** </summary>

Consider the function $$f(x,y)=\sin(2\pi x)\cos(2\pi y)$$. Observe that the integral of $$f$$ over any axis-aligned rectangle is $$0$$ if and only if it has at least one side of integer length. In particular, the integral of $$f$$ over any of the rectangles that $$R$$ is partitioned into is $$0$$, so the integral of $$f$$ over $$R$$ is $$0$$ as well. The required follows.

</details>