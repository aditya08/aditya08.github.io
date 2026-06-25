---
title: "High-Performance Star-M SVD for Big Data Compression"
date: 2026-05-15
tags: ["tensor decomposition","t-SVDM","data compression","shared-memory","parallel algorithms"]
author: ["Md Taufique Hussain","Grey Ballard","Aditya Devarakonda","Srinivas Eswar","Naman Pesricha","Vishwas Rao"]
description: "This paper presents a shared-memory parallel, high-performance implementation of the star-M SVD for compressing large scientific tensors"
summary: "Tensor-based decomposition methods compress large datasets with less accuracy loss than traditional matrix methods. Under the star-M tensor framework, tensors decompose in a matrix-mimetic way through the star-M SVD, which carries optimality guarantees but has been confined to productivity-oriented language implementations. We present a shared-memory parallel, high-performance implementation built on batched tensor-times-matrix and slice-wise SVD kernels, achieving a 42x strong-scaling speedup from 1 to 64 threads on the ncep-air-6 dataset."
hiddenInList: true
cover:
    image: "splash.png"
    alt: "Taylor-Green vortex reconstruction via star-M SVD compression"
    relative: true
editPost:
    URL: "https://github.com/pmichaillat/hugo-website"
    Text: "Preprint, arXiv:2605.16058"

---

##### Download

+ [Paper](https://arxiv.org/abs/2605.16058)

---

##### Abstract

In the era of big data, effectively compressing large datasets while performing complex mathematical operations is crucial. Tensor-based decomposition methods have shown superior compression capabilities with minimal loss of accuracy compared to traditional matrix methods. Under the star-M tensor framework, tensors can be decomposed in a matrix-mimetic way, including using the star-M SVD. This tensor SVD has optimality guarantees and has shown exceptional performance on specific types of data, but software implementations have been mostly limited to productivity-oriented languages. In this work, we present our development of a shared-memory parallel, high-performance solution designed to efficiently implement the underlying algorithms. This software will enable optimal compression of extensive scientific datasets, paving the way for enhanced data analysis and insights.

---

##### Figure 6: Strong scaling of the star-M SVD on the ncep-air-6 dataset

![](figure.png)

---

##### Citation

Md Taufique Hussain, Grey Ballard, Aditya Devarakonda, Srinivas Eswar, Naman Pesricha and Vishwas Rao, "High-Performance Star-M SVD for Big Data Compression", *arXiv:2605.16058*, 2026. https://arxiv.org/abs/2605.16058

```latex
@misc{hussain2026highperformance,
      title={High-Performance Star-M SVD for Big Data Compression},
      author={Md Taufique Hussain and Grey Ballard and Aditya Devarakonda and Srinivas Eswar and Naman Pesricha and Vishwas Rao},
      year={2026},
      eprint={2605.16058},
      archivePrefix={arXiv},
      primaryClass={cs.DC},
      url={https://arxiv.org/abs/2605.16058},
}
```

---
