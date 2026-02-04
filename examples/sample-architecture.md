# Sample Architecture — Edge-Anchored, Cloud-Optional

This example demonstrates a practical, vendor-agnostic deployment of the Governed Data Stack.

Goal:
- keep authority (keys, policy, canonical structure) at the edge
- use cloud only for convenience and scoped redundancy
- maintain exit readiness at all times

---

## Components

### 1) Sovereign Edge Node (Authoritative Tier)
Purpose:
- canonical data layout
- encryption key custody
- policy + consent signals
- audit logs of sync and agent actions

Typical implementations:
- personal workstation
- small home/office server
- dedicated mini PC
- NAS-class device

---

### 2) Client Devices
- phone (capture)
- laptop/desktop (work)
- optional tablet

These devices should not be the canonical store.
They are working surfaces.

---

### 3) Cloud Convenience Tier (Optional)
Purpose:
- remote access
- collaboration
- device-to-device sync assistance
- limited redundancy

Constraint:
- should be replaceable without restructuring.

---

### 4) Archive Tier (Cold Storage)
Purpose:
- low-cost retention
- long-term continuity
- disaster recovery

Archive should be:
- slow
- cheap
- durable
- periodically verified

---

## Data Tiers

### Hot (Active)
Examples:
- current projects
- working documents
- in-progress media edits

Location:
- edge node + working device
Cloud:
- optional

---

### Warm (Occasional)
Examples:
- completed projects still referenced
- administrative documents
- older media still used periodically

Location:
- edge node
Cloud:
- optional and scoped

---

### Cold (Archive)
Examples:
- historical media
- old backups
- rarely used materials

Location:
- archive tier
Cloud:
- minimal or none

---

## Directory Structure (Canonical)

The canonical structure lives on the edge node:

/Vault
/00-Identity
/01-Admin
/02-Projects
/03-Media
/04-Archive
/05-Exports
/06-Logs


Notes:
- keep a stable top-level structure
- avoid platform-native folders as the canonical root
- store exports in predictable locations

---

## Sync Rules (Authority-Preserving)

### Phone → Edge
- phone uploads photos/videos into `/Vault/03-Media/Incoming`
- edge node sorts and deduplicates

Rule:
- phone is a capture device, not the archive.

---

### Laptop → Edge
- laptop edits working files in `/Vault/02-Projects/...`
- edge node remains canonical
- laptop holds working copies only

Rule:
- if the laptop dies, the project survives.

---

### Edge → Cloud (Scoped)
- only specific folders are mirrored
- never mirror everything by default

Recommended approach:
- mirror `/Vault/02-Projects` selectively
- mirror `/Vault/01-Admin` if needed for mobile access
- do not mirror `/Vault/04-Archive`

Rule:
- cloud exists for convenience, not custody.

---

### Edge → Archive (Scheduled)
- archive receives snapshots, not continuous sync
- archive is immutable where possible

Rule:
- backups are not “sync.”
They are recovery points.

---

## Encryption & Keys (Minimal Model)

- client-side encryption where feasible
- keys are stored and managed at the edge
- cloud receives encrypted material when possible

If client-side encryption is not used:
- treat the cloud tier as untrusted
- limit scope and content

---

## Redundancy (3-2-1+)

Minimum target:
- 3 copies of important data
- 2 different media types
- 1 copy offsite

Example:
- primary: edge node storage
- secondary: local backup drive
- offsite: archive tier

Optional:
- add a second offsite copy for critical assets

---

## Exit Drill (What “Ready” Looks Like)

You are exit-ready when you can:
- export all cloud data without breaking structure
- rebuild from edge + archive without the cloud
- swap providers without changing canonical paths

A simple quarterly drill:
1. export a small cloud subset
2. verify directory structure survives
3. restore one project from archive
4. confirm checksums and integrity

---

## Why This Works

- authority remains local
- cloud remains optional
- cost creep is contained
- provenance and policy can be anchored
- automation can be delegated safely

Next: `examples/cost-comparison.md`
