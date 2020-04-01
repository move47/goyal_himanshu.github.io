---
layout: post
title: "Implementing and Analyzing Homomorphic UC Commitments"
excerpt_separator:  <!--more-->
categories:
  - Publications
tags:
  - 2PC
  - Oblivious Transfer
  - Malicious
  - Roberto Trifiletti
---

Peter Rindal & Roberto Trifiletti  ~ <a href="https://eprint.iacr.org/2017/407">eprint/2017/407</a>

In this paper we present SplitCommit, a portable and efficient C++ implementation of the recent additively homomorphic commmitment scheme of Frederiksen et al. [FJNT16]. We describe numerous optimizations that go into engineering such an implementation, including highly optimized general purpose bit-matrix transposition and efficient ECC encoding given the associated generator matrix. We also survey and analyze in detail the applicability of [FJNT16] and include a detailed comparison to the canonical (non-homomorphic) commitment scheme based on a Random Oracle. We include performance benchmarks of the implementation in various network setting, for instance on a 10 Gbps LAN we achieve amortized commitment and decommitment running times of 0.65μs and 0.27μs, respectively. Finally we also include an extensive tutorial on how to use the library. 

