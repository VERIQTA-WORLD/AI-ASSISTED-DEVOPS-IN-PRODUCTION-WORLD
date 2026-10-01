# Roadmap

AI-Assisted DevOps in Production World teaches engineers how to use AI to investigate problems, review changes, and support production work while retaining responsibility for decisions and outcomes.

This roadmap describes the planned development of the repository. It does not promise release dates or imply that reserved materials are complete.

## Current stage

The repository is at the scaffold stage.

Available:

- Public README, navigation tables, and catalogue indexes.
- 39 numbered engineering sections.
- 100 collection directions across 10 domains.
- An empty outline and starter exercise structure for each direction.
- Reserved project, lab, interview, notebook, and case-file folders.
- Visual assets and tool directories.

Learning notes, exercises, examples, implementations, and templates remain empty until developed and reviewed.

Titles containing “50 Problems” or “100 Incidents” describe planned scope, not published case counts.

## Development principles

Every practical resource will connect AI use to an engineering problem.

The standard workflow is:

1. Define the problem.
2. Gather and redact evidence.
3. Ask AI within explicit constraints.
4. Capture the response.
5. Review it as an engineer.
6. Verify claims and proposed behavior.
7. Implement in an authorized environment.
8. Test outcomes and failure scenarios.
9. Establish production controls and recovery options.

Prompting is one stage. Evidence, technical understanding, verification, and human control remain central throughout.

## Phase 1. Establish the learning foundation

Develop the guidance learners need before using AI with infrastructure or operational evidence.

| Area | Planned deliverables |
|---|---|
| Orientation | How to use the repository, learning paths, prerequisites, and lab setup |
| Engineering foundations | AI capabilities, limitations, uncertainty, and ownership |
| Evidence | Context selection, provenance, collection, and redaction |
| Interaction | Task framing, constraints, structured responses, and iterative questioning |
| Review | Claim checking, command inspection, version validation, and alternative hypotheses |
| Verification | Isolated tests, documentation checks, acceptance criteria, and recorded results |
| Human control | Authorization, access boundaries, stop conditions, and recovery planning |

### Completion criteria

- Learners can distinguish observations, hypotheses, and AI-generated claims.
- Published examples demonstrate redaction and independent verification.
- Review criteria are explicit and usable.
- Each resource states its status and verification limits.

## Phase 2. Publish a small set of complete exercises

Develop representative exercises before expanding the entire collection.

Initial candidates:

| Domain | Candidate problem |
|---|---|
| Terraform | A plan unexpectedly proposes replacing a production database |
| Linux | A service fails after a configuration change |
| Docker | A container exits or fails to shut down gracefully |
| Kubernetes | A workload remains Pending despite apparently available capacity |
| CI/CD | A pipeline fails after a dependency or permission change |
| Observability | An alert suggests a cause that the available evidence does not establish |

These are planned scenarios. Their inclusion does not establish that they have been implemented or verified.

### Completion criteria

Each published exercise includes:

- All nine workflow stages.
- An authorized, reproducible lab environment.
- Synthetic or properly redacted evidence.
- A recorded or clearly labeled illustrative AI response.
- Engineer review explaining accepted and rejected recommendations.
- Verification, acceptance tests, and a relevant failure scenario.
- Cleanup and documented limitations.

## Phase 3. Expand the 100-direction collection

Develop the collection in manageable groups.

| Domain | Collection numbers |
|---|---|
| Core DevOps and production engineering | 001–010 |
| Linux | 011–020 |
| Kubernetes | 021–030 |
| Terraform and infrastructure as code | 031–040 |
| Docker and containers | 041–050 |
| CI/CD | 051–060 |
| AWS, Azure, GCP, and multi-cloud | 061–070 |
| Networking and security | 071–080 |
| Observability, incidents, and reliability | 081–090 |
| Automation, data services, and engineering reviews | 091–100 |

For each direction, develop:

- A focused outline and learning objectives.
- Prerequisites and compatible tool versions.
- Practical exercises with increasing difficulty.
- Relevant evidence and supporting references.
- Review questions and assessment criteria.
- Explicit boundaries around production application.

Publish complete, useful units rather than treating folder creation as content completion.

## Phase 4. Build production case files

Develop investigations that teach reasoning under uncertainty.

Planned case-file elements:

- Symptoms, impact, and an incident timeline.
- Relevant architecture and recent changes.
- Evidence available at each stage.
- Competing explanations.
- AI recommendations and engineer assessment.
- Verification and response decisions.
- Recovery, follow-up actions, and remaining uncertainty.

Label every case as synthetic, reproduced, or based on a documented incident. Do not invent real-world provenance or expose confidential incident evidence.

### Completion criteria

- Evidence supports the stated conclusions.
- Hypotheses are distinguishable from confirmed findings.
- Recovery actions include their risks and limitations.
- Postmortem conclusions follow from the investigation.

## Phase 5. Develop projects and portfolio work

Add projects for Junior, Mid-Level, and Senior learners.

| Level | Planned emphasis |
|---|---|
| Junior | Bounded problems, evidence collection, response review, and basic verification |
| Mid-Level | Multiple tools, integration testing, automation, and operational tradeoffs |
| Senior | Architecture, access boundaries, evaluation design, reliability, and governance |
| Capstone | A complete AI-assisted workflow with documented controls and measured outcomes |

Projects must explain what the learner builds, how to verify it, how it fails, and how to recover or clean up.

Portfolio guidance must distinguish independently created work from repository materials whose publication requires permission under [LICENSE](LICENSE).

## Phase 6. Develop retrieval and tool-assisted workflows

Introduce integrations after the review and verification foundations are established.

Planned topics include:

- Retrieval from approved documentation and runbooks.
- Source freshness, citations, and access-aware retrieval.
- Read-only diagnostic integrations.
- Agent tool permissions and execution boundaries.
- MCP integration patterns.
- Approval gates and audit records.
- Prompt injection and malicious tool-output handling.
- Timeouts, cost limits, and stop mechanisms.

### Completion criteria

- Inputs, tools, permissions, and data flows are documented.
- Untrusted content does not grant additional authority.
- Failure behavior and unauthorized-action tests are included.
- Production access is not required to complete introductory exercises.

## Phase 7. Add evaluation and maintenance practices

Develop methods for assessing whether AI assistance improves engineering work.

| Area | Planned measures |
|---|---|
| Technical correctness | Supported claims, valid commands, and compatible configurations |
| Evidence use | Conclusions traceable to supplied or independently checked evidence |
| Operational behavior | Correct handling of uncertainty, failures, and action boundaries |
| Learning | Ability to explain, challenge, and verify recommendations |
| Efficiency | Time, cost, and review effort under documented conditions |
| Regression | Changes in outcomes after model, tool, or workflow updates |

Do not use response confidence, fluency, or length as substitutes for correctness.

Benchmark results must identify the environment, evaluation method, dataset provenance, and limitations.

## Publication gates

Before practical content is published, it must satisfy [RESOURCE-STANDARD.md](RESOURCE-STANDARD.md).

| Gate | Required outcome |
|---|---|
| Scope | A clear problem, learning objective, and permitted environment |
| Evidence | Authorized, relevant, and appropriately redacted inputs |
| Review | Technical claims and proposed actions assessed |
| Verification | Appropriate checks completed and their limits recorded |
| Operations | Failure handling, cleanup, and recovery documented |
| Presentation | Working navigation, readable assets, and clear instructions |
| Attribution | Sources and applicable asset terms identified |
| Status | Scaffold, Draft, Reviewed, Verified, or Archived accurately assigned |

Content may be published as Draft or Reviewed when that status is explicit. It must not be described as Verified without recorded execution evidence.

## Maintenance priorities

As content is developed:

- Correct errors before expanding affected material.
- Update version-sensitive guidance.
- Review external links and dependencies.
- Record material changes in [CHANGELOG.md](CHANGELOG.md).
- Archive outdated workflows with an explanation.
- Keep unresolved security details out of public discussions.
- Replace placeholders only with reviewed content.

## Contributing to the roadmap

Propose additions or changes through the process in [CONTRIBUTING.md](CONTRIBUTING.md).

A useful proposal identifies:

- The engineering problem.
- The intended learner.
- The evidence and environment required.
- The role AI would play.
- How recommendations would be reviewed and verified.
- Expected costs, risks, and cleanup.

Security concerns should follow [SECURITY.md](SECURITY.md).

## Scheduling

This roadmap is organized by dependencies and completion criteria. It does not set fixed publication dates.

Priorities may change as exercises are tested, learner feedback is received, or tools and services evolve.
