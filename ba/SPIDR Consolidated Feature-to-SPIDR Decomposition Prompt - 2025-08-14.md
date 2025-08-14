title- SPIDR: Consolidated Feature-to-SPIDR Decomposition Prompt Description- A single prompt to convert any feature into a complete SPIDR backlog: S (Spikes), P (Paths), I (Interfaces), D (Data), R (Rules). Produces ready-to-use stories and artifacts across lenses. Role- Business Analyst, Product Owner, Tech Lead Tags- #SPIDR #Decomposition #FeatureSlicing #Backlog #Jira #Rally Version: 1.0 Last_updated: 14-Aug-2025 Author: Dheeraj Sangore

Prompt:

You are an experienced BA and Agile practitioner. Convert the feature below into a SPIDR-structured backlog. “{Insert feature here}”

Objectives: - Reveal unknowns and risks early (S) - Slice delivery by user/system flows (P) - Define the contracts and surfaces (I) - Model and govern data (D) - Codify business logic (R)

Deliverables: 1) Feature summary: outcomes, metrics, scope/non-goals, stakeholders 2) SPIDR overview table | Lens | Purpose | Outputs | |------|---------|---------| | S | Reduce uncertainty | Spike backlog, decision log | | P | Slice flows | Path stories with Gherkin ACs | | I | Define contracts | OpenAPI/UI specs, contract tests | | D | Model/migrate data | ERD/DDL, mappings, quality checks | | R | Formalize logic | Decision tables, rule stories |

3) Uncertainties inventory (map each to lens) 4) Backlog by lens (ready for Jira/Rally) - S: Spike stories (timeboxed, decision-focused) - P: Path stories (happy/alt/sad/edge) - I: Interface stories (API/UI/Event with contracts and tests) - D: Data stories (model, mapping, migration, quality) - R: Rule stories (decision tables and BDD cases) 5) Cross-cutting concerns: security, privacy, performance, observability, rollout 6) Dependencies and sequencing: minimal viable path first; surface critical path 7) Acceptance strategy: test types per lens; entry/exit criteria 8) Decision log: date, decision, owner, context, options, impact 9) References: specs, diagrams, repos, contacts

Formatting guidelines: - Use concise bullets and tables; prefer Given/When/Then ACs - Keep each story thin and independently valuable - Link artifacts (specs/diagrams) where applicable

Template — Start Here

Feature summary - Purpose: {why} - Outcomes: {metrics} - Scope: {in} - Non-goals: {out} - Stakeholders: {roles}

Uncertainties inventory (mapped to SPIDR) | # | Uncertainty | Lens | Risk | Notes | |---|-------------|------|------|-------| | 1 | {unknown} | S | High | {note} |

Backlog by lens S – Spikes - Title: Spike: Investigate {topic} Timebox: {days} AC: {answers+artifacts+decision}

P – Paths - Title: Path: {actor} {verb} {goal} – {variation} AC: Given/When/Then

I – Interfaces - Title: Interface: API – {purpose} AC: Spec+examples+contract tests

D – Data - Title: Data: {entity/process} – {action} AC: ERD/DDL+mapping+quality checks

R – Rules - Title: Rule: {decision/validation} – {context} AC: Decision table + BDD cases

Sequencing plan - Earliest usable slice: {describe} - Dependencies: {list} - Risks and mitigations: {list}

Decision log | Date | Decision | Owner | Context | Options | Impact | |------|----------|-------|---------|---------|--------| | {dd-mmm-yyyy} | {text} | {name/role} | {short} | {list} | {short} |
