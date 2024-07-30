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
  $O(1)$-approximation [Narayanan, Silwal, Indyk, and Zamir, ICML 2021] or dimension $m=O(\epsilon^{-2}\log n)$, which follows from [Makarychev, Makarychev, and Razenshteyn, STOC 2019]. <br><br>

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
  on the facilities [Cohen-Addad, Feldmann and Saulpic, JACM 2021]. <br><br>

  Our main technical contribution is a fast procedure
  that decomposes the input $X$ into several instances of $k$-median.
  This decomposition is key to both our dimension reduction and our PTAS,
  and while inspired by [Czumaj, Lammersen, Monemizadeh and Sohler, SODA 2013],
  it has several significant differences.<br>
  </font>
  </details>

- **Spanners in Planar Domains via Steiner Spanners and non-Steiner Tree Covers**
  <br>
  Sujoy Bhore and Balázs Keszegh and Andrey Kupavskii and **Hung Le** and Alexandre Louvet and Dömötör Pálvölgyi and Csaba D. Tóth.
  <br>[[PDF](https://arxiv.org/abs/2404.05045)][[blog post](https://minorfree.github.io/SFTreeCover/)]
  <br>Manuscript.
  <details><summary style="color:#7C4700">Abstract</summary>
  <font color = "7C4700">
  
  We study spanners in planar domains, including polygonal domains, polyhedral terrain, and planar metrics. Previous work showed that for any constant $\epsilon\in (0,1)$, one could construct a $(2+\epsilon)$-spanner with $O(n\log(n))$ edges (SICOMP 2019), and there is a lower bound of $\Omega(n^2)$ edges for any $(2-\epsilon)$-spanner (SoCG 2015). The main open question is whether a linear number of edges suffices and the stretch can be reduced to $2$. We resolve this problem by showing that for stretch $2$, one needs $\Omega(n\log n)$ edges, and for stretch $2+\epsilon$ for any fixed $\epsilon \in (0,1)$, $O(n)$ edges are sufficient. Our lower bound is the first super-linear lower bound for stretch $2$. <br><br>
  
  En route to achieve our result, we introduce the problem of constructing non-Steiner tree covers for metrics, which is a natural variant of the well-known Steiner point removal problem for trees (SODA 2001). Given a tree and a set of terminals in the tree,  our goal is to construct a collection of a small number of dominating trees such that for every two points, at least one tree in the collection preserves their distance within a small stretch factor. Here, we identify an unexpected threshold phenomenon around  $2$ where a sharp transition from $n$ trees to $\Theta(\log n)$ trees and then to $O(1)$ trees happens. Specifically, (i) for stretch $ 2-\epsilon$, one needs $\Omega(n)$ trees; (ii) for stretch $2$, $\Theta(\log n)$ tree is necessary and sufficient; and (iii) for stretch $2+\epsilon$, a constant number of trees suffice. Furthermore, our lower bound technique for the non-Steiner tree covers of stretch $2$ has further applications in proving lower bounds for two related constructions in tree metrics: reliable spanners and locality-sensitive orderings. Our lower bound for locality-sensitive orderings matches the best upper bound (STOC 2022). <br><br>
  
  Finally, we study $(1+\epsilon)$-spanners in planar domains using Steiner points. In planar domains, Steiner points are necessary to obtain a stretch arbitrarily close to $1$. Here, we construct a $(1+\epsilon)$-spanner with an almost linear dependency on $\epsilon$ in the number of edges; the precise bound is $O((n/\epsilon)\cdot \log(\epsilon^{-1}\alpha(n))\cdot \log \epsilon^{-1})$ edges, where $\alpha(n)$ is the inverse Ackermann function. Our result generalizes to graphs of bounded genus. For $n$ points in a polyhedral metric, we construct a Steiner $(1+\epsilon)$-spanner with $O((n/\epsilon)\cdot \log(\epsilon^{-1}\alpha(n))\cdot \log \epsilon^{-1})$ edges.<br>
  </font>
  </details>

Manuscripts
------