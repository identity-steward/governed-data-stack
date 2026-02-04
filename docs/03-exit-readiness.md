# 03 — Exit Readiness

Exit is not a failure state.
It is a design requirement.

Any system that cannot be exited safely, predictably, and without coercion
is not a system you control—it is a system you endure.

This document explains why **exit readiness** must be designed in from the beginning,
and how it changes every downstream decision.

---

## Exit Is the Measure of Authority

You can tell who holds authority in a system by answering one question:

> “Who pays the highest cost when leaving?”

If the answer is “the user,” authority has already drifted.

Exit readiness reverses this by ensuring that:
- leaving is possible
- leaving is documented
- leaving is survivable
- leaving does not require permission

---

## Why Exit Is Rarely Designed First

Most systems optimize for:
- onboarding
- retention
- growth
- convenience

Exit is treated as:
- a support issue
- an edge case
- a future concern

This leads to architectures where:
- data structures are opaque
- dependencies are implicit
- workflows are entangled
- users stay because leaving is risky

Exit readiness corrects this bias.

---

## What Exit Readiness Actually Requires

Exit readiness is not just “export your data.”

It requires:

- **Format portability**  
  Data stored in non-proprietary, documented formats.

- **Structural continuity**  
  Directory layouts and metadata that survive migration.

- **Policy independence**  
  Rules and permissions that are not platform-bound.

- **Key custody**  
  Encryption keys that move with you.

- **Operational rehearsal**  
  Practiced exits, not theoretical ones.

---

## Exit Changes How You Choose Tools

When exit is a primary constraint:
- convenience features are evaluated differently
- vendor promises are discounted
- lock-in risks become visible early

Tools are selected not for how easy they are to enter,
but for how cleanly they can be replaced.

This leads to calmer decisions and fewer regrets.

---

## Exit in Automated and Agentic Systems

Automation increases the cost of poor exit design.

When agents are involved:
- decisions happen continuously
- actions compound
- mistakes propagate quickly

If exit is unclear:
- revocation becomes symbolic
- consent becomes retrospective
- disputes become legal rather than operational

Exit readiness allows:
- immediate revocation
- clean shutdown of automation
- safe reconfiguration
- continuity without escalation

---

## Exit as a Form of Repair

Exit is not abandonment.
It is often the **first step in restoration**.

Exit enables:
- renegotiation
- rebalancing
- correction of past assumptions
- recovery from asymmetrical relationships

In this sense, exit readiness is reparative.
It restores symmetry between participant and system.

---

## How This Stack Treats Exit

This architecture treats exit as:

- a documented procedure
- a tested capability
- a non-punitive action
- a signal of health, not conflict

Every component in the stack must be:
- replaceable
- understandable
- survivable without it

If a component fails this test, it does not belong.

---

## Where This Leads Next

With authority anchored at the edge and exit designed in,
the remaining questions are operational:

- How is this applied in practice?
- What does a real deployment look like?
- How can this be delegated responsibly?

Those questions are addressed in `/examples` and `/services`.

