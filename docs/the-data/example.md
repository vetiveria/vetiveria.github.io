---
layout: default
title: Example
parent: The Data
nav_order: 3
my_variable: header_latex.html
---

{% if page.my_variable %}
  {% include {{ page.my_variable }} %}
{% endif %}

# Example
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## All

$$\qquad \frac{1}{N} \sum_{i = 0}^{N - 1} {x_{i}^2}$$

This is the ...
