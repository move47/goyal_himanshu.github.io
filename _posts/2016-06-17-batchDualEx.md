---
layout: post
title: Faster Malicious 2-party Secure Computation with Online/Ofine Dual Execution
excerpt_separator:  <!--more-->
categories:
  - Publications
tags:
  - 2PC
  - Malicious
  - Oblivious Transfer
  - Private Set Intersection
  - Garbled Circuit
  - Mike Rosulek
  - Usenix
---


We describe a highly optimized protocol for general-purpose secure two-party computation (2PC) in the presence of malicious adversaries. Our starting point is a protocol of Kolesnikov et. al. (TCC 2015). We adapt that protocol to the online/offline setting, where two parties repeatedly evaluate the same function (on possibly different inputs each time) and perform as much of the computation as possible in an offline preprocessing phase before their inputs are known. Along the way we develop several significant simplifications and optimizations to the protocol.
<!--more-->

We have implemented a prototype of our protocol and report on its performance. When two parties on Amazon servers in the same region use our implementation to securely evaluate the AES circuit 1024 times, the amortized cost per evaluation is _5.1ms offline + 1.3ms online_. The total offline+online cost of our protocol is in fact less than the _online_ cost of any reported protocol with malicious security. For comparison, our protocol's closest competitor (Lindell & Riva, CCS 2015) uses 74ms offline + 7ms online in an identical setup.

Our protocol can be further tuned to trade performance for leakage. As an example, the performance in the above scenario improves to _2.4ms offline + 1.0ms online_ if we allow an adversary to learn a single bit about the honest party's input with probability 2−20
(but not violate any other security property, e.g. correctness). 

Peter Rindal & Mike Rosulek  ~ <a href="https://eprint.iacr.org/2016/632">eprint/2016/632</a> ~ <a href="https://www.usenix.org/conference/usenixsecurity16/list-accepted-papers">Usenix'16</a>
