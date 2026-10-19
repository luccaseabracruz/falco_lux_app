---
status: Draft
---
# Open Questions, Assumptions and Hypotheses

Types: `Unknown` · `Assumption` · `Hypothesis` · `Open Question`
Status: `Open` · `Answered` · `Dropped`

## Blocking questions

| ID | Type | Question | Why it matters | Blocks | Status |
|---|---|---|---|---|---|
| OQ-01 | Open Question | Are birds assigned to a **site** or to **specific technicians**? The client's answers say "birds of their site"; the specification says "assigned to specific technicians". | Defines the data model and RBAC. | Data model (M0), M2a | Open |
| OQ-02 | Unknown | Who defines schedules/shifts? What counts as "late"? | Without an expected start time there is no late alert. | M1a | Open |
| OQ-05 | Open Question | Is fake-GPS blocking really required? Is there evidence of fraud? | May force a native app (see ADR-001). | ADR-001, M1b | Open |
| OQ-06 | Open Question | Daily selfie, GPS and pings: what is the legal basis, and what do labor law and GDPR allow in PT and ES? | Legal risk. Confirm with a lawyer/DPO. | Selfie (M1b), pings (M1c) | Open |

## Other questions

| ID | Type | Question | Status |
|---|---|---|---|
| OQ-03 | Unknown | Scale: how many sites, technicians and birds? | Open |
| OQ-04 | Unknown | Network coverage at real sites (and dead zones)? Determines what SOS can promise. | Open |
| OQ-07 | Open Question | Were technicians consulted? Do they accept selfie, GPS and pings? | Open |
| OQ-08 | Open Question | Does the "real-time" map show only the position at clock-in/pings, or continuous location? | Open |
| OQ-09 | Open Question | CITES: are expiry alerts needed? Who sees the documents (admin only or also technicians)? | Open |
| OQ-10 | Open Question | Is billing linked to attendance or reports? (Field left "[to fill]" in the client's answers.) | Open |
| OQ-11 | Unknown | Weather and tide data sources for PT and ES, and how to get them after sync? | Open |
| OQ-12 | Open Question | Is weight prediction a rule (from the falconer) or a statistical model? How is it validated? | Open |
| OQ-13 | Open Question | Measurable success criteria and current baseline (today there are no records). | Open |
| OQ-14 | Unknown | Technicians' devices: Android/iOS, personal or company-owned, device management? | Open |
| OQ-15 | Open Question | Is the Spanish UI needed in the MVP? | Open |

## Assumptions
| ID | Assumption | How to validate |
|---|---|---|
| A-01 | Every technician has a smartphone with GPS and a front camera. | OQ-14 |
| A-02 | Location fraud is a real risk. | OQ-05 |
| A-03 | A pilot at one site with 1-2 technicians is possible. | Ask the client |

## Hypotheses
| ID | Hypothesis | Measure |
|---|---|---|
| H-01 | Real-time visibility reduces lateness and absences. | Record lateness before/after the pilot |
| H-02 | Next-day weight prediction is reliable enough to help the falconer. | Compare prediction and actual weight during the pilot |