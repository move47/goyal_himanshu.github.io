---
layout: post
title: "Fast Private Set Intersection from Homomorphic Encryption"
excerpt_separator:  <!--more-->
categories:
  - Publications
tags:
  - 2PC
  - Semi-honest
  - FHE
  - Private Set Intersection
  - Hao Chen 
  - Kim Laine
  - ccs
---

Hao Chen and Kim Laine and Peter Rindal ~ <a href="https://eprint.iacr.org/2017/299">eprint/2017/299</a> ~ <a href="https://acmccs.github.io/papers/">CCS'17</a>

Private Set Intersection (PSI) is a cryptographic technique that allows two parties to compute the intersection of their sets without revealing anything except the intersection. We use fully homomorphic encryption to construct a fast PSI protocol with a small communication overhead that works particularly well when one of the two sets is much smaller than the other, and is secure against semi-honest adversaries.
<!--more-->

The most computationally efficient PSI protocols have been constructed using tools such as hash functions and oblivious transfer, but a potential limitation with these approaches is the communication complexity, which scales linearly with the size of the larger set. This is of particular concern when performing PSI between a constrained device (cellphone) holding a small set, and a large service provider (e.g. _WhatsApp_), such as in the Private Contact Discovery application.
Our running-time-optimized benchmarks show that it takes 36 seconds of online-computation, 71 seconds of non-interactive (receiver-independent) pre-processing, and only 12.5MB of round trip communication to intersect five thousand 32-bit strings with 16 million 32-bit strings. Compared to prior works, this is roughly a 38--115× reduction in communication with minimal difference in computational overhead. 
