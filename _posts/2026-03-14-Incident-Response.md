---
layout: default
title: "It's Time to Bring Incident Response to the Training Table"
date: 2026-04-14
---

# It's Time to Bring Incident Response to the Red Team Table

Over the past years, organizations have invested heavily in exercising their cyber security capabilities through frameworks such as TIBER-EU, TLPT and ART.

These exercises have undoubtedly increased the maturity of detection and response capabilities. Security Operations Centers are more capable, playbooks are more mature, and defenders have become increasingly familiar with sophisticated attack techniques.

But there is a question we rarely ask:

> Are we actually ready to recover?

During many Red Team exercises, the objective is to assess whether an attack can be detected and contained. Increasingly, organizations succeed in doing exactly that. However, when an incident evolves into a full-scale business disruption, such as ransomware affecting critical systems, a different challenge emerges.

The challenge is no longer detection.

The challenge is recovery.

# Security controls can become recovery obstacles

Many of the security measures we advocate for every day are highly effective during normal operations. Yet during a crisis, those same controls can unexpectedly slow down recovery efforts.

Consider a few examples:

* Local administrator passwords are managed through LAPS, but the Domain Controllers containing the passwords are unavailable.
* USB booting is disabled across the estate, preventing responders from using forensic or recovery media.
* Network segmentation restricts access to systems required for restoration activities.
* Administrative accounts depend on infrastructure that is itself affected by the incident.
* Backup systems are operational, but the tools required to access them are not.

None of these are design flaws.

They are simply examples of a reality that is rarely exercised: recovering an environment while parts of that same environment are unavailable.

# The practical problems nobody talks about

In my incident response experience, some of the biggest challenges were not technical compromises.

They were logistical.

Questions suddenly arise that nobody expected to answer:

* Do we have enough spare laptops for the response team?
* Do we have replacement drives readily available?
* Where is the installation media for critical software?
* Which software versions are actually required?
* Do we have licenses available?
* How do we communicate if corporate email is unavailable?
* What happens if the internet connection needs to be disconnected?
* Is there an alternative internet connection available?
* Do recovery teams have the hardware needed to work from an isolated location?

These are not advanced cyber security questions.

Yet they can become critical blockers during a real incident.

Unfortunately, they are also the type of issues that are often discovered only when responders are already under significant pressure.

# A missing seat at the table

Threat Intelligence teams help identify realistic threats.

Red Teams simulate those threats.

Blue Teams learn how to detect and respond.

But Incident Response and Recovery teams are often involved only after the exercise has ended.

I believe this needs to change.

Incident responders should be involved much earlier when scenarios are designed and executed. Not because they need another technical briefing, but because they understand what happens after the attack succeeds.

They understand:

* Which systems are required for recovery.
* Which dependencies are often overlooked.
* Which emergency procedures actually work.
* Which assumptions break down during a crisis.
* Which practical resources are missing.

That perspective is incredibly valuable during threat intelligence workshops, Red Team planning sessions and Purple Team discussions.

# Exercising recovery readiness

Perhaps the next evolution of cyber exercises is not making attacks more advanced.

Perhaps it is making recovery more realistic.

Alongside questions such as:

> Can the SOC detect this attacker?

we should also ask:

> Can we rebuild this system?

> Can we restore this business process?

> Can we operate if core infrastructure is unavailable?

> What would we need tomorrow morning if this happened tonight?

These questions are often less glamorous than advanced attack techniques, but they are ultimately the questions that determine how quickly an organization recovers.

# Conclusion

TIBER-EU, TLPT and ART have significantly improved the way organizations prepare for sophisticated cyber attacks. The industry should be proud of that progress.

However, cyber resilience is more than prevention, detection and response.

It also includes recovery.

As organizations continue to mature their exercising programs, it may be time to give Incident Response and Recovery specialists a permanent seat at the table. Not after the exercise, but during the planning, execution and evaluation phases.

Because when a serious incident occurs, the most important question is often not how the attacker got in.

It is how quickly the organization can get back on its feet.
