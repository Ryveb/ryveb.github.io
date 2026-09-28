---

layout: default
title: "Which Offensive Security Certification Should You Choose?"
date: 2026-09-10
---

# Which Offensive Security Certification Should You Choose?

Over the past few years, I have completed several offensive security certifications:

* OSCP
* OSEP
* OSWP
* CARTP
* CRTO
* CRTL

At the moment, I am also working on CAPE.

A question I regularly see is:

> Which offensive security certification should I choose?

There is no single answer to that question.

Although many of these certifications fall under the broad category of offensive security, they focus on very different skills. Some are heavily focused on penetration testing, others on Active Directory, red teaming, cloud environments or wireless security.

In this post, I want to explain how I see these certifications after going through them myself, what I think each certification is useful for, and which one I would choose depending on your goal.

---

## OSCP

The OSCP is probably the most well-known certification on this list.

For me, OSCP is mainly a penetration testing certification. It teaches you how to approach machines methodically, identify vulnerabilities, exploit them and escalate privileges.

The biggest value of OSCP is not necessarily a specific technique. It is learning how to work independently and create a sound methodology.

You will spend a lot of time enumerating systems, testing ideas, getting stuck and trying another approach.

### Good for

* People starting with penetration testing
* Building a broad offensive security foundation
* Learning enumeration and exploitation
* Linux and Windows privilege escalation
* Learning to troubleshoot your own attacks

### Less focused on

* Advanced Active Directory attacks
* Red team operations
* Command and Control infrastructure
* Cloud attacks
* Evasion

If you are relatively new to offensive security and want a strong general foundation, OSCP still makes a lot of sense.

---

## OSEP

OSEP feels like a logical continuation after OSCP.

Where OSCP mostly teaches you how to compromise systems, OSEP focuses much more on operating in environments where security controls are actively trying to stop you.

This includes areas such as:

* Application whitelisting
* Antivirus and endpoint security evasion
* PowerShell
* Lateral movement
* Active Directory attacks
* Pivoting
* More advanced exploitation techniques

OSEP is therefore much closer to the type of problems you can encounter during more mature penetration tests and red team engagements.

One of the main differences with OSCP is that simply having an exploit is often not enough anymore. You also need to think about how you deliver it, how you execute it and how you move further into the environment.

### Good for

* People who already understand penetration testing
* Learning to work around security controls
* Advanced Windows environments
* Active Directory attacks
* Lateral movement
* Developing a more attacker-like mindset

I would not recommend starting with OSEP without already having a solid offensive security foundation.

---

## CRTO

CRTO is where the focus changes significantly.

Instead of traditional penetration testing, CRTO focuses much more on red team operations.

A large part of the course revolves around using a Command and Control framework and operating inside an Active Directory environment.

This introduces concepts such as:

* C2 infrastructure
* Beacons
* Credential access
* Kerberos attacks
* Lateral movement
* Active Directory attack paths
* Operational security

For me, this type of training is particularly useful because it connects individual attack techniques into an actual operation.

Instead of thinking:

> How do I exploit this machine?

You start thinking more like:

> I have access to this system. What information can I collect, where can I move next and how can I reach my objective?

That is an important difference between penetration testing and red teaming.

### Good for

* People interested in red teaming
* Command and Control
* Understanding attack paths
* Learning how offensive operations are structured

If your goal is to move from penetration testing towards red teaming, CRTO is one of the certifications I would seriously consider.

---

## CRTL

CRTL continues where CRTO stops.

It focuses on more advanced red team tradecraft and assumes that you already understand the concepts covered in CRTO.

The important difference is that the technical challenges become more difficult and you need to think more carefully about how you operate.

This makes it much more relevant for people who already have some experience with red team operations.

### Good for

* Experienced penetration testers
* Red team operators
* More advanced Active Directory environments
* Advanced C2 usage
* Evasion and operational tradecraft
* People who already completed CRTO or have equivalent knowledge

---

## CARTP

CARTP has a much more specific focus: Azure and Entra ID.

This makes it quite different from certifications such as OSCP or CRTO.

Instead of attacking a traditional on-premises Active Directory environment, you start looking at identities, permissions and attack paths in Microsoft cloud environments.

That becomes increasingly important because many organisations now have hybrid environments consisting of both:

Understanding only traditional Active Directory is therefore becoming less sufficient for offensive security professionals.

### Good for

* Azure security
* Entra ID attacks
* Cloud identity
* Hybrid environments
* People already comfortable with Active Directory

I would especially recommend CARTP if you already understand traditional Active Directory and want to expand into Microsoft cloud environments.

---

## OSWP

OSWP is the outlier in this list.

It focuses specifically on wireless security.

You work with concepts surrounding Wi-Fi networks, authentication and attacks against wireless infrastructure.

Compared with OSCP, OSEP or CRTO, the scope is much narrower.

That is not necessarily a bad thing. It simply means that I would choose OSWP because I specifically want to learn wireless security, rather than because I want a general offensive security certification.

### Good for

* Wireless penetration testing
* Understanding Wi-Fi attacks
* People who want a specialised certification

For most penetration testers, I would consider this an additional skill rather than the main certification path.

---

## CAPE

At the time of writing this, I am still working on CAPE.

Because of that, I do not want to give a final opinion on the certification yet.

My reason for taking it is to continue developing skills beyond traditional penetration testing and Active Directory-focused offensive security.

Once I have completed it, I will update this section with my full experience.



# Certifications vs Experience

One thing that becomes increasingly obvious after completing multiple certifications is that certifications are only part of the learning process.

A certification gives you:

* A structured learning path
* A lab environment
* Exposure to techniques you may not normally use
* A goal to work towards

But passing an exam does not automatically mean that you can apply all of those techniques during a real engagement.

Real environments are messy.

Tools behave differently. Security controls interfere with attacks. Documentation is incomplete. Networks are segmented. Credentials do not work where you expect them to work.

And perhaps most importantly, during a real engagement you need to understand when a technique is appropriate, not just how to execute it.

That part mainly comes from experience.

---

# Final Thoughts

Looking back at these certifications, I do not think there is one certification that is simply "the best".

They solve different problems.

OSCP gives you a broad penetration testing foundation.

OSEP pushes you towards more advanced offensive techniques and evasion.

CRTO introduces you to red team operations and C2-based attacks.

CRTL takes that further into more advanced red team tradecraft.

CARTP adds Azure and Entra ID to your skill set.

OSWP gives you specialised knowledge of wireless security.

And CAPE is the certification I am currently using to continue that learning path.

The question I would therefore ask is not:

> Which certification is the best?

But:

> Which skill am I currently missing?

Once you can answer that question, choosing the next certification becomes much easier.
