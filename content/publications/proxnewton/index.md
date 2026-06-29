---
title: "Reducing Communication in Proximal Newton Methods for Sparse Least Squares Problems"
date: 2018-08-13
tags: ["proximal Newton methods","communication avoidance","sparse least squares","distributed-memory","Spark"]
author: ["Saeed Soori","Aditya Devarakonda","Zachary Blanco","James Demmel","Mert Gurbuzbalaban","Maryam Mehri Dehnavi"]
description: "This paper presents communication-reducing proximal Newton methods for sparse least-squares problems"
summary: "This work proposes RC-SFISTA with iteration-overlapping and Hessian reuse for sparse least-squares problems. The method reduces latency costs by a factor of $k$ and demonstrates speedups up to 12x compared to ProxCoCoA on MPI and Spark implementations evaluated on 1 to 512 nodes."
hiddenInList: true
cover:
    image: "splash.png"
    alt: "Speedups for CA-SFISTA and CA-SPNM"
    relative: true
editPost:
    URL: "https://doi.org/10.1145/3225058.3225131"
    Text: "Publisher, ACM ICPP'18"

---

##### Download

+ [Paper](https://doi.org/10.1145/3225058.3225131)

---

##### Abstract

Proximal Newton methods are iterative algorithms that solve $\ell_1$-regularized least-squares problems. Distributed-memory implementations of these methods have become popular since they enable the analysis of large-scale machine learning problems. However, the scalability of these methods is limited by the communication overhead on modern distributed architectures. We propose a stochastic variance-reduced proximal method with iteration-overlapping and Hessian reuse to find an efficient trade-off between computation complexity and data communication. The proposed RC-SFISTA algorithm reduces latency costs by a factor of $k$ without altering bandwidth costs. RC-SFISTA is implemented on both MPI and Spark and compared to ProxCoCoA. The performance of RC-SFISTA is evaluated on 1 to 512 nodes for multiple benchmarks and demonstrates speedups of up to 12x compared to ProxCoCoA with scaling properties that outperform the original algorithm.

---

##### Figures 4 and 5: CA-SFISTA and CA-SPNM Speedups

![](figure.png)

---

##### Citation

Saeed Soori, Aditya Devarakonda, Zachary Blanco, James Demmel, Mert Gurbuzbalaban and Maryam Mehri Dehnavi, "Reducing Communication in Proximal Newton Methods for Sparse Least Squares Problems", *Proceedings of the 47th International Conference on Parallel Processing*, pp. 1-10, 2018. https://doi.org/10.1145/3225058.3225131

```latex
@inproceedings{soori2018reducing,
  title={Reducing Communication in Proximal Newton Methods for Sparse Least Squares Problems},
  author={Soori, Saeed and Devarakonda, Aditya and Blanco, Zachary and Demmel, James and Gurbuzbalaban, Mert and Dehnavi, Maryam Mehri},
  booktitle={Proceedings of the 47th International Conference on Parallel Processing},
  pages={1--10},
  year={2018},
  doi={10.1145/3225058.3225131},
  url={https://doi.org/10.1145/3225058.3225131}
}
```

---
