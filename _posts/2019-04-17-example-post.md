---
title: "Clustering Analysis of Chicago Population"
date: 2020-12-21
published: true
tags: [dataviz, matplotlib]
excerpt: "This is an example blog post"
toc: true
toc_sticky: true
---

# 1. Select # of clusters with the scree plot

Below shows that the elbow in the plot of SSE against clustering solution is about 3 (from 2 to 3 there is a distinct drop in within groups sum of squares), after which this decrease drops off dramatically, suggesting that a 3-cluster solution may be a good fit to the data. Generally, a smaller number around 2 or 3 is better as it increases the interpretability of the clustering results.

![scree-plot]({{ site.url }}{{ site.baseurl }}/assets/images/screeplot.png)

# 2.
