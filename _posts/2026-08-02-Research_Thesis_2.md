---
layout: default
title: "Gaining Unauthorised Access to an 802.1X and IPv6 Configured Network"
date: 2016-08-02
---

# Gaining Unauthorised Access to an 802.1X and IPv6 Configured Network

During my MSc System and Network Engineering at the University of Amsterdam, I worked together with Robert Diepeveen on a research project focused on network access control and IPv6 security. The research investigated whether it was possible to gain unauthorized access to an 802.1X protected network by piggybacking on an already authenticated user's network session. 【1-bdf6ed】

At the time, several techniques for bypassing 802.1X controls in IPv4 environments had already been published. However, little research existed regarding the applicability of these techniques within IPv6 networks. As organizations increasingly adopted IPv6, we wanted to understand whether the transition introduced meaningful barriers for attackers or whether existing attack concepts remained effective. 【1-bdf6ed】

Our primary research question was:

> Is it possible to gain unauthorised access to an 802.1X and IPv6 configured network? 【1-bdf6ed】

To answer this question, we first analyzed existing attacks against 802.1X protected IPv4 environments and identified the components that made these attacks possible. We then translated those concepts to IPv6 through literature research and practical validation in a controlled lab environment. 【1-bdf6ed】

The research demonstrated that piggybacking on an authenticated 802.1X session remained feasible within an IPv6 environment and was not fundamentally different from its IPv4 counterpart. We also explored several mitigation strategies, including IPsec, MACsec, Secure Neighbor Discovery (SEND), and intrusion detection technologies. 【1-bdf6ed】

One of the key lessons from this project was that authentication mechanisms often protect access to a network, but not necessarily the authenticated session itself. Understanding the distinction between authentication, authorization and session security remains essential when designing secure enterprise networks. 【1-bdf6ed】

Looking back, this research further strengthened my interest in offensive security and demonstrated the importance of validating security assumptions as organizations adopt new technologies and protocols.

The full paper can be found here:

**[Gaining Unauthorised Access to an 802.1X and IPv6 Configured Network](https://www.os3.nl/_media/2015-2016/courses/rp2/p87_report.pdf)**. 【1-bdf6ed】
``
