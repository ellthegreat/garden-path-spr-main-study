# Garden Path SPR – Main Study

Independent repository for the conceptual replication/extension experiment.

## Current status

**Development scaffold only. Not ready for participant recruitment or data collection.**

The previous repository and its Cloudflare Worker are intentionally left untouched. This repository will host the new experiment once the stimuli and procedure have been checked.

## Planned task structure

- Immediate session: main sentence-reading task.
- Delayed session: main sentence-reading task plus a separate Transfer block.
- Each trial will separately record sentence reading time, comprehension-decision RT, response, and accuracy.
- Pilot records and main-study records will be stored separately in the new Airtable base.
- Participant identifiers must be coded; do not commit names, contact details, secrets, API tokens, or participant data to this repository.

## Important implementation gates

1. Verify and counterbalance the target and control stimulus lists.
2. Finalize Form A / Form B and the three-week delayed schedule.
3. Implement the experiment with jsPsych (not a custom word-by-word display).
4. Implement a separate, authenticated/secured data endpoint. Never expose Airtable credentials in browser code.
5. Test on desktop and mobile, and verify that records arrive in the correct Airtable base and table.
6. Run a pilot and confirm the actual session duration before recruitment.

## Files

- `index.html`: temporary development landing page.
- `stimuli/`: finalized stimulus lists will be added after item audit.
- `js/`: experiment code will be added after procedure specification.
