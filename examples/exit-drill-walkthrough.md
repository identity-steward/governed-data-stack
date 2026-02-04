# Exit Drill Walkthrough — Practicing Exit Readiness

Exit readiness is not theoretical.
It is a practiced capability.

This walkthrough documents a **lightweight exit drill** that can be run
quarterly or semi-annually to ensure the system remains survivable
without any single cloud provider.

---

## Purpose of the Drill

The goal is not to abandon the cloud.
The goal is to confirm that **you can**.

An exit drill verifies that:
- canonical data is intact
- structure survives export
- dependencies are visible
- recovery paths are understood
- authority is not silently upstream

---

## Scope (What This Drill Covers)

This drill tests:
- cloud export
- local structure integrity
- archive recovery
- minimal reconfiguration

It does **not** require:
- full provider shutdown
- service cancellation
- downtime

---

## Pre-Drill Conditions

Before starting, confirm:
- edge node is current and reachable
- archive backups are up to date
- no active migrations are underway
- documentation reflects current structure

Estimated time: **30–60 minutes**

---

## Step 1 — Identify a Test Subset

Choose a **non-critical subset** of data, such as:
- one completed project
- one media folder
- a small administrative set

Document:
- source paths
- total size
- expected contents

This subset should be representative but low-risk.

---

## Step 2 — Export from Cloud

Using the provider’s standard tools:
- export the chosen subset
- preserve original filenames and timestamps
- avoid proprietary formats if export options exist

Do **not** clean or reorganize yet.

The goal is to observe what the platform gives you.

---

## Step 3 — Rehydrate into Edge Structure

Place the exported data into the canonical edge layout:

/Vault/02-Projects/<test-project>
or
/Vault/03-Media/<test-set>


Verify:
- directory depth
- file counts
- basic integrity (open a few files)

Note any friction or surprises.

---

## Step 4 — Restore from Archive (Optional but Recommended)

Select one archived snapshot related to the same subset.

Restore it to a **temporary location** and compare:
- file presence
- checksums (if available)
- timestamps

This confirms that archive backups are viable,
not just present.

---

## Step 5 — Simulate Provider Loss

Without disconnecting accounts:
- stop syncing the tested subset
- treat the cloud copy as unavailable

Ask:
- can work continue?
- is anything missing?
- are any tools hard-dependent on the platform?

If the answer is “yes,” document it.

---

## Step 6 — Document Findings

Create a short note covering:
- what worked
- what was awkward
- what broke
- what assumptions were revealed

This documentation is part of governance.

Exit readiness improves through observation, not blame.

---

## Step 7 — Update the Stack (If Needed)

Based on findings:
- adjust sync scope
- revise directory structure
- clarify documentation
- change tool usage
- move data between tiers

Small changes compound into resilience.

---

## Success Criteria

The drill is successful if:
- data survives export intact
- structure remains coherent
- archive restores cleanly
- continued operation is possible
- no permissions were required

If success depends on goodwill or exceptions,
authority has drifted.

---

## Why This Matters

Exit drills:
- surface hidden dependencies
- prevent silent lock-in
- reduce migration panic
- normalize departure as healthy
- make delegation safer

A system that cannot be exited
cannot be fully trusted.

---

## Frequency Recommendation

- Individuals: **1–2× per year**
- Media-heavy workflows: **quarterly**
- Automated / agentic systems: **before major changes**

Exit readiness is not paranoia.
It is operational hygiene.
