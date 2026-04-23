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
In theoretical computer science, authors are listed in alphabetical order.

- **Near Linear Time Approximation Schemes for Clustering of Partially Doubling Metrics** <br>
  Anne Driemel, Jan Höckendorff, Ioannis Psarros, Christian Sohler, **Di Yue**. <br>
  To Appear in [ICALP 2026](https://icalppodcspaa2026.cs.rhul.ac.uk/icalp/). <br>
  [[arXiv](https://arxiv.org/abs/2603.24336)]
  <details><summary>Abstract</summary>
  <font size=2>
  In the metric $k$-median problem we are given a finite metric space $(X\cup Y, \mathbf{d})$ and the objective is to compute a set of $k$ centers $C\subseteq Y$ that minimizes $\sum_{p\in X} \min_{c\in C} \mathbf{d}(p,c)$. In general metric spaces, the 
  best polynomial time algorithm, which is due to Cohen-Addad, Grandoni, Lee, Schwiegelshohn, and Svensson [Cohen-Addad, Grandoni, Lee, Schwiegelshohn, and Svensson; STOC 2025], computes a $(2+\epsilon)$-approximation for arbitrary constant $\epsilon>0$. However, if the metric space has bounded doubling dimension, a near linear time $(1+\epsilon)$-approximation algorithm is known due to the work of Cohen-Addad, Feldmann, and Saulpic [Cohen-Addad, Feldmann, and Saulpic; JACM 2021]. <br><br>

  In this paper, we show that the $(1+\epsilon)$-approximation algorithm can be generalized to the case when either $X$ or $Y$ has bounded doubling dimension (but the other set not).  
  The case when $X$ has bounded doubling dimension is motivated by the assumption that even though $X$ is part of a high-dimensional space, it may be that it is close to a low-dimensional structure. 
  The case when $Y$ has bounded doubling dimension is perhaps more natural. It is motivated by specific clustering problems where the centers are low-dimensional. Specifically, our work in this setting implies the first near linear time approximation algorithm for the  $(k,\ell)$-median problem under discrete Fr\'echet distance when $\ell$ is constant. The latter problem is a version of the $k$-median problem under Fr\'echet distance when the input consists of time series of $z$ reals and where the centers are time series of $\ell$ reals [Driemel, Krivosija, and Sohler; SODA 2016].
  Previously, for this problem no $(1+\epsilon)$-approximation algorithm with running time polynomial in $k$ was known. 
  We also introduce a novel complexity reduction for time series of real values that leads to a similar result for the case of discrete Fr\'echet distance. <br><br>

  In order to solve the case when $Y$ has a bounded doubling dimension, we introduce a form of dimension reduction that replaces points from $X$ by sets of points in $Y$. 
  To solve the case when $X$ has a bounded doubling dimension, we generalize Talwar's decomposition [Talwar, STOC 2004] of doubling metrics to our setting. The running time of our algorithms is $2^{2^t} \tilde O(n+m)$ where $t=O(\mathrm{ddim} \log \frac{\mathrm{ddim}}{\epsilon})$ and where $\mathrm{ddim}$ is the doubling dimension of $X$ (resp.\ $Y$). 
  The results
  also extend to the metric (uncapacitated) facility location problem.
  We believe that our techniques are likely applicable to other problems. 

  </font>
  </details>

- **Dimension Reduction for Clustering: The Curious Case of Discrete Centers** <br>
  Shaofeng H.-C. Jiang, Robert Krauthgamer, Shay Sapir, Sandeep Silwal, **Di Yue**. <br>
  In Proceedings of [ITCS 2026](http://itcs-conf.org/). <br>
  [[doi](https://doi.org/10.4230/LIPIcs.ITCS.2026.82)] 
  [[arXiv](https://arxiv.org/abs/2509.07444)] 
  [[Shay's talk](https://www.youtube.com/watch?v=VBc258LA7YU)]
  <details><summary>Abstract</summary>
  <font size=2>
  The Johnson-Lindenstrauss transform is a fundamental method for dimension
  reduction in Euclidean spaces, that can map any dataset of $n$ points into
  dimension $O(\log n)$ with low distortion of their distances. This dimension
  bound is tight in general, but one can bypass it for specific problems. Indeed,
  tremendous progress has been made for clustering problems, especially in the
  \emph{continuous} setting where centers can be picked from the ambient space
  $\mathbb{R}^d$. Most notably, for $k$-median and $k$-means, the dimension bound
  was improved to $O(\log k)$ [Makarychev, Makarychev and Razenshteyn, STOC
  2019]. <br><br>

  We explore dimension reduction for clustering in the \emph{discrete} setting,
  where centers can only be picked from the dataset, and present two results that
  are both parameterized by the doubling dimension of the dataset, denoted as
  $\operatorname{ddim}$. The first result shows that dimension
  $O_{\epsilon}(\operatorname{ddim} + \log k + \log\log n)$ suffices, and is
  moreover tight, to guarantee that the cost is preserved within factor
  $1\pm\epsilon$ for every set of centers. Our second result eliminates the
  $\log\log n$ term in the dimension through a relaxation of the guarantee
  (namely, preserving the cost only for all approximately-optimal sets of
  centers), which maintains its usefulness for downstream applications. <br><br>

  Overall, we achieve strong dimension reduction in the discrete setting, and
  find that it differs from the continuous setting not only in the dimension
  bound, which depends on the doubling dimension, but also in the guarantees
  beyond preserving the optimal value, such as which clusterings are preserved.
  </font>
  </details>


- **Near-Optimal Dimension Reduction for Facility Location**  <br>
  Lingxiao Huang, Shaofeng H.-C. Jiang, Robert Krauthgamer, **Di Yue**. <br>
  In Proceedings of [STOC 2025](https://acm-stoc.org/stoc2025/). <br>
  [[doi](https://dl.acm.org/doi/10.1145/3717823.3718214)]
  [[arXiv](https://arxiv.org/abs/2411.05432)]
  [[slides](/files/dim_reduction_FL/FL_talk_STOC.pdf)]
  [[talk](https://www.youtube.com/watch?v=L0xXUzmzltw&list=PL2200vk1q4pnCq8BwJXwnD6SohMwST6aY&index=88&t=4s)]
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