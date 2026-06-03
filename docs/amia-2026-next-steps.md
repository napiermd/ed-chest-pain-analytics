# AMIA 2026 Podium Abstract and Post-MCiM Plan

Updated: 2026-06-03

## Current Status

AMIA podium abstract `#15227` was accepted:

`Training Clinical Decision Support from Ambient Conversation: Separating Patient Signal from Documentation Bias in Emergency Chest Pain`

The current revision is no longer just an abstract cleanup. It is the project control point for the post-MCiM research plan.

## Faculty Feedback to Incorporate

### Mark Musen

- The revised abstract is directionally strong.
- The new framing works.
- Main issue: the writing is too telegraphic.
- Action: confirm AMIA final program length. If there is room, expand the Discussion and make the phase 1 results easier to read.

### Ashley Griffin

- Clarify whether the 360-case set is representative of ED ACS presentations.
- Define ECE or remove it from the table.
- Explain why there were 8 reviews for 5 cases.
- Define the Section 5G ratings in plain language.
- Explain where the phase 2 endpoints came from.
- Add how phase 1 findings change the architecture, especially around omitted differentials and safety misses.

## Response Position

Send one reply-all to Mark and Ashley, not separate emails. They are already in the same project thread, and the next-step plan needs both methodological and writing feedback in one place.

Draft response is saved in the OpenClaw workspace:

`drafts/ashley-musen-amia-reply-2026-06-03.txt`

## Revision Decisions

### Cohort Representativeness

Do not overclaim the 360-case set. It is an enriched development/evaluation set built around chest pain and documentation bias patterns, not a clean ED ACS denominator.

Phase 2 should use a cleaner consecutive or stratified ED chest-pain cohort, with deliberate representation of:

- Lower-risk chest pain presentations
- Atypical ACS presentations
- Patients at higher risk of documentation or diagnostic bias
- Non-ACS dangerous mimics, including PE, aortic dissection, and pleural effusion/pneumonia patterns

### Calibration

ECE means expected calibration error. It should be defined in the abstract/table if retained.

If AMIA space is tight, remove ECE from the abstract and keep it in the follow-on paper.

### Phase 1 Review Count

The `8 reviews` language is confusing because there were 5 cases. Rewrite as:

- 5 pilot cases
- 2 initial reviewers
- 8 completed case-review instruments due to partial overlap/completion state

Do not imply 8 unique cases.

### Section 5G

Replace internal form language with clinical language:

`dangerous-miss / safety-override rating`

The reader should not need to know the review instrument structure to understand the result.

### Architecture Change From Phase 1

Phase 1 suggests feature extraction is mostly stable, but risk synthesis is overconfident and can omit dangerous alternatives.

Planned architecture change:

1. Extract chest pain features.
2. Generate differential diagnosis safety layer before final ACS risk synthesis.
3. Force explicit check for time-sensitive mimics: PE, aortic dissection, effusion/pneumonia, pneumothorax when relevant.
4. Preserve ACS risk output, but add a safety-override channel when non-ACS danger patterns appear.
5. Compare model risk synthesis against blinded EM physician reviewer judgments.

## Phase 2 Endpoint Frame

Phase 2 endpoints should be tied to the safety question:

Does the system preserve high NPV for 30-day MACE while improving disposition concordance and avoiding unsafe misses?

Candidate endpoints:

- Disposition concordance with physician reviewers
- Safety-override appropriateness
- Dangerous-miss detection for non-ACS mimics
- Time-to-disposition
- 30-day MACE NPV at the AHA safety floor

Do not frame these as deployment-ready clinical performance claims. Frame them as phase 2 evaluation targets.

## Near-Term Action Plan

### This Week

- Finish required MCiM coursework.
- Reply to Mark and Ashley with the reset email.
- Confirm AMIA final program abstract length and formatting constraints.
- Locate the current revised abstract and reviewer-feedback packet.
- Create a single project folder for:
  - AMIA abstract
  - Reviewer feedback
  - Faculty feedback
  - Phase 1 pilot data summary
  - Phase 2 plan

### Next Week

- Hold 20-30 minute Zoom with Mark and Ashley if they agree.
- Send one-page next-step outline before the call.
- Revise the AMIA abstract based on:
  - Less telegraphic Discussion
  - Defined ECE or removed ECE
  - Clear pilot-review count
  - Plain-language Section 5G description
  - Representative-cohort caveat
  - Architecture change from phase 1 safety feedback

### Post-MCiM

- Convert this from abstract mode to paper mode.
- Decide between:
  - JAMIA-style methods/evaluation paper
  - Narrow AMIA follow-on abstract/presentation
  - Internal Sayvant validation artifact first, then external manuscript
- Build phase 2 cohort plan.
- Define reviewer protocol and adjudication plan.
- Lock source-of-truth documents in this repo.

## Open Questions

- What is AMIA's final program length limit for the accepted podium abstract?
- Was the revised abstract already resubmitted after Ashley and Mark's feedback?
- Are the final phase 1 reviewer numbers updated after Nick's completion?
- Where is the current abstract file stored?
- Should phase 2 prioritize academic publication or product validation first?

