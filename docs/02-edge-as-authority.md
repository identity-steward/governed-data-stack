# 02 — Edge as Authority

In distributed systems, *authority is not abstract*.  
It lives where decisions are enforced.

For most people today, authority quietly migrated from the individual
to platforms that control execution, keys, and policy enforcement.

This document explains why **the edge**—not the cloud—is the only place
where durable authority can live.

---

## What “Edge” Means Here

The edge is not defined by hardware size or compute power.

It is defined by **control**.

An edge node is the environment where:
- encryption keys are held
- policies are evaluated
- logs are written
- revocation is enforced
- execution is authorized

This may be:
- a personal computer
- a small server
- a dedicated device
- a secured workstation

What matters is not scale, but custody.

---

## Why the Cloud Cannot Be the Authority

Cloud platforms are excellent at:
- availability
- redundancy
- scaling
- managed execution

They are not designed to be:
- neutral arbiters of intent
- custodians of user sovereignty
- revocation-first systems

Cloud services must retain the ability to:
- suspend accounts
- alter terms
- change APIs
- reprice access
- prioritize their own incentives

This is not malicious.
It is structural.

Authority placed in the cloud is authority placed **elsewhere**.

---

## The Edge as Root of Trust

When authority is anchored at the edge:

- The **canonical state** is local
- Cloud systems become optional
- Policies are evaluated before action
- Revocation is immediate and auditable
- Automation acts under user-defined scope

The cloud becomes a subcontractor.
The edge remains the principal.

---

## Edge Authority in Automated Systems

As systems become more automated and agent-driven,
the distinction between *access* and *action* disappears.

Agents do not ask politely.
They execute.

If agents are authorized only by cloud dashboards,
then their behavior follows platform terms.

If agents are authorized at the edge,
their behavior follows **your** terms.

Edge authority is therefore a prerequisite for:
- delegated agents
- constrained automation
- trustworthy audit trails
- enforceable consent signaling

---

## What the Edge Actually Does in This Stack

Within this architecture, the edge is responsible for:

- Maintaining the canonical data layout
- Holding encryption keys
- Storing policy definitions
- Logging agent actions
- Enforcing revocation
- Signing outbound requests

The edge does **not** need to:
- host public services
- scale globally
- replace the cloud

It needs to be **authoritative**, not large.

---

## Failure Modes Without an Edge Authority

When no authoritative edge exists:

- Revocation becomes symbolic
- Consent is implied, not enforced
- Logs are platform-controlled
- Disputes are retrospective
- Exit is expensive and risky

These are not edge cases.
They are the default outcomes.

---

## Edge First, Cloud Second

This stack adopts a simple hierarchy:

1. **Edge:** authority, keys, policy, logs  
2. **Cloud:** convenience, access, redundancy  
3. **Archive:** resilience and long-term storage  

This order is non-negotiable.
Reversing it reverses control.

---

Next: `03-exit-readiness.md`
