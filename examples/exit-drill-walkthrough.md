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

