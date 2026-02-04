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
