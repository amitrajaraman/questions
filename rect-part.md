---
layout: page
title:	Partitioning a rectangle
---

**Question.**    
Let $$R$$ be a rectangle that can be partitioned into smaller rectangles, each of which have at least one side of integer length. Prove that $$R$$ has at least one side of integer length.

<div id="collapseOne" class="collapse show" role="tabpanel" aria-labelledby="headingOne">
  <div class="card-block">
    Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird on it squid single-origin coffee nulla assumenda shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore wes anderson cred nesciunt sapiente ea proident. Ad vegan excepteur butcher vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic synth nesciunt you probably haven't heard of them accusamus labore sustainable VHS.
  </div>
</div>

**Solution**    
Consider the function $$f(x,y)=\sin(2\pi x)\cos(2\pi y)$$. Observe that the integral of $$f$$ over any axis-aligned rectangle is $$0$$ if and only if it has at least one side of integer length. In particular, the integral of $$f$$ over any of the rectangles that $$R$$ is partitioned into is $$0$$, so the integral of $$f$$ over $$R$$ is $$0$$ as well. The required follows.