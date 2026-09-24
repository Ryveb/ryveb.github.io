---
layout: default
title: "Can Single Sign On Weaken the Security of Your Crown Jewel Systems?"
date: 2026-06-16
---

# Introduction

Single Sign On (SSO) has become a cornerstone of modern identity management. By allowing users to authenticate once and access multiple applications, SSO improves usability, reduces password fatigue, and simplifies access management.

However, SSO is often misunderstood as a security control in its own right.

In reality, SSO is primarily an access mechanism. While it can strengthen security when combined with additional controls, it can also increase the impact of an identity compromise. During multiple Red Team engagements, I observed how access to a central identity platform enabled attackers to rapidly expand their access to critical applications and sensitive systems.

The challenge is not that SSO is insecure. The challenge is that organizations frequently place too much trust in a single authentication event.

# Identity: The New Security Perimeter

Traditional security architectures focused on protecting networks and systems. Today, attacker activity increasingly revolves around identities.

Modern cloud environments, SaaS applications and hybrid infrastructures rely heavily on centralized identity providers such as Active Directory and Microsoft Entra ID. These platforms often provide access to hundreds or even thousands of applications.

This creates a concentration of trust. If an attacker successfully compromises a privileged identity or gains control over the central identity platform, the compromise can extend far beyond a single system.

The identity platform effectively becomes a gateway to the organization's most valuable assets.

# The Red Team Perspective

During Red Team exercises, the compromise of an identity provider frequently marks a turning point in the engagement.

Once administrative control over an identity platform is obtained, attackers no longer need to compromise each application individually. Existing trust relationships, federated authentication mechanisms and SSO integrations provide opportunities to move directly toward critical business applications.

This does not mean that SSO creates the vulnerability. The issue lies in the centralized trust model that SSO depends on.

When every application trusts the same source of authentication, compromising that source can have far-reaching consequences.

# Why Disabling SSO Is Usually the Wrong Answer

A common reaction is to suggest removing SSO from critical applications.

At first glance, this seems logical. If a crown jewel system uses a separate authentication mechanism, compromise of the central identity provider may no longer grant immediate access.

In practice, this approach often creates more problems than it solves.

Separate authentication systems introduce:

* Additional credentials for users and administrators.
* Increased password reuse and password management challenges.
* Fragmented authentication logging.
* More complex access management processes.
* Greater operational overhead.

Organizations often replace one risk with several new ones while simultaneously reducing visibility across their environment.

# Protecting Crown Jewel Systems

Instead of removing SSO, organizations should focus on strengthening the authentication journey to critical systems.

The objective should be to ensure that compromise of a single identity does not automatically result in compromise of the most sensitive assets.

Several controls are particularly effective.

## Multifactor Authentication

Critical systems should require additional verification before access is granted.

Where possible, organizations should prioritize phishing resistant authentication methods such as FIDO2 security keys or passkeys instead of relying solely on traditional MFA methods.

## Conditional Access

Access decisions should consider contextual signals such as:

* Device compliance
* User risk
* Sign in risk
* Geographic location
* Network characteristics
* Application sensitivity

Authentication should be adaptive rather than static.

## Privileged Access Management

Administrative privileges should be tightly controlled and granted only when necessary.

Organizations should separate standard user accounts from privileged identities and adopt just in time access wherever possible.

## Continuous Validation

Authentication should not be treated as a one time event.

User behaviour, session activity and resource access patterns should continue to be evaluated throughout the session. Unexpected changes in behaviour should trigger additional verification or session termination.

# SSO and Zero Trust

The most effective organizations do not view SSO and Zero Trust as competing concepts.

In fact, SSO is often an essential component of a Zero Trust architecture.

Zero Trust assumes that no identity, device or session should be trusted implicitly. Every access request must be continuously validated using available context and risk signals.

Within this model, SSO provides centralized identity management, while Zero Trust adds the controls required to prevent that centralization from becoming a single point of failure.

# Conclusion

SSO delivers significant operational and security benefits, but it should never be viewed as a standalone security control.

By centralizing authentication, SSO also centralizes trust. When that trust is compromised, attackers may gain access to a broad range of connected systems, including an organization's most critical assets.

The solution is not to abandon SSO. The solution is to strengthen it.

Organizations that combine SSO with strong multifactor authentication, conditional access policies, privileged access management and Zero Trust principles can retain the usability benefits of centralized identity management while significantly reducing the impact of identity compromise.

In modern environments, securing identities is no longer just part of cybersecurity. It is cybersecurity.
