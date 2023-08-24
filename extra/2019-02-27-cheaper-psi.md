---
layout: post
title: "Cheaper Private Set Intersection via Differentially Private Leakage"
excerpt_separator:  <!--more-->
categories:
  - Publications
tags:
  - 2PC
  - Oblivious Transfer
  - Private Set Intersection
  - Differential Privacy
  - Malicious
  - Adam Groce
  - Mike Rosulek
  - PETS
---

Adam Groce, Peter Rindal & Mike Rosulek ~ <a href="https://eprint.iacr.org/2019/1159">eprint/2019/1159</a> ~ <a href="https://petsymposium.org/cfp19.php">PETS'19</a>

In this work we demonstrate that allowing differentially private leakage can significantly improve the concrete performance of secure 2-party computation (2PC) protocols. Specifically, we focus on the private set intersection (PSI) protocol of Rindal and Rosulek (CCS 2017), which is the fastest PSI protocol with security against malicious participants. We show that if differentially private leakage is allowed, the cost of the protocol can be reduced by up to 63%, depending on the desired level of differential privacy. On the technical side, we introduce a security model for differentially-private leakage in malicious-secure 2PC. We also introduce two new and improved mechanisms for "differentially private histogram overestimates," the main technical challenge for differentially-private PSI. 