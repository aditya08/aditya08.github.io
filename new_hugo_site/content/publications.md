---
title: ""
date: 2021-04-11
draft: false
---
### Peer-Reviewed Journal Papers
A. Devarakonda, K. Fountoulakis, J. Demmel and M. W. Mahoney, **Avoiding Communication in Primal and Dual Block Coordinate Descent Methods**, SIAM Journal on Scientific Computing (SISC), 2019.  
(<a href="https://doi.org/10.1137/17M1134433" target="_blank">Link</a>)
(<a href="javascript:toggleBlock('DFDM19-abstract')">Abstract</a>) (<a href="javascript:toggleBlock('DFDM19-bibtex')">Bibtex</a>) (<a href="#DFDM16-tr">Technical Report</a>)
<span class="hide-content" id="DFDM19-abstract">Primal and dual block coordinate descent methods are iterative methods for solving regularized and unregularized optimization problems. Distributed-memory parallel implementations of these methods have become popular in analyzing large machine learning datasets. However, existing implementations communicate at every iteration which, on modern data center and supercomputing architectures, often dominates the cost of floating-point computation. Recent results on communication-avoiding Krylov subspace methods suggest that large speedups are possible by re-organizing iterative algorithms to avoid communication. We show how applying similar algorithmic transformations can lead to primal and dual block coordinate descent methods that only communicate every s iterations--where s is a tuning parameter--instead of every iteration for the <em>regularized least-squares problem</em>. We show that the communication-avoiding variants reduce the number of synchronizations by a factor of s on distributed-memory parallel machines without altering the convergence rate and attains strong scaling speedups of up to 6.1× on a Cray XC30 supercomputer.</span>
<pre class="hide-content" id="DFDM19-bibtex"><code>
    @article{DFDM19,  
    title={Avoiding communication in primal and dual block coordinate descent methods},  
    author={Devarakonda, Aditya and Fountoulakis, Kimon and Demmel, James and Mahoney, Michael W},  
    journal={SIAM Journal on Scientific Computing},  
    volume={41},  
    number={1},  
    pages={C1--C27},  
    year={2019},  
    publisher={SIAM}  
    }
</code></pre>

---
M. Parashar, M. Abdelbaky, I. Rodero, and A. Devarakonda, **Cloud Paradigms and Practices for Computational and Data-Enabled Science and Engineering**, Computing in Science and Engineering (CISE), 2013.  
(<a href="https://doi.org/10.1109/MCSE.2013.49" target="_blank">Link</a>)
(<a href="javascript:toggleBlock('PARD13-abstract')">Abstract</a>) (<a href="javascript:toggleBlock('PARD13-bibtex')">Bibtex</a>) (<a href="#PARD12-tr">Technical Report</a>)
<span class="hide-content" id="PARD13-abstract">Clouds are rapidly joining high-performance computing (HPC) systems, clusters, and grids as viable platforms for scientific exploration and discovery. As a result, understanding application formulations and usage modes that are meaningful in such a hybrid infrastructure, and how application workflows can effectively utilize it, is critical. Here, three hybrid HPC/grid and cloud cyber infrastructure usage modes are explored: HPC in the Cloud, HPC plus Cloud, and HPC as a Service, presenting illustrative scenarios in each case and outlining benefits, limitations, and research challenges.</span>
<pre class="hide-content" id="PARD13-bibtex"><code>
    @article{PARD13,
    title={Cloud paradigms and practices for computational and data-enabled science and engineering},
    author={Parashar, Manish and AbdelBaky, Moustafa and Rodero, Ivan and Devarakonda, Aditya},
    journal={Computing in Science \& Engineering},
    volume={15},
    number={4},
    pages={10--18},
    year={2013},
    publisher={IEEE}
    }
</code></pre>

---
D. Villegas, N. Bobroff, I. Rodero, J. Delgado, Y. Liu, A. Devarakonda, L. Fong, S. M. Sadjadi, and M. Parashar, **Cloud Federation in a Layered Service Model**, Journal of Computer and Systems Sciences (JCSS), 2012.  
(<a href="https://doi.org/10.1016/j.jcss.2011.12.017" target="_blank">Link</a>)
(<a href="javascript:toggleBlock('VBR+12-abstract')">Abstract</a>) (<a href="javascript:toggleBlock('VBR+12-bibtex')">Bibtex</a>)
<span class="hide-content" id="VBR+12-abstract">We show how a layered Cloud service model of software (SaaS), platform (PaaS), and infrastructure (IaaS) leverages multiple independent Clouds by creating a federation among the providers. The layered architecture leads naturally to a design in which inter-Cloud federation takes place at each service layer, mediated by a broker specific to the concerns of the parties at that layer. Federation increases consumer value for and facilitates providing IT services as a commodity. This business model for the Cloud is consistent with broker mediated supply and service delivery chains in other commodity sectors such as finance and manufacturing. Concreteness is added to the federated Cloud model by considering how it works in delivering the Weather Research and Forecasting service (WRF) as SaaS using PaaS and IaaS support. WRF is used to illustrate the concepts of delegation and federation, the translation of service requirements between service layers, and inter-Cloud broker functions needed to achieve federation.</span>
<pre class="hide-content" id="VBR+12-bibtex"><code>
    @article{VBR+12,
    title={Cloud federation in a layered service model},
    author={Villegas, David and Bobroff, Norman and Rodero, Ivan and Delgado, Javier and Liu, Yanbin and Devarakonda, Aditya and Fong, Liana and Sadjadi, S Masoud and Parashar, Manish},
    journal={Journal of Computer and System Sciences},
    volume={78},
    number={5},
    pages={1330--1344},
    year={2012},
    publisher={Elsevier}
    }
</code></pre>

### Peer-Reviewed Conference Papers
A. Devarakonda and J. Demmel, **Avoiding Communication in Logistic Regression**, Proceedings of the 27th IEEE International Conference on High Performance Computing, Data, and Analytics (HiPC), 2020, <em>To appear</em>.  
(<a href="javascript:toggleBlock('DDarxiv20-abstract')">Abstract</a>) (<a href="javascript:toggleBlock('DDarxiv20-bibtex')">Bibtex</a>) (<a href="#DD20-tr">Technical Report</a>)
<span class="hide-content" id="DDarxiv20-abstract">Stochastic gradient descent (SGD) is one of the most widely used optimization methods for solving various machine learning problems. SGD solves an optimization problem by iteratively sampling a few data points from the input data, computing gradients for the selected data points, and updating the solution. However, in a parallel setting, SGD requires interprocess communication at every iteration. We introduce a new communication-avoiding technique for solving the logistic regression problem using SGD. This technique re-organizes the SGD computations into a form that communicates every s iterations instead of every iteration, where s is a tuning parameter. We prove theoretical flops, bandwidth, and latency upper bounds for SGD and its new communication-avoiding variant. Furthermore, we show experimental results that illustrate that the new Communication-Avoiding SGD (CA-SGD) method can achieve speedups of up to 4.97× on a high-performance Infiniband cluster without altering the convergence behavior or accuracy.</span>
<pre class="hide-content" id="DDarxiv20-bibtex"><code>
    @article{DDarxiv20,
    author = {{Devarakonda}, Aditya and {Demmel}, James},
    title = "{Avoiding Communication in Logistic Regression}",
    journal = {arXiv e-prints},
    keywords = {Computer Science - Machine Learning, Computer Science - Distributed, Parallel, and Cluster Computing},
        year = 2020,
    month = nov,
        eid = {arXiv:2011.08281},
    pages = {arXiv:2011.08281},
    archivePrefix = {arXiv},
    eprint = {2011.08281},
    primaryClass = {cs.LG},
    adsurl = {https://ui.adsabs.harvard.edu/abs/2020arXiv201108281D},
    adsnote = {Provided by the SAO/NASA Astrophysics Data System}
    }
</code></pre>

---
S. Soori, A. Devarakonda, Z. Blanco, J. Demmel, M. Gurbuzbalaban, M. M. Dehnavi, **Reducing Communication in Proximal Newton Methods for Sparse Least Squares Problems**, Proceedings of the 47th International Conference on Parallel Processing (ICPP), 2018.  
(<a href="https://doi.org/10.1145/3225058.3225131" target="_blank">Link</a>)
(<a href="javascript:toggleBlock('SD+18-abstract')">Abstract</a>) (<a href="javascript:toggleBlock('SD+18-bibtex')">Bibtex</a>) (<a href="#SD+17-tr">Technical Report</a>)
<span class="hide-content" id="SD+18-abstract">Proximal Newton methods are iterative algorithms that solve l1-regularized least squares problems. Distributed-memory implementation of these methods have become popular since they enable the analysis of large-scale machine learning problems. However, the scalability of these methods is limited by the communication overhead on modern distributed architecture. We propose a stochastic variance-reduced proximal method along with iteration-overlapping and Hessian-reuse to find an efficient trade-off between computation complexity and data communication. The proposed RC-SFSITA algorithm reduces latency costs by a factor of k without altering bandwidth costs. RC-SFISTA is implemented on both MPI and Spark and compared to the state-of-the-art framework, ProxCoCoA. The performance of RC-SFISTA is evaluated on 1 to 512 nodes for multiple benchmarks and demonstrates speedups of up to 12× compared to ProxCoCoA with scaling properties that outperform the original algorithm.</span>
<pre class="hide-content" id="SD+18-bibtex"><code>
    @inproceedings{SD+18,
    author = {Soori, Saeed and Devarakonda, Aditya and Blanco, Zachary and Demmel, James and Gurbuzbalaban, Mert and Dehnavi, Maryam Mehri},
    title = {Reducing Communication in Proximal Newton Methods for Sparse Least Squares Problems},
    booktitle = {Proceedings of the 47th International Conference on Parallel Processing},
    series = {ICPP 2018},
    year = {2018},
    isbn = {978-1-4503-6510-9},
    location = {Eugene, OR, USA},
    pages = {22:1--22:10},
    articleno = {22},
    numpages = {10},
    url = {http://doi.acm.org/10.1145/3225058.3225131},
    doi = {10.1145/3225058.3225131},
    acmid = {3225131},
    publisher = {ACM},
    address = {New York, NY, USA},
    }
</code></pre>

---
A. Devarakonda, K. Fountoulakis, J. Demmel, and Michael W. Mahoney, **Avoiding Synchronization in First-Order Methods for Sparse Optimization**, Proceedings of the 32nd International Parallel and Distributed Processing Symposium (IPDPS), 2018.  
(<a href="https://doi.org/10.1109/IPDPS.2018.00051" target="_blank">Link</a>)
(<a href="javascript:toggleBlock('DKDM18-abstract')">Abstract</a>) (<a href="javascript:toggleBlock('DKDM18-bibtex')">Bibtex</a>) (<a href="#DFDM17-tr">Technical Report</a>)
<span class="hide-content" id="DKDM18-abstract">Parallel computing has played an important role in speeding up convex optimization methods for big data analytics and large-scale machine learning (ML). However, the scalability of these optimization methods is inhibited by the cost of communicating and synchronizing processors in a parallel setting. Iterative ML methods are particularly sensitive to communication cost since they often require communication every iteration. In this work, we extend well-known techniques from Communication-Avoiding Krylov subspace methods to first-order, block coordinate descent methods for Support Vector Machines and Proximal Least-Squares problems. Our Synchronization-Avoiding (SA) variants reduce the latency cost by a tunable factor of 's' at the expense of a factor of 's' increase in flops and bandwidth costs. We show that the SA-variants are numerically stable and can attain large speedups of up to 5.1x on a Cray XC30 supercomputer.</span>
<pre class="hide-content" id="DKDM18-bibtex"><code>
    @inproceedings{DKDM18,
    title={Avoiding Synchronization in First-Order Methods for Sparse Convex Optimization},
    author={Devarakonda, Aditya and Fountoulakis, Kimon and Demmel, James and Mahoney, Michael W},
    booktitle={2018 IEEE International Parallel and Distributed Processing Symposium (IPDPS)},
    pages={409--418},
    year={2018},
    organization={IEEE}
    }
</code></pre>

---
A. Gittens, A. Devarakonda, E. Racah, M. Ringenburg, L. Gerhardt, J. Kottalam, J. Liu, K. Maschhoff, S. Canon, J. Chhugani, P. Sharma, J. Yang, J. Demmel, J. Harrell, V. Krishnamurthy, and M. W. Mahoney, **Matrix Factorizations At Scale: A Comparison of Scientific Data Analytics in Spark and C+MPI Using Three Case Studies**, Proceedings of the International Conference on Big Data (BigData), 2016.  
(<a href="https://doi.org/10.1109/BigData.2016.7840606" target="_blank">Link</a>)
(<a href="javascript:toggleBlock('GD+16-abstract')">Abstract</a>) (<a href="javascript:toggleBlock('GD+16-bibtex')">Bibtex</a>) (<a href="#GD+16-tr">Technical Report</a>)
<span class="hide-content" id="GD+16-abstract">We explore the trade-offs of performing linear algebra using Apache Spark, compared to traditional C and MPI implementations on HPC platforms. Spark is designed for data analytics on cluster computing platforms with access to local disks and is optimized for data-parallel tasks. We examine three widely-used and important matrix factorizations: NMF (for physical plausability), PCA (for its ubiquity) and CX (for data interpretability). We apply these methods to 1.6TB particle physics, 2.2TB and 16TB climate modeling and 1.1TB bioimaging data. The data matrices are tall-and-skinny which enable the algorithms to map conveniently into Spark's data-parallel model. We perform scaling experiments on up to 1600 Cray XC40 nodes, describe the sources of slowdowns, and provide tuning guidance to obtain high performance.</span>
<pre class="hide-content" id="GD+16-bibtex"><code>
    @inproceedings{GD+16,
    title={Matrix factorizations at scale: A comparison of scientific data analytics in Spark and C+ MPI using three case studies},
    author={Gittens, Alex and Devarakonda, Aditya and Racah, Evan and Ringenburg, Michael and Gerhardt, Lisa and Kottalam, Jey and Liu, Jialin and Maschhoff, Kristyn and Canon, Shane and Chhugani, Jatin and others},
    booktitle={2016 IEEE International Conference on Big Data (Big Data)},
    pages={204--213},
    year={2016},
    organization={IEEE}
    }
</code></pre>

---
R. Carbunescu, A. Devarakonda, J. Demmel, S. Gordon, J. Alameda, and S. Mehringer, **Architecting an Autograder for Parallel Code**, Proceedings of the Annual Conference on Extreme Science and Engineering Discovery Environment (XSEDE), 2014.  
(<a href="https://doi.org/10.1145/2616498.2616571" target="_blank">Link</a>)
(<a href="javascript:toggleBlock('CD+14-abstract')">Abstract</a>) (<a href="javascript:toggleBlock('CD+14-bibtex')">Bibtex</a>)
<span class="hide-content" id="CD+14-abstract">As parallel computing grows and becomes an essential part of computer science, tools must be developed to help grade assignments for large courses, especially with the prevalence of Massive Open Online Courses (MOOCs) increasing in recent years. This paper describes some of the general challenges related to building an autograder for parallel code with general suggestions and sample design decisions covering presented assignments. The paper explores the results and experiences from using these autograders to enable the XSEDE 2013 and 2014 Parallel Computing Course using resources from SDSC-Trestles, TACC-Stampede and PSC-Blacklight.</span>
<pre class="hide-content" id="CD+14-bibtex"><code>
    @inproceedings{CD+14,
    author = {Carbunescu, Razvan and Devarakonda, Aditya and Demmel, James and Gordon, Steven and Alameda, Jay and Mehringer, Susan},
    title = {Architecting an Autograder for Parallel Code},
    year = {2014},
    isbn = {9781450328937},
    publisher = {Association for Computing Machinery},
    address = {New York, NY, USA},
    url = {https://doi.org/10.1145/2616498.2616571},
    doi = {10.1145/2616498.2616571},
    abstract = {As parallel computing grows and becomes an essential part of computer science, tools must be developed to help grade assignments for large courses, especially with the prevalence of Massive Open Online Courses (MOOCs) increasing in recent years. This paper describes some of the general challenges related to building an autograder for parallel code with general suggestions and sample design decisions covering presented assignments. The paper explores the results and experiences from using these autograders to enable the XSEDE 2013 and 2014 Parallel Computing Course using resources from SDSC-Trestles, TACC-Stampede and PSC-Blacklight.},
    booktitle = {Proceedings of the 2014 Annual Conference on Extreme Science and Engineering Discovery Environment},
    articleno = {68},
    numpages = {8},
    keywords = {Autograding, Online education},
    location = {Atlanta, GA, USA},
    series = {XSEDE '14}
    }
</code></pre>

### Technical Reports
*Technical reports without (Abstract) and (Bibtex) links are superseded by conference and/or journal papers.*  

A. Devarakonda and J. Demmel, **Avoiding Communication in Logistic Regression**, arXiv:2011.08281 (cs.LG), 2020.  
(<a id="DD20-tr" href="https://arxiv.org/abs/2011.08281" target="_blank">Link</a>)

---
A. Devarakonda, K. Fountoulakis, J. Demmel, and M. W. Mahoney, **Avoiding Synchronization in First-Order Methods for Sparse Convex Optimization**, arXiv:1712.06047 (cs.DC), 2017.  
(<a id="DFDM17-tr" href="https://arxiv.org/abs/1712.06047" target="_blank">Link</a>)

---
S. Soori, A. Devarakonda, J. Demmel, M. Gurbuzbalaban, and M. M. Dehnavi, **Avoiding Communication in Proximal Methods for Convex Optimization Problems**, arXiv:1710.08883 (cs.DC), 2017.  
(<a id="SD+17-tr" href="https://arxiv.org/abs/1710.08883" target="_blank">Link</a>)

---
A. Devarakonda, M. Naumov, and M. Garland, **Adabatch: Adaptive Batch Sizes for Training Deep Neural Networks**, arXiv:1712.02029 (cs.LG), 2017.  
(<a href="https://arxiv.org/abs/1712.02029" target="_blank">Link</a>)
(<a href="javascript:toggleBlock('DNG17-abstract')">Abstract</a>) (<a href="javascript:toggleBlock('DNG17-bibtex')">Bibtex</a>)
<span class="hide-content" id="DNG17-abstract">Training deep neural networks with Stochastic Gradient Descent, or its variants, requires careful choice of both learning rate and batch size. While smaller batch sizes generally converge in fewer training epochs, larger batch sizes offer more parallelism and hence better computational efficiency. We have developed a new training approach that, rather than statically choosing a single batch size for all epochs, adaptively increases the batch size during the training process. Our method delivers the convergence rate of small batch sizes while achieving performance similar to large batch sizes. We analyse our approach using the standard AlexNet, ResNet, and VGG networks operating on the popular CIFAR-10, CIFAR-100, and ImageNet datasets. Our results demonstrate that learning with adaptive batch sizes can improve performance by factors of up to 6.25 on 4 NVIDIA Tesla P100 GPUs while changing accuracy by less than 1% relative to training with fixed batch sizes.</span>
<pre class="hide-content" id="DNG17-bibtex"><code>
    @article{DNG17,
    title={AdaBatch: adaptive batch sizes for training deep neural networks},
    author={Devarakonda, Aditya and Naumov, Maxim and Garland, Michael},
    journal={arXiv preprint arXiv:1712.02029},
    year={2017}
    }
</code></pre>

---
A. Gittens, A. Devarakonda, E. Racah, M. Ringenburg, L. Gerhardt, J. Kottalam, J. Liu, K. Maschhoff, S. Canon, J. Chhugani, P. Sharma, J. Yang, J. Demmel, J. Harrell, V. Krishnamurthy, M. W. Mahoney, Prabhat, **Matrix Factorization at Scale: A Comparison of Scientific Data Analytics in Spark and C+MPI Using Three Case Studies**, arXiv:1607.01335 (cs.DC), 2016.  
(<a id="GD+16-tr" href="https://arxiv.org/abs/1607.01335" target="_blank">Link</a>)

---
A. Devarakonda, K. Fountoulakis, J. Demmel, and M. W. Mahoney, **Avoiding Communication in Primal and Dual Block Coordinate Descent Methods**, arXiv:1612.04003 (cs.DC), 2016.  
(<a id="DFDM16-tr" href="https://arxiv.org/abs/1612.04003" target="_blank">Link</a>)

---
N. Totla and A. Devarakonda, **Massive Parallelization of SAT Solvers**, UC Berkeley, 2013.  
(<a href="https://nishanttotla.com/EECSHome/papers/Massive-Parallel-SAT.pdf" target="_blank">Link</a>)
(<a href="javascript:toggleBlock('TD13-abstract')">Abstract</a>) (<a href="javascript:toggleBlock('TD13-bibtex')">Bibtex</a>)
<span class="hide-content" id="TD13-abstract">Boolean Satisfiability (SAT) is a well known NP-complete problem that forms the basis of modern constraint solving. The canonical problem consists of a conjunction of boolean clauses where each clause is a disjunction of literals. The problem is to determine whether there exists a satisfying assignment (and find it if it does). Despite the theoretical hardness of the SAT problem, modern solvers are extremely efficient and sophisticated in terms of the algorithms and heuristics they use. This is especially true for industrial instances generated from practical applications. Even so, further performance gains are harder to produce, while there still exist instances that are unsolvable by modern solvers. Fortunately, this is also a time when the generalization and availability of multicore hardware makes it easier to take advantage of parallel processing capabilities for further speedups. In this paper, we focus on massive parallelization (very large number of processors) of SAT solvers. The goal is to obtain a detailed understanding of the factors that affect performance, communication overheads and efficient ways to encode domain specific knowledge.</span>
<pre class="hide-content" id="TD13-bibtex"><code>
    @article{TD13,
    title={Massive Parallelization of SAT Solvers},
    author={Totla, Nishant and Devarakonda, Aditya},
    year={2013}
    }
</code></pre>

---
M. Parashar, M. Abdelbaky, I. Rodero, and A. Devarakonda **Cloud Paradigm and Practices for CDS&E**, Cloud and Autonomic Computing Center Research Report, 2012.  
(<a id="PARD12-tr" href="https://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.363.4913" target="_blank">Link</a>)