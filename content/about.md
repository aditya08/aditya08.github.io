---
title: ""
date: 2021-04-10
draft: false
---
### Bio
Aditya Devarakonda is an Assistant Professor in the Department of Computer Science at Wake Forest University. Prior to that he was an Assistant Research Scientist in the Department of Physics and Astronomy at Johns Hopkins University. He received his Ph.D. in Computer Science from the University of California, Berkeley in 2018 and his B.S in Computer Engineering from Rutgers University, New Brunswick in 2012.

His research interests are in high performance computing, machine learning, and scientific computing with a focus on the design, analysis, and implementation of efficient parallel algorithms. His prior work includes the development of communication-avoiding algorithms and techniques for machine learning. He was a recipient of the NSF Graduate Research Fellowship and the EECS Department Fellowship while at UC Berkeley.

### Professional Appointments
- *Visiting Scientist, Oak Ridge National Lab (Oak Ridge, TN).*
- *Assistant Professor, Department of Computer Science, Wake Forest University (Winston-Salem, NC).*
- Assistant Research Scientist, Department of Physics and Astronomy, Johns Hopkins University (Baltimore, MD).
- Senior Professional Staff, Large-Scale Analytics Group, Johns Hopkins University Applied Physics Lab (Laurel, MD).

### Ph.D. Thesis
*Avoiding Communication in First Order Methods for Optimization.*  
Thesis Committee: <a href="https://people.eecs.berkeley.edu/~demmel/" target="_blank">Jim Demmel</a>, <a href="https://www.stat.berkeley.edu/~mmahoney/" target="_blank">Michael W. Mahoney</a>, and <a href="https://www.stat.berkeley.edu/~aditya" target="_blank">Aditya Guntuboyina</a>.

(<a href="https://escholarship.org/uc/item/3rm6d2mf" target="_blank">Link</a>)
(<a href="javascript:toggleBlock('D18-abstract')">Abstract</a>) (<a href="javascript:toggleBlock('D18-bibtex')">Bibtex</a>)
<p class="hide-content" id="D18-abstract">Machine learning has gained renewed interest in recent years due to advances in computer hardware (processing power and high-capacity storage) and the availability of large amounts of data which can be used to develop accurate, robust models. While hardware improvements have facilitated the development of machine learning models in a single machine, the analysis of large amounts of data still requires parallel computing to obtain shorter running times or where the dataset cannot be stored on a single machine.<br>
In addition to hardware improvements, algorithm redesign is also an important direction to further reduce running times. On modern computer architectures, the cost of moving data (communication) from main memory to caches in a single machine is orders of magnitude more expensive than the cost of performing floating-point operations (computation). On parallel machines the cost of moving data from one processor to another over an interconnection network is the most expensive operation. The large gap between computation and communication suggests that algorithm redesign should be driven by the goal of avoiding communication and, if necessary, decreasing communication at the expense of additional computation.<br>
Many problems in machine learning solve mathematical optimization problems which, in most non-linear and non-convex cases, requires iterative methods. This thesis is focused on deriving communication-avoiding variants of the block coordinate descent method, which is a first-order method that has strong convergence rates for many optimization problems. Block coordinate descent is an iterative algorithm which at each iteration samples a small subset of rows or columns of the input matrix, solves a subproblem using just the chosen rows or columns, and obtains a partial solution. This solution is then iteratively refined until the optimal solution is reached or until convergence criteria are met. In the parallel case, each iteration of block coordinate descent requires communication. Therefore, avoiding communication is key to attaining high performance.<br>
This thesis adapts well-known techniques from existing work on communication-avoiding (CA) Krylov and s-step Krylov methods. CA-Krylov methods unroll vector recurrences and rearrange the sequence of computation in way that defers communication for s iterations, where s is a tunable parameter. For CA-Krylov methods the reduction in communication cost comes at the expense of numerical instability for large values of s.<br>
We apply a similar recurrence unrolling technique to block coordinate descent in order to obtain communication-avoiding variants which solve the L2-regularized least-squares, L1-regularized least-squares, Support Vector Machines, and Kernel problems. Our communication-avoiding variants reduce the latency cost by a tunable factor of s at the expense of a factor of s increase in computational and bandwidth costs for the L2 and L1 least-squares and SVM problems. The CA-variants for these problems require additional computation and bandwidth in order to update the residual vector. For CA-kernel methods the computational and bandwidth costs do not increase. This is because the CA-variants of kernel methods can reuse elements of the kernel matrix already computed and therefore do not need to compute and communicate additional elements of the kernel matrix.<br>
Our experimental results illustrate that our new, communication-avoiding methods can obtain speedups of up to 6.1x on a Cray XC30 supercomputer using MPI for parallel processing. For CA-kernel methods we show modeled speedups of 26x, 120x, and 197x for MPI on a predicted Exascale system, Spark on a predicted Exascale system, and Spark on a cloud system, respectively. Furthermore we also experimentally confirm that our algorithms are numerically stable for large values of s.<br>
Finally, we also present an adaptive batch size technique which reduces the latency cost of training convolutional neural networks (CNN). With this technique we have achieved speedups of up to 6.25x when training CNNs on up to 4 NVIDIA P100 GPUs. Furthermore, we were able to train the ImageNet dataset using the ResNet-50 network with a batch size of up to 524,228 which would allow neural network training to attain a higher fraction of peak GPU performance than training with smaller batch sizes.</p>
<pre class="hide-content" id="D18-bibtex"><code>
    @phdthesis{D18thesis,
    title={Avoiding Communication in First Order Methods for Optimization},
    author={Devarakonda, Aditya},
    year={2018},
    school={UC Berkeley}
    }
</code></pre>

### Education
- Ph.D. in Computer Science from University of California, Berkeley.
- M.S. in Computer Science from University of California, Berkeley.
- B.S. in Computer Engineering from Rutgers University, New Brunswick.
