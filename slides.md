---
# You can also start simply with 'default'
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://cover.sli.dev
# some information about your slides (markdown enabled)
title: Welcome to Slidev
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# https://sli.dev/guide/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/guide/syntax#mdc-syntax
mdc: true
---

# Welcome to Slidev

Presentation slides for developers

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:edit />
  </button>
  <a href="https://github.com/slidevjs/slidev" target="_blank" alt="GitHub" title="Open in GitHub"
    class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
transition: fade-out
---
Centroids: A1: (2, 10) B1: (5, 8) C1: (1, 2)
| Data Points | Distance to A1 | Distance to B1 | Distance to C1 | Cluster | New Cluster |
|-------------|----------------|----------------|----------------|---------|-------------|
| (2, 10)     |                |                |                |         |             |
| (2, 5)      |                |                |                |         |             |
| (8, 4)      |                |                |                |         |             |
| (5, 8)      |                |                |                |         |             |
| (7, 5)      |                |                |                |         |             |
| (6, 4)      |                |                |                |         |             |
| (1, 2)      |                |                |                |         |             |
| (4, 9)      |                |                |                |         |             |

<br/>

---
transition: slide-up
level: 2
---
Populated: Centroids 1: A1: (2, 10) B1: (5, 8) C1: (1, 2)
| Data Points | Distance to A1 | Distance to B1 | Distance to C1 | Cluster | New Cluster |
|-------------|----------------|----------------|----------------|---------|-------------|
| (2, 10)     |      0          |   3.6             |     8.06           |    A     |             |
| (2, 5)      |      5.0          |        4.2        |         3.16       |   C      |             |
| (8, 4)      |       8.4         |           5.0     |       7.28        |     B    |             |
| (5, 8)      |    3.6            |       0.0         |       7.21        |     B    |             |
| (7, 5)      |        7.07        |       3.6         |            6.71    |   B      |             |
| (6, 4)      |        7.2        |        4.1        |           5.3     |     B    |             |
| (1, 2)      |        8.08        |       7.21         |       0.0         |     C    |             |
| (4, 9)      |    2.2            |        1.4        |         7.6       |    B     |             |


---
transition: slide-up
level: 2
---
Populated: Centroids 2: A1: (2, 10) B1: (6, 6) C1: (1.5, 3.5)
| Data Points | Distance to A1 | Distance to B1 | Distance to C1 | Cluster | New Cluster |
|-------------|----------------|----------------|----------------|---------|-------------|
| (2, 10)     |      0          |   5.6             |     6.51           |    A     |        A     |
| (2, 5)      |      5.0          |        4.12       |         1.58       |   C      |     C        |
| (8, 4)      |       8.4         |           2.82     |       6.51       |     B    |      B       |
| (5, 8)      |    3.6            |       2.23        |       5.700      |     B    |        B     |
| (7, 5)      |        7.07        |       1.41        |            5.700   |   B      |      B       |
| (6, 4)      |        7.2        |        2.0       |           4.52    |     B    |         B    |
| (1, 2)      |        8.06        |       6.40         |       1.56        |     C    |      C       |
| (4, 9)      |    2.23           |        3.60      |         6.04      |    B     |         A    |


---
transition: slide-up
level: 2
---
Populated: Centroids 3: A1: (3, 9.5) B1: (6.5,5.25) C1: (1.5, 3.5)
| Data Points | Distance to A1 | Distance to B1 | Distance to C1 | Cluster | New Cluster |
|-------------|----------------|----------------|----------------|---------|-------------|
| (2, 10)     |      1.1          |   6.5             |     6.51           |    A     |   A          |
| (2, 5)      |      4.61         |        4.51      |         1.58       |   C      |        C    |
| (8, 4)      |       7.43         |           1.95     |       6.51       |     B    |   B        |
| (5, 8)      |    2.5         |       5.70        |       5.700      |     B    |         A   |
| (7, 5)      |        6.02        |       0.55        |            5.700   |   B      |     B       |
| (6, 4)      |        6.26       |        1.34       |           4.52    |     B    |       B     |
| (1, 2)      |        7.76       |       6.38         |       1.58        |     C    |     C       |
| (4, 9)      |    1.11        |        4.50      |         6.04      |    A     |         A    |


---
transition: slide-up
level: 2
---
Populated: Centroids 4: A1: (3.67, 9) B1: (7,4.33) C1: (1.5, 3.5)
| Data Points | Distance to A1 | Distance to B1 | Distance to C1 | Cluster | New Cluster |
|-------------|----------------|----------------|----------------|---------|-------------|
| (2, 10)     |      1.9          |   7.55             |     6.51           |    A    |   A          |
| (2, 5)      |      4.33        |        5.04      |         1.58       |   C      |      C     |
| (8, 4)      |       6.61        |           1.05     |       6.51       |     B    |     B      |
| (5, 8)      |    1.66        |       4.17       |       5.700      |     A    |       A     |
| (7, 5)      |        5.20       |       0.666        |            5.700   |   B      |    B        |
| (6, 4)      |        5.51       |        1.05       |           4.52    |     B    |     B       |
| (1, 2)      |        7.49      |       6.43         |       1.58        |     C    |     C       |
| (4, 9)      |    0.33       |        5.55     |         6.04      |    A     |         A    |