# Cost Comparison — Consumer Cloud vs Governed Stack

This example compares **realistic storage costs** over time for individuals,
creators, and small organizations using common cloud-first approaches
versus an edge-anchored, governed data stack.

Figures are intentionally conservative and region-agnostic.
Actual costs vary, but **patterns remain consistent**.

---

## Scenario Assumptions

- Mixed personal + business data
- Photos, videos, documents, backups
- Moderate media growth (video included)
- Multiple devices (phone + laptop)
- Desire for remote access and backups
- No enterprise discounts assumed

Data footprint (approximate):
- Year 1: 2–4 TB
- Year 5: 8–12 TB (media-heavy users reach this quickly)

---

## Option A — Consumer Cloud Only

Typical setup:
- Primary cloud storage (Google Drive / iCloud / Dropbox)
- Automatic sync across devices
- Cloud-native photo libraries
- Platform-managed backups

### Costs
- Monthly: $20–$30
- Annual: $240–$360

### 1-Year Total
- $240–$360

### 5-Year Total
- $1,200–$1,800  
*(often higher due to tier jumps)*

### Hidden Costs
- Sync inflation and duplicates
- Platform lock-in
- Migration time if leaving
- Limited visibility into what drives usage

---

## Option B — Hybrid (Edge + Minimal Cloud)

Typical setup:
- Local edge node (existing computer or small server)
- Selective cloud sync for active folders
- Cloud used only for access and sharing
- Local backups for redundancy

### Costs
- One-time hardware (if needed): $400–$800
- Monthly cloud: $5–$10
- Annual cloud: $60–$120

### 1-Year Total
- $460–$920

### 5-Year Total
- $700–$1,400  
*(hardware amortized, cloud remains flat)*

### Benefits
- Significant cost flattening
- Clear authority boundaries
- Easier exits
- Reduced platform dependence

---

## Option C — Governed Stack (Edge + Archive)

Typical setup:
- Dedicated or software-based edge node
- No full cloud mirror
- Archive-tier storage for cold data
- Scheduled backups, not continuous sync

### Costs
- One-time hardware: $600–$1,200
- Archive storage: $1–$4 / TB / month
- Annual archive (8–12 TB): $100–$400

### 1-Year Total
- $700–$1,400

### 5-Year Total
- $1,100–$2,200  
*(storage grows, but costs scale predictably)*

### Benefits
- Lowest long-term risk
- Clear exit readiness
- Stable structure over time
- Suitable for automation and agents

---

## Cost Is Not the Only Variable

While raw dollar amounts matter, the governed stack optimizes for:

- **Predictability**  
  Costs scale linearly, not exponentially.

- **Control**  
  No forced tier jumps or ecosystem pressure.

- **Exit power**  
  Migration does not require re-architecture.

- **Time savings**  
  Less cleanup, fewer emergency migrations.

---

## Summary Table

| Approach | 1-Year | 5-Year | Lock-In Risk | Exit Cost |
|--------|--------|--------|-------------|-----------|
| Cloud Only | $240–$360 | $1,200–$1,800+ | High | High |
| Hybrid | $460–$920 | $700–$1,400 | Medium | Low |
| Governed Stack | $700–$1,400 | $1,100–$2,200 | Low | Low |

---

## Why This Matters

Cloud-only setups appear cheaper early.
Governed systems become cheaper **over time**—especially when accounting for:
- growth
- migration
- automation
- long-term continuity

Cost discipline follows **authority discipline**.

---

Next: `examples/exit-drill-walkthrough.md`
