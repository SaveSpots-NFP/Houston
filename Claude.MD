# Houston Research Project Guide

This repository is for a Houston/Harris County research paper modeled on the SaveSpots Dallas paper and the 2026 cohort deliverables guide. The goal is not to copy Dallas findings or methods wholesale, but to build the strongest possible Houston-specific analysis using the best available data and a transparent, reproducible workflow.

## Core mission

Answer three questions:

1. Where is the burden?
2. Where is the service gap?
3. Where should supply go?

The final product should read like a defensible public-health research paper that connects burden, access, and practical placement recommendations.

## Geographic scope

- Default geographic scope is Harris County unless the project plan or data access says otherwise.
- Use only geographies justified by underlying data quality.
- Never allocate coarse data to finer geographies than the data support.
- If a metric is only available at a larger geography, report it at that geography and do not create false precision.

## Data and methods rules

- Every quantity must be classified as one of: measured, modeled, or published.
- Do not present quantities without a clear provenance label and uncertainty framing.
- At least one primary quantity used in the main analysis must be measured, not inferred or published only.
- Composite weights must be fully disclosed.
- Include at least two sensitivity variants for composite weighting or ranking decisions.
- Acknowledge data gaps honestly rather than smoothing them away.
- Do not use individual-level records, addresses, overdose/decedent coordinates, or precise point locations in published artifacts or repository files.
- Keep all outputs privacy-preserving and consistent with a public-facing research workflow.

## Research design constraints

- Use Dallas as a methodological benchmark, not as a template or a source of Houston findings.
- Prioritize Houston-relevant data and policy context.
- Build the analysis around the strongest available evidence in the local setting.
- Distinguish between service access, need, and supply allocation; they are not interchangeable.
- Interpret results in terms of risk, burden, and shortage, not just map density.

## Required workflow

Use this order of operations:

1. Data inventory and analysis plan
2. Geography and population baseline
3. Supply inventory
4. Access measurement
5. Prioritization
6. Placement recommendation
7. Figures and maps
8. Validation and sensitivity analyses
9. Manuscript
10. Preprint or public-facing writeup
11. Abstract
12. Poster

Do not begin causal or placement modeling before the data inventory and analysis plan is documented and reviewed.

## Repository and execution expectations

- Keep the repository reproducible with one-command outputs whenever feasible.
- Document dependencies and clear run steps.
- Separate raw inputs, cleaned data, analysis scripts, and final figures.
- Avoid one-off notebooks that cannot be rerun easily.
- Prefer scripts or pipeline steps that can be rerun from a documented command.

## Reporting and interpretation standards

- Explain when a result is measured, modeled, or published.
- Distinguish between estimated need and observed utilization.
- Discuss both burden and access constraints.
- Include sensitivity analyses showing how weighting assumptions change results.
- Present uncertainty and caveats explicitly.
- Do not claim precision that the data do not support.

## Outputs expected for the project

The project should ultimately support:

- A full research manuscript
- A preprint or public-facing summary
- A concise abstract
- One or more figures/maps showing burden, access, and placement recommendations
- A clear methods section describing data sources, data quality, provenance, and sensitivity checks

## Privacy and ethics

- No individual-level data in the repo.
- No addresses, exact locations, or overdose/decedent coordinates in code, figures, or notes.
- No publication of personally identifying or sensitive geocoded information.
- Aggregate to appropriate geographies and report only summarized, privacy-safe results.

## Working principles for future iterations

When proposing code, analysis, or narrative, ensure the work:

- is tractable for Houston/Harris County,
- uses transparent and defensible methods,
- preserves privacy,
- clearly states what is measured versus modeled versus published,
- explains weighting choices and sensitivity analyses,
- and is aligned to the project’s burden-gap-placement research questions.

## Recommended default approach

The project should be framed as a local burden and access analysis with a public-health planning lens. The final product should emphasize:

- service need and burden at appropriate geographies,
- observed and modeled gaps in availability or access,
- a transparent supply-allocation recommendation,
- and a documented set of assumptions and sensitivity checks.

## Data availability finding: Environment B

The current public-source audit supports treating Houston/Harris County as Environment B unless a future HCIFS or HCPH request produces a de-identified case-level extract. Harris County Institute of Forensic Sciences (HCIFS) does not expose a public bulk overdose-death or toxicology dataset. Its public Case Status tool provides basic information for Medical Examiner cases dating back 24 months, while completed autopsy reports are requested individually by email or mail. HCIFS directs Texas Public Information Act and data requests in writing to its Public Information Officer at IFSPIO@ifs.hctx.net.

Harris County Public Health's Substance Use Data Hub is the strongest local public alternative. It publishes aggregate fatal-overdose trends and states that the underlying fatal data come from HCIFS. Its disclaimer identifies important limitations: deaths are for people pronounced dead in Harris County, reporting may be delayed by pending toxicology, and substance fields are free text subject to spelling differences, misclassification, duplication, and naming variation. Texas DSHS's Texas Health Data dashboard is another public aggregate source based on death certificates, with county-level measures, substance categories, and suppression rules.

Until a data request proves otherwise, do not claim that HCIFS case-level data are publicly available. Design the main analysis around aggregate, privacy-preserving data. Do not request or store names, addresses, exact coordinates, case numbers, or individual-level records. The full source-by-source audit, including access routes and documented absences, is in [data-availability-audit.md](data-availability-audit.md).

## Section 4 deliverable standard: City Profile and Harm Reduction Landscape

Section 4 is the first substantive city-specific deliverable and becomes manuscript Sections 3 and 5. Target length is 1,500-2,500 words. It is pipeline-independent and must establish whether Houston has a locally grounded overdose and harm-reduction story before infrastructure or placement modeling begins.

The profile is not a census summary. Every statistic must connect to overdose risk, naloxone access, treatment access, infectious disease, criminal-justice barriers, or policy. Required content is: overdose burden with at least a three-year mortality trend, percent change, fentanyl contribution, polysubstance share, and non-fatal volume where published; demographics with an explicit harm-reduction consequence; treatment capacity and retention plus HIV/hepatitis C burden as an injection-drug-use proxy; the criminal-justice intersection; existing infrastructure assessed by organization, function, and geography; populations current outreach misses and why; and one sentence naming the single most consequential structural gap.

Every paragraph should follow the substitution-test sequence: state a local condition, provide supporting evidence with source and time window, interpret what it means, and draw the implication for harm-reduction access or delivery. Generic national claims without Houston evidence fail this standard. When a required quantity is unavailable, state that absence and its consequence rather than substituting an incompatible geography or definition.

This document is the working source of truth for the repo and should be updated as methods, geography, or deliverables evolve.


