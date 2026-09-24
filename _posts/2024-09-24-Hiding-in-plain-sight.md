---
layout: default
title: "Hiding in Plain Sight: Command and Control via Google Search"
date: 2024-09-24
---

> **Responsible use:** This research was conducted to improve awareness of covert Command and Control channels. The concept should only be tested in environments where explicit authorization has been provided.

# Introduction

Modern Network Detection and Response solutions increasingly use anomaly detection to identify suspicious network traffic. This presents a challenge for Red Teams: how can Command and Control traffic remain inconspicuous when unusual destinations and communication patterns may trigger alerts?

One possible answer is to hide the communication inside traffic that users already generate every day.

This research explores whether Google search history and search suggestions can function as a covert communication channel.

# The concept

Google synchronizes search activity between devices signed in to the same account. A search performed on one device may therefore become visible in the search history or suggestion list on another device.

That synchronization creates a basic communication mechanism:

1. The operator submits a search containing a command.
2. A controlled endpoint retrieves the latest search entry.
3. The endpoint executes the command.
4. Its output is submitted as a new search.
5. The operator retrieves the result through the synchronized search history.

In the proof of concept, the operator submitted the command `hostname`. The controlled endpoint retrieved and executed it, after which the hostname was returned through another search entry.

# Under the hood

During the research, we analyzed the network traffic associated with submitting searches and retrieving search suggestions.

The relevant web requests were reduced to their essential components and converted into Bash commands using `curl`. This demonstrated that both sides of the communication channel could be automated:

* Submitting a command through a Google search
* Retrieving that command from the suggestion data
* Executing the command on a controlled system
* Returning the output through another search
* Retrieving the result from the operator system

No dedicated Command and Control domain was required. Communication blended into traffic associated with a widely used internet service.

# Why this matters

Traditional Command and Control infrastructure often communicates with attacker controlled domains or redirectors. These destinations may be detected through reputation checks, network indicators or deviations from normal user behaviour.

A covert channel that uses a commonly accessed service changes that detection problem. Blocking the service outright may not be practical, while the surrounding traffic can initially appear legitimate.

This does not mean the channel is invisible. Defenders can still investigate unusual automation, unexpected authentication artefacts, nonstandard search patterns and endpoint processes interacting with web services.

# Limitations and next steps

The proof of concept establishes a working communication loop, but several challenges remain:

* Encoding and encrypting commands and output
* Transferring larger messages reliably
* Handling modified input caused by autocorrect
* Maintaining the correct order of commands and responses
* Distinguishing communication between multiple endpoints
* Integrating the channel with an established Command and Control framework
* Evaluating its detectability against modern NDR solutions

# Conclusion

This research demonstrates how a familiar feature can potentially be repurposed as a covert communication channel.

For Red Teams, the concept highlights the value of studying trusted services from an attacker perspective. For defenders, it demonstrates why monitoring cannot rely exclusively on domain reputation or destination based controls.

Sometimes suspicious traffic does not look suspicious at all. It simply looks like someone using Google.
`
