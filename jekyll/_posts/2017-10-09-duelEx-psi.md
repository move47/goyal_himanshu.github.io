---
layout: post
title: "Malicious-Secure Private Set Intersection via Dual Execution"
excerpt_separator:  <!--more-->
categories:
  - Publications
tags:
  - 2PC
  - Malicious
  - Oblivious Transfer
  - Private Set Intersection
  - Mike Rosulek
  - ccs
---

Peter Rindal & Mike Rosulek ~ <a href="https://eprint.iacr.org/2017/769">eprint/2017/769</a> ~ <a href="https://acmccs.github.io/papers/">CCS'17</a>

Private set intersection (PSI) allows two parties, who each hold a set of items, to compute the intersection of those sets without revealing anything about other items. Recent advances in PSI have significantly improved its performance for the case of semi-honest security, making semi-honest PSI a practical alternative to insecure methods for computing intersections. However, the semi-honest security model is not always a good fit for real-world problems.

In this work, we introduce a new PSI protocol that is secure in the presence of malicious adversaries. Our protocol is based entirely on fast symmetric-key primitives and inherits important techniques from state-of-the-art protocols in the semi-honest setting. Our novel technique to strengthen the protocol for malicious adversaries is inspired by the dual execution technique of Mohassel & Franklin (PKC 2006). Our protocol is optimized for the random-oracle model, but can also be realized (with a performance penalty) in the standard model.

We demonstrate our protocol's practicality with a prototype implementation. To securely compute the intersection of two sets of size 220
requires only 13 seconds with our protocol, which is ∼12× faster than the previous best malicious-secure protocol (Rindal & Rosulek, Eurocrypt 2017), and only 3× slower than the best semi-honest protocol (Kolesnikov et al., CCS 2016). 