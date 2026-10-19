---
status: Draft
---
# M1a — Online attendance

## Outcome
Management knows, on a dashboard, who is at each site and when they checked in and out, without calling anyone.

## In scope
- Check-in/check-out with **geofence validation on the server**.
- Radius configurable per site; blocking and alert outside the perimeter.
- Several technicians per site; changing site on the same day.
- Schedule model and late/forgotten clock-in alert.
- Dashboard states: green (at site), yellow (late), red (outside perimeter).

## Out of scope
Offline, selfie, fake GPS, SOS/pings, weighing.

## Prerequisites
- **OQ-02** answered (schedules and definition of "late").
- GPS spike (1-2 sessions): real accuracy outdoors and indoors, relation to the 300 m radius.

## Stories
- [ ] Spike: GPS accuracy on a real device
- [ ] Schedule/shift model
- [ ] Check-in with server-side geofence validation
- [ ] Check-out (possibly at another site)
- [ ] Block outside the perimeter + alert to management
- [ ] Scheduled job: late/forgotten clock-in alert
- [ ] Dashboard (list and map) with states
- [ ] One-week pilot at one site

## Success criteria
During the pilot, management answers "who is at the site right now?" from the dashboard, and every check-in/out of the period is recorded.

## Definition of Done
Same as M0, plus geofence tests (inside, outside, on the boundary) and a completed pilot.

## Risks
- Technician acceptance (OQ-07).
- GPS accuracy vs. configured radius.
- Legal aspects of tracking (OQ-06): in this milestone the position is recorded only at clock-in/out.

## Estimate
~30-45 h (low confidence). Actual: _to fill._