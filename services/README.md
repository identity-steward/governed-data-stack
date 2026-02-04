# Services — Delegated Operation

This directory describes **optional delegation paths** for operating
the Governed Data Stack.

Delegation is not required.
The documentation in this repository is sufficient for self-operation.

Services exist for those who align with the architecture
but do not wish to maintain it themselves.

---

## Delegation vs Dependency

Delegation means:
- scope is defined
- authority remains with the client
- actions are logged
- revocation is possible

Dependency means:
- authority is transferred
- systems become opaque
- exit becomes costly
- decisions are upstream

Services offered here are structured as **delegation**, not dependency.

---

## When Delegation Makes Sense

Delegation is appropriate when:

- time is more constrained than money
- operational discipline is desired but not enjoyable
- automation or agents are being introduced
- exit readiness must be maintained continuously
- the system is becoming business-critical

Delegation is *not* a requirement for using this stack.

---

## Service Categories

The services described in this directory fall into three categories:

### 1) Initial Architecture & Setup
For those who want:
- a clean, correct deployment
- authority anchored properly from the start
- minimal trial-and-error

This typically includes:
- data inventory and tiering
- edge authority configuration
- cloud scope reduction
- archive setup
- documentation handoff

---

### 2) Ongoing Stewardship
For those who want:
- continued oversight
- cost and dependency monitoring
- periodic exit drills
- policy and scope adjustments

Stewardship focuses on **preserving optionality over time**.

---

### 3) Delegated Authority (Agent-Operated)
For environments where:
- automation or agents act continuously
- scope must be enforced mechanically
- auditability matters
- revocation must be immediate

This model treats the system as a **governed environment**,
not a set-and-forget toolchain.

---

## What Services Do Not Do

These services do **not**:

- sell data
- claim ownership of client assets
- block exit
- impose proprietary tooling
- require long-term contracts

Any service that requires surrendering authority
is incompatible with this stack.

---

## How to Proceed

If you believe delegation is appropriate for your situation,
see `ENGAGE.md` for how to initiate a conversation.

Good-faith alignment is assumed.
