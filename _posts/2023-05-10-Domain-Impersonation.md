---
layout: post
title: "Domain Impersonation opportunities amidst TLS availability"
excerpt_separator: <!--more-->
categories:
  - Blog
tags:
  - Internet Security
  - Security and Privacy
# baseurl: /assets/Blog/FL/
---

<!--
---
layout: post associated with malicious actors causing disruptions and malfunctions. This research contributes to the field of ICS security and provides valuable insights for securing industrial processes.
-->

Motivation: This research work investigates the significant threat of do-
main impersonation attacks, wherein attackers create do-
mains that resemble legitimate ones to deceive users into
disclosing sensitive information. The effectiveness of existing
security measures in detecting and preventing such attacks is
analyzed. Specifically, the warning messages in the browsers
and the Safe Browsing API, a prevalent browser-based se-
curity mechanism, are examined in identifying potentially
harmful websites. Our Chrome-based browser study states
that around 45% of look-alike domains are available to buy,
and the browser application only shows warning messages
for only 1%, providing an open area for attackers to launch
malicious webpages. Our research also demonstrates the lim-
itations of relying solely on these mechanisms, as attackers
can easily obtain certificates for look-alike domains through
free certificate authorities such as Let’s Encrypt. We find
that majority of the look-alike domains in our dataset have
valid TLS certificates and that RPKI validity cannot be used
to distinguish these sites. To address this issue, we propose
a solution that combines tools such as DNSTwist and CT
Monitors, which can assist domain owners in identifying
potentially malicious look-alike domains. This solution can
help mitigate the risks of domain impersonation attacks and
improve the security of popular domains on the internet.
The findings of this research work contribute to a more com-
prehensive understanding of the security risks associated
with popular domains and inform the development of more
effective security measures.


**Keywords**: Domain Typosquatting, Google Chrome, Safe
Browsing, RPKI, TLS Certificates

Acknowledgement: This work was done in collaboration with Samina Mulani at Georgia Tech.

**Project Report**  [[pdf]](/docs/SII_Project_Report.pdf)