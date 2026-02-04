# 00 — Why Local-First

Local-first is not a preference.  
It is a statement about **authority**.

Modern cloud platforms optimize for convenience and retention. This is useful—
until the platform becomes the default owner of your workflows, your data layout,
your identity surface, and your exit options.

A local-first posture restores a simple principle:

> If your data is not under your control, it is not fully yours to govern.

This does not mean “no cloud.”
It means the cloud is a tool, not a master.

---

## The Core Problem: Authority Drift

In practice, cloud dependency creates a gradual transfer of authority:

- **Keys drift** (platform-controlled encryption and recovery paths)
- **Structure drifts** (platform-specific formats, syncing, and metadata)
- **Cost drifts** (storage inflation, duplicates, ecosystem pressure)
- **Identity drifts** (accounts become access gates, not representations)
- **Exit drifts** (leaving becomes painful enough that you stop trying)

Local-first architectures counter that drift by making the edge the root of trust.

---

## Local-First ≠ Offline

Local-first means:

- the **canonical copy** is controlled by you
- encryption keys are **yours**
- policies are defined by you
- cloud providers can be swapped without rebuilding your life

Cloud services can still be used for:
- remote access
- collaboration
- redundancy
- archive storage

…but they operate as subcontractors to your authority.

---

## Why This Matters in Automated / AI Environments

Automation changes the stakes.

As systems become more agentic, “access” becomes “action”:
- systems read
- systems summarize
- systems classify
- systems train
- systems redistribute

If authority lives only in cloud dashboards, then action follows platform terms.
If authority is anchored locally, then action follows **your** terms.

Local-first is therefore a prerequisite for:
- delegated agents with revocation
- audit trails you can trust
- meaningful consent signaling
- long-term continuity

---

## Practical Outcomes

A local-first posture enables:

- **Exit readiness**
  Replace any cloud provider without losing structure.

- **Cost control**
  Prevent sync inflation and redundant storage.

- **Provenance continuity**
  Maintain attribution and integrity across reuse.

- **Privacy by default**
  Keys and policies remain in your custody.

- **Evolvability**
  Your data remains interrogable and adaptable over time.

---

## What This Repository Builds On

This stack uses a tiered approach:

- **Edge (authoritative):** keys, policy, canonical storage, logs  
- **Cloud (convenience):** access, sharing, optional redundancy  
- **Archive (resilience):** low-cost storage and long-term retention  

Local-first is the foundation that makes the rest of the system coherent.

---

Next: `01-cloud-cost-creep.md`
