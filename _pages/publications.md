---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: false
---

<!-- {% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %} -->


- **Near-Optimal Dimension Reduction for Facility Location**  
  Lingxiao Huang, Shaofeng H.-C. Jiang, Robert Krauthgamer, **Di Yue** <br>
  Accepted to [*STOC 2025*](https://acm-stoc.org/stoc2025/). <br>
  [[arXiv](https://arxiv.org/abs/2411.05432)]
  [[slides](/files/dim_reduction_FL/FL_talk_Weizmann.pdf)]
  <details><summary>Abstract</summary>
  <font size=2>
  Oblivious dimension reduction, à la the Johnson-Lindenstrauss (JL) Lemma,
  is a fundamental approach for processing high-dimensional data.
  We study this approach for Uniform Facility Location (UFL)
  on a Euclidean input $X \subset\mathbb R^d$,
  where facilities can lie in the ambient space (not restricted to $X$).
  Our main result is that target dimension $m=\tilde{O}(\epsilon^{-2} \mathrm{ddim})$
  suffices to $(1+\epsilon)$-approximate the optimal value of UFL
  on inputs whose doubling dimension is bounded by $\mathrm{ddim}$.
  It significantly improves over previous results, that could only achieve
  $O(1)$-approximation [Narayanan, Silwal, Indyk, and Zamir, ICML 2021]
  or dimension $m=O(\epsilon^{-2}\log n)$ for $n=|X|$,
  which follows from [Makarychev, Makarychev, and Razenshteyn, STOC 2019]. <br><br>

  Our oblivious dimension reduction
  has immediate implications to streaming and offline algorithms,
  by employing known algorithms for low dimension.
  In dynamic geometric streams, 
  it implies a $(1+\epsilon)$-approximation algorithm
  that uses $O(\epsilon^{-1}\log n)^{\tilde{O}(\mathrm{ddim}/\epsilon^{2})}$ bits of space,
  which is the first streaming algorithm for UFL to utilize the doubling dimension.
  In the offline setting, it implies a $(1+\epsilon)$-approximation algorithm,
  which we further refine to run in time
  $((1/\epsilon)^{\tilde O(\mathrm{ddim})} d +  2^{(1/\epsilon)^{\tilde O(\mathrm{ddim})}}) \cdot \tilde{O}(n)$. 
  Prior work has a similar running time but requires some restriction
  on the facilities [Cohen-Addad, Feldmann and Saulpic, JACM 2021]. <br><br>

  Our main technical contribution is a fast procedure to decompose
  an input $X$ into several $k$-median instances for small $k$.
  This decomposition is inspired by, but has several significant differences from [Czumaj, Lammersen, Monemizadeh and Sohler, SODA 2013],
  and is key to both our dimension reduction and our PTAS. <br>
  </font>
  </details>