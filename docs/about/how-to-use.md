# About this document

This document is designed to help organisations **evaluate Microsoft Entra Verified ID and Face Check** in a structured and practical way.

It provides **scenario‑based guidance, evaluation prompts, and rollout considerations** to support scoping and running a proof‑of‑concept (POC), with a focus on **high‑assurance identity verification** rather than implementation detail.

This guidance is intended to accelerate understanding and decision‑making — not to prescribe a single architecture or deployment model.

---

# What problem this guidance helps you evaluate

Microsoft Entra Verified ID enables organisations to issue **privacy‑preserving, decentralised credentials** to employees and external workers.

**Face Check** strengthens this capability by:
- Verifying a **real human is present at the moment of access**
- Protecting against **impersonation, deepfakes, and synthetic identity fraud**
- Providing high assurance **without exposing or storing biometric data**

Together, these capabilities help organisations answer:

> **“Are we confident the right person is present right now when something high‑risk happens?”**

---

# How to use this document to run a POC

This document should be used as a **POC planning and validation guide**, not as a step‑by‑step deployment manual.

A recommended POC approach is:

1. **Start with high‑risk workflows**  
   Focus on scenarios where impersonation or fraud would have the highest impact (e.g. helpdesk recovery, privileged access).

2. **Select a small number of scenarios**  
   You do not need to test every scenario in this document. One or two are usually sufficient.

3. **Validate assurance, not just integration**  
   Measure success in terms of confidence, risk reduction, and operational fit — not feature coverage.

4. **Use outcomes to inform next steps**  
   The POC should help decide where Verified ID and Face Check should be expanded, integrated, or deferred.

!!! tip
    High‑risk, low‑volume scenarios typically deliver the fastest learning and clearest value in a POC.

---

# How to read the sections in this document

## Executive Summary
A high‑level overview of what **Verified ID and Face Check do**, and how they support Zero Trust and identity assurance strategies.

## Business Benefits
Summarises **risk reduction, security uplift, and user experience benefits**, with an emphasis on privacy‑respecting verification.

## Typical Scenarios Where Face Check Applies
A catalogue of **common patterns** where real‑time identity and presence verification adds value.  
These scenarios are illustrative — not mandatory.

## Use Case Scenarios (1–8)
Each scenario includes:
- A clear **goal**
- **Functional steps** to test
- **Expected outcomes**

These sections form the **core POC scope options**.

## One‑Page Process Flow
A simplified, end‑to‑end view of how Verified ID and Face Check fit into:
- Onboarding
- Access requests
- Risk events
- Account recovery

This is particularly useful for **architecture, security, and audit discussions**.

## Setup Process
A high‑level **configuration checklist** showing the typical sequence of setup steps.  
This is not a deployment runbook.

## Relative Priority (Suggested Rollout Order)
A **risk‑based sequencing model (P0–P3)** to help prioritise rollout based on impact and readiness.

---

# Important disclaimers

!!! warning "Guidance, not prescription"
    This document provides **general guidance and example scenarios only**.

    - It does not mandate specific architectures or workflows  
    - It does not replace formal solution design or security review  
    - Scenarios must be adapted to your organisation’s **risk model, regulatory obligations, and operating environment**

!!! note "Preview and roadmap considerations"
    Some integration patterns — particularly **risk‑based or Conditional Access‑driven Face Check step‑up** — may be in preview, under development, or subject to change.

    All POC assumptions should be validated against **current Microsoft documentation and release status**.

