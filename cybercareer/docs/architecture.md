# Architecture

## Logical components

1. **Configuration** — local search preferences and candidate-approved facts.
2. **Discovery** — searches permitted job sources and employer career pages.
3. **Normalization** — converts results into a consistent opportunity record.
4. **Deduplication** — avoids repeating the same requisition.
5. **Fit analysis** — maps job requirements to confirmed candidate evidence.
6. **Preparation** — drafts tailored resumes and application answers.
7. **Reporting** — produces a daily summary and updates a local tracker.

## Suggested operating model

Use an orchestrator or scheduled task to run discovery and reporting. Keep credentials in a secret manager or environment variables, not in source files. Store candidate resumes and generated application materials in a private local directory.

## Human-in-the-loop boundary

Research and drafting can be automated. Final review, attestations, outbound messages, and application submission remain under candidate control.
