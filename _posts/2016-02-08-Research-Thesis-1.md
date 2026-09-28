---
layout: default
title: "Exfiltrating data from managed profiles in Android for Work"
date: 2016-02-08
---

# Exfiltrating Data from Managed Profiles in Android for Work

During my MSc System and Network Engineering at the University of Amsterdam, we worked on a research project focused on the security of Android for Work environments. The research examined whether data stored within managed Android work profiles could be accessed or exfiltrated from personal profiles on the same device.

At the time, Android for Work was rapidly gaining adoption as a Bring Your Own Device (BYOD) solution. Organizations could separate business and personal data on employee-owned devices while maintaining a seamless user experience. This naturally raised an important security question: how effective is this separation when the underlying device becomes compromised?

Our research revolved around a central question:

> Is it possible to exfiltrate information from a managed profile to a personal profile in Android for Work?

To answer this question, we analyzed Android's profile separation mechanisms, investigated the Binder Inter Process Communication (IPC) framework, and evaluated how data isolation behaved on rooted devices. During the project, we identified several scenarios where profile separation could potentially be weakened and explored techniques that could lead to data leakage between managed and personal profiles.

One of the key takeaways from the project was that security boundaries within mobile operating systems should not be viewed in isolation. The effectiveness of work profile separation is closely tied to the security of the underlying device, the availability of encryption, and the assumptions made about an attacker's capabilities.

Looking back, this was one of my first security research projects and an important milestone in developing an offensive security mindset: understanding not only how security controls are designed, but also where the assumptions behind those controls can break down.

The full paper is available here:

**[Exfiltrating Data from Managed Profiles in Android for Work](https://www.os3.nl/_media/2015-2016/courses/rp1/p31_report.pdf)**.
