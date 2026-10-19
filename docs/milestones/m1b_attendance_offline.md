---
status: Draft
---
# M1b — Offline and anti-fraud

## Outcome
A technician works a whole day without network, syncs afterwards, and no records are lost or duplicated.

## In scope
- Local record queue and sync with retries.
- Client-generated IDs (idempotency).
- Device time **and** server receipt time; flag discrepancies.
- Sync status visible to the user.
- Selfie at clock-in (front camera, no gallery), private storage and automatic purge after 30 days.
- Fake-GPS detection, according to ADR-001.

## Out of scope
SOS/pings (M1c), weighing.

## Prerequisites
- ADR-001 decided (PWA / native / hybrid).
- OQ-04 (network coverage), OQ-05 (fake GPS needed?) and OQ-06 (selfie: legal basis).
- ADR-003: sync design (direction: append-only records with client-side IDs).

## Stories
- [ ] ADR-003 and sync spike
- [ ] Local storage and upload queue
- [ ] Idempotent sync with retries
- [ ] Sync status indicator
- [ ] Record device vs. server time + flag discrepancies
- [ ] Selfie: capture, private storage
- [ ] Job to purge selfies older than 30 days
- [ ] Fake-GPS detection (if kept)

## Mandatory tests
Airplane mode; network lost mid-sync; duplicate uploads; device clock changed; app closed with pending records.

## Success criteria
A full day offline, synced afterwards, with no duplicates or losses; clock discrepancies visible to the admin.

## Definition of Done
Same as M0, plus the tests above automated where possible.

## Risks
Biggest technical risk of the project. If it blows up, split selfie and fake GPS into an M1b2.

## Estimate
~40-70 h (low confidence). Actual: _to fill._