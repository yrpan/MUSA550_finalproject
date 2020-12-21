---
title: "Data Visualizations for the K-Means Clustering Analysis of Chicago Population"
date: 2020-12-21
published: true
tags: [dataviz, matplotlib, altair]
excerpt: "The scree plot, interactive altair plots, results table"
altair-loader:
  altair-chart-1: "charts/clustermap.json"
toc: true
toc_sticky: true
---

# 1. Select # of clusters with the scree plot

Below shows that the elbow in the plot of SSE against clustering solution is about 3 (from 2 to 3 there is a distinct drop in within groups sum of squares), after which this decrease drops off dramatically, suggesting that a 3-cluster solution may be a good fit to the data. Generally, a smaller number around 2 or 3 is better as it increases the interpretability of the clustering results.

![scree-plot]({{ site.url }}{{ site.baseurl }}/assets/images/screeplot.png)

# 2. Interactive Altair Plots

<div id="altair-chart-1"></div>

This was produced using Altair and embedded in this static web page. 

```python
import altair as alt
alt.renderers.enable('notebook')