---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<!-- {% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %} -->

Published
------

Submitted
------

- **Near-Optimal Dimension Reduction for Facility Location**  
  Lingxiao Huang, Shaofeng H.-C. Jiang, Robert Krauthgamer, **Di Yue** <br>
  Submitted.
  <details><summary style="color:#7C4700">Abstract</summary>
  <font color = "7C4700">
  Oblivious dimension reduction, a l\`{a}  the Johnson-Lindenstrauss (JL) Lemma, is a fundamental approach for processing high-dimensional data. We study this approach for Uniform Facility Location (UFL)on a Euclidean input $X\subset\mathbb{R}^d$, where facilities can lie in the ambient space (not restricted to $X$). Our main result is that target dimension $m=\tilde{O}(\epsilon^{-2}\mathrm{ddim})$ suffices to $(1+\epsilon)$-approximate the optimal value of UFL on inputs whose doubling dimension is bounded by $\mathrm{ddim}$. Previous results could only achieve 
  $O(1)$-approximation [Narayanan, Silwal, Indyk, and Zamir, ICML 2021] or dimension $m=O(\epsilon^{-2}\log n)$, which follows from [Makarychev, Makarychev, and Razenshteyn, STOC 2019].

  Our oblivious dimension reduction
  has immediate implications to streaming and offline algorithms,
  by employing known algorithms for low dimension.
  In the setting of dynamic geometric streams and $X\subseteq [\Delta]^d$,
  it implies an algorithm that achieves $(1 + \epsilon)$-approximation
  using $O(\epsilon^{-1}\log \Delta)^{\tilde{O}(\mathrm{ddim}/\epsilon^{2})}$ bits of space,
  which is the first streaming algorithm for UFL to utilize the doubling dimension.
  In the offline setting, it implies a $(1+\epsilon)$-approximation algorithm,
  which we further refine to run in time
  $( (1/\epsilon)^{\tilde{O}(\mathrm{ddim})} d +  2^{(1/\epsilon)^{\tilde{O}(\mathrm{ddim})}}) \cdot \tilde{O}(n)$. 
  Prior work has a similar running time but requires some restriction
  on the facilities [Cohen-Addad, Feldmann and Saulpic, JACM 2021]. 

  Our main technical contribution is a fast procedure
  that decomposes the input $X$ into several instances of $k$-median.
  This decomposition is key to both our dimension reduction and our PTAS,
  and while inspired by [Czumaj, Lammersen, Monemizadeh and Sohler, SODA 2013],
  it has several significant differences. 
  </font>
  </details>

Manuscripts
------