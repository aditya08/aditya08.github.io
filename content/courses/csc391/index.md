---
title: "CSC 391/691: Algorithms for Large-Scale Machine Learning"
date: 2026-08-26
url: /courses/csc391-691/
tags: ["machine learning","high-performance computing","parallel algorithms","distributed-memory","GPU programming","communication avoidance","performance modeling","reproducibility","computer science education"]
author: ["Aditya Devarakonda"]
description: "CSC 391/691 at Wake Forest: designing, implementing, and evaluating machine-learning algorithms under communication, memory, and hardware constraints."
summary: "A dual-listed undergraduate and graduate course at Wake Forest University on algorithms for large-scale machine learning. Students derive cost models, implement distributed and GPU methods on a production cluster, and audit performance claims. Offered Fall 2026."
showToc: false
disableAnchoredHeadings: false
hideMeta: false
---

**Wake Forest University, Department of Computer Science**<br>
Fall 2026 · Wednesdays and Fridays, 2:00–3:15 p.m. · Alumni Hall 289<br>
Instructor: [Aditya Devarakonda](/bio/) · Dual-listed for undergraduate (CSC 391) and graduate (CSC 691) credit

---

### Course Description

Large-scale machine-learning algorithms must use data, memory, processors, accelerators, and networks together. On modern computing systems, communication and memory traffic often cost more than arithmetic, so an algorithm that is mathematically sound can still fail to scale. This course studies how to design, implement, and evaluate learning algorithms under those constraints.

Three questions run through the semester. Given a machine-learning algorithm:

- What computation, communication, and memory traffic does it require?
- Where is the bottleneck, and how does the bottleneck change with problem size and hardware scale?
- What evidence supports a performance or deployment claim, and what remains unknown?

Given a learning task and a computing system, students use cost models, implementations, measurements, and claim audits to decide which design is justified.

Compared with a traditional machine-learning course, this course emphasizes algorithmic scalability and system constraints rather than statistical modeling. Topics include stochastic optimization, distributed learning, GPU computation, communication-efficient algorithms, performance modeling, reproducibility, and responsible deployment.

There are no formal prerequisites. Students are expected to be able to program and to have completed a data structures course; no prior study of machine learning, numerical linear algebra, or parallel programming is assumed. The opening weeks build that background, and every programming assignment provides a starter repository so that assessed work stays focused on algorithms, measurements, and reasoning.

---

### Learning Objectives

At the end of the course, students will be able to:

- derive computation, communication, and memory-cost models for machine-learning algorithms on parallel systems,
- design and implement stochastic, distributed, and GPU-based learning methods that reduce communication,
- measure convergence and performance, report variability, and explain weak or strong scaling behavior,
- evaluate trade-offs among algorithmic efficiency, statistical performance, reproducibility, and system constraints,
- audit claims in research papers, generated analyses, and their own experiments by separating evidence from inference, and
- identify limits in technical evidence and deployment expertise, then justify whether a system should be deployed, redesigned, delayed, limited, or withheld.

---

### Character and Judgment in Technical Work

The final two objectives develop **virtue perception** through humility and temperance in research, algorithm design, and deployment. Students are assessed on what they notice, how they support and revise claims, and how they justify action under uncertainty — not on reaching a preferred conclusion or displaying a personal character trait.

This emphasis runs through the graded structure rather than sitting beside it:

- **Claim audits.** Students decompose a generated or published performance claim, identify what the evidence actually supports, design corrective measurements, and rewrite the claim at the scope the evidence permits.
- **Individual live defenses.** Each engineering study ends with an oral defense in which students explain design choices, interpret unexpected results, and reason about constraints introduced in discussion. The defense determines half of the study grade.
- **Negative results earn full credit.** A well-designed experiment that produces a negative or null result can earn full credit. The quality of the investigation is what is assessed, not whether the experiment produced a positive result.
- **Evidence standards in every artifact.** Homeworks and studies require a defensible baseline, performance variability across at least three runs, at least two problem scales, and a limitations section naming experiments not performed.
- **Generative AI as a detection target.** Generative AI is permitted and encouraged on homeworks and studies, subject to one non-negotiable condition: students must be able to explain, justify, and adapt anything they submit without assistance. Because generative AI produces confident, well-formatted, and incorrect claims, detecting those failures is itself a learning objective. Exams and defenses are closed-book, so 62.5% of the course grade rests on demonstrated understanding.

This work is supported by the Wake Forest [Program for Leadership and Character](https://leadershipandcharacter.wfu.edu/).

---

### Course Structure

Students run real jobs on **DEAC**, Wake Forest's production HPC cluster, using multi-node allocations and GPU partitions. The course has seven graded artifacts in four categories:

| Component | Weight |
|---|---|
| Three homeworks | 20% |
| Two engineering studies | 35% |
| Written midterm | 20% |
| Oral final | 25% |

The three homeworks cover foundations and benchmarking, distributed scaling and its cost model, and a GPU kernel applied to a learning workload. Each produces measurements or code that a later engineering study reuses, so work is revised rather than discarded.

The two engineering studies are substantial investigations — a distributed scaling study and a kernel-and-workload study — each consisting of real runs on DEAC, a report, software, and an individual live defense.

**Dual-listing.** CSC 391 and CSC 691 share the same concepts, rigor floor, midterm, and oral final. CSC 691 students evaluate one additional experimental condition in each homework and engineering study, and lead a second research-paper discussion. The additional condition may be another problem scale, hardware configuration, or baseline.

---

### Course Calendar

| Dates | Module | Topics |
|---|---|---|
| Aug 26, 28 | Foundations | Course framing and what "large-scale" means; linear algebra and numerical computing |
| Sep 2, 4 | Foundations | Machine-learning basics; SGD and coordinate descent |
| Sep 9, 11 | Foundations | DEAC mini-tutorial, regularization, and stopping criteria; optimization at scale and benchmarking hygiene |
| Sep 16, 18 | Distributed | SPMD, MPI collectives, and SLURM; parameter servers and synchronous versus asynchronous methods |
| Sep 23, 25 | Distributed | Communication bottlenecks and cost models; communication-avoiding algorithms |
| Sep 30, Oct 2 | GPU | Execution model, memory hierarchy, and launch configuration; linear-algebra kernels and achieved versus peak bandwidth |
| Oct 7, 9 | GPU | Batching and roofline analysis; performance-model workshop and GPU measurement lab |
| Oct 14, 16 | GPU · Exams | Memory-bandwidth limits and profiling; written midterm |
| Oct 21, 23 | Studio · Workloads | Distributed scaling study and individual defenses; kernel methods and GNN scaling |
| Oct 28, 30 | Workloads | Large language models and data provenance; workload characterization |
| Nov 4, 6 | Emerging | Scientific machine learning and simulation; HPC and machine-learning convergence |
| Nov 11, 13 | Emerging | Research case studies and open problems; surrogates, weak baselines, and overclaiming |
| Nov 18, 20 | Studio | Claim-audit workshop and deployment decision practice; counter-evidence and revision |
| Dec 2, 4 | Studio · Review | Kernel and workload study with individual defenses; course synthesis and oral-final review |
| Dec 12 | Exams | Individual oral final |

Research-paper and case discussions run as class activities throughout the semester. CSC 391 students lead one paper discussion; CSC 691 students lead two.

---

### Related

This course is closely tied to the [REASOn Lab](/reason-lab/) research program on resource-efficient algorithms for scalable optimization. Students interested in continuing this work as research are encouraged to get in touch.

Enrolled students should consult Canvas for the authoritative syllabus, assignments, and schedule.
