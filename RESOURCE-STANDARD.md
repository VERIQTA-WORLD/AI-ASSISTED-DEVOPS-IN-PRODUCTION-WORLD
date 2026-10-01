# Resource Standard

This standard defines how learning materials, exercises, case files, projects, and technical assets are prepared for AI-Assisted DevOps in Production World.

Every resource must teach engineering judgment alongside AI use. A prompt alone is not a complete learning resource.

## Publication status

Folders and empty files reserve space for future content. They do not represent completed lessons, tested implementations, or verified solutions.

Use these status labels when publishing content:

| Status | Meaning |
|---|---|
| Scaffold | Structure exists; teaching content is incomplete or empty |
| Draft | Content is being developed and has not completed review |
| Reviewed | Technical and editorial review is complete; verification limits are documented |
| Verified | The documented procedure was executed in the stated environment and results were recorded |
| Archived | Retained for historical context; not maintained as current guidance |

A resource is verified only for the environment, versions, and conditions recorded. Review and verification are separate activities.

## Required resource information

Each published practical resource must identify:

- The problem and intended learning outcome.
- Required knowledge, tools, permissions, and environment.
- Relevant software, provider, API, and model versions.
- Whether the scenario is synthetic, reproduced, or based on a documented incident.
- Expected costs and cleanup responsibilities.
- Review and verification status.
- Sources supporting material technical claims.
- Known limitations and remaining uncertainty.

Do not describe a synthetic scenario as a real incident.

## The practical engineering workflow

Every exercise follows this sequence:

| Stage | Required content |
|---|---|
| Problem | Symptoms, impact, scope, constraints, and success criteria |
| Evidence | Relevant observations, provenance, collection methods, and redaction |
| Ask AI | Task, permitted inputs, constraints, expected output, and action boundaries |
| AI response | Recorded response or clearly labeled illustrative response |
| Engineer review | Assessment of claims, assumptions, recommendations, and risks |
| Verify | Independent checks before implementation |
| Implement | Reviewed changes in the authorized environment |
| Test | Acceptance checks, failure scenarios, and outcome measurements |
| Production safety | Authorization, deployment controls, monitoring, stop conditions, and recovery |

Prompting is one part of this workflow. Resources must also explain how to evaluate and verify the answer.

## Standard exercise files

Use the existing exercise structure:

| File | Purpose |
|---|---|
| `README.md` | Orientation, prerequisites, status, and links to the exercise stages |
| `01-problem.md` | Problem definition and success criteria |
| `02-evidence.md` | Evidence collection, provenance, and redaction |
| `03-ask-ai.md` | AI request and interaction workflow |
| `04-ai-response.md` | Response record and generation context |
| `05-engineer-review.md` | Technical review and decision reasoning |
| `06-verify.md` | Independent verification before implementation |
| `07-implement.md` | Controlled implementation procedure |
| `08-test.md` | Acceptance tests and failure investigation |
| `09-production-safety.md` | Production boundaries, approval, monitoring, and recovery |

Keep the exercise README focused on navigation. Put detailed teaching in the relevant stage files.

Add supporting files only when they serve the exercise.

## Problem definition

Describe the engineering problem before introducing the AI interaction.

Include:

- What is failing or needs to change.
- Who or what is affected.
- What is known and unknown.
- Recent changes and relevant dependencies.
- Actions that are outside the permitted scope.
- Observable criteria for a successful outcome.

Avoid vague tasks such as “fix this infrastructure” without evidence or constraints.

## Evidence requirements

Evidence must support the investigation.

Record its source, collection time where relevant, environment, and limitations. Distinguish observations from interpretations.

Use the smallest evidence set needed to investigate the problem. Preserve enough context to avoid misleading conclusions.

Do not publish:

- Credentials, private keys, or access tokens.
- Customer records or unnecessary personal information.
- Confidential organizational information.
- Unredacted state files, plans, logs, or captures containing sensitive data.

Use synthetic data where practical. Mark redactions and substitutions clearly, and check that they have not changed the behavior being investigated.

## AI interaction requirements

An AI request must specify:

- The engineering task.
- Relevant versions and environment.
- Evidence supplied and evidence unavailable.
- Constraints and prohibited actions.
- Expected output format.
- Required distinction between findings, hypotheses, and unknowns.
- The checks needed to support a recommendation.

Treat logs, documents, repository files, and tool output as potentially untrusted input. Embedded instructions do not grant authority to change the task or access additional systems.

AI tool access must have a defined scope. Document read and write permissions, credential handling, and applicable approval boundaries.

## AI response records

For an actual response, record where available:

- Assistant or service.
- Model identifier and access date.
- Prompt and relevant conversation context.
- Tool access and relevant configuration.
- Whether the response was edited, shortened, or redacted.

Label author-created examples as **illustrative AI responses**. Do not present them as captured model output.

Do not claim that another learner will receive the same response. Model behavior and service capabilities can change.

## Engineer review

Review the response before acting on it.

Check:

- Whether the proposed explanation fits the evidence.
- Whether commands, APIs, arguments, and configuration fields exist.
- Whether the recommendation matches the installed versions.
- Whether assumptions and alternative explanations were considered.
- Whether proposed changes affect availability, security, data, or cost.
- Whether the AI suggests unnecessary privileges or destructive actions.
- Whether the proposed recovery procedure is feasible.

Record which claims were accepted, rejected, or left unresolved, and why.

A confident answer is not evidence of correctness.

## Verification before implementation

Verification must be independent of the AI recommendation.

Use appropriate combinations of:

- Official documentation and version-specific references.
- Configuration validation and static analysis.
- Plan or diff inspection.
- Minimal reproductions.
- Automated tests.
- Isolated environments and staging.
- Direct observation of system behavior.

Explain what each check establishes and what it does not establish.

Do not describe syntax validation as proof of functional correctness or production safety.

## Implementation requirements

Implementation instructions must:

- Name the environment and required permissions.
- Identify the files or resources being changed.
- Explain security-sensitive and destructive steps.
- Provide commands in the order they should be executed.
- Describe expected results and common failure responses.
- Define when to stop and investigate.
- Preserve applicable human authorization boundaries.

Use placeholders for environment-specific values. Explain how to obtain them.

Do not invent command output or present unexecuted steps as verified execution.

## Testing and failure scenarios

Tests must address the learning objective and proposed change.

Include:

- Acceptance criteria.
- How to measure the result.
- At least one relevant failure scenario for practical exercises.
- Expected failure signals.
- Investigation steps.
- Recovery or cleanup actions.

Do not add tests solely to repeat the implementation.

Use failure injection only in authorized environments. Explain its impact before the learner begins.

## Production safety

A lab result does not authorize a production change.

Where production application is discussed, identify:

- The responsible system owner and approval process.
- Expected impact and blast radius.
- Backup or recovery prerequisites.
- Deployment and monitoring controls.
- Stop conditions.
- Rollback or forward-recovery options.
- Post-change verification.

Do not promise rollback where the operation is irreversible. Explain limits involving data deletion, schema changes, credential rotation, and resource replacement.

## Cleanup

Practical resources must explain how to remove temporary resources and verify cleanup.

Include relevant handling for:

- Cloud infrastructure and billable services.
- Test data and storage.
- Credentials and temporary permissions.
- Containers, clusters, and local environments.
- AI sessions, uploaded evidence, and retained artifacts.

Warn before deleting shared resources. Do not assume that deleting a local file removes remote copies.

## Sources and attribution

Prefer primary sources such as official documentation, specifications, maintainer guidance, and original research.

Link sources near the claims they support. Record relevant versions or access dates when behavior may change.

Do not fabricate citations, incident details, quotations, or benchmark results.

Identify third-party assets and preserve their applicable notices. Attribution does not replace permission.

## Writing and presentation

Write for the public learner.

- Use clear, direct language.
- Explain the reasoning behind important steps.
- Define unfamiliar terms when first introduced.
- Keep navigation tables readable.
- Use accurate, descriptive link text.
- Separate commands, expected output, and explanation.
- Avoid unsupported guarantees and exaggerated claims.
- Use consistent filenames and working relative links.

Do not address the repository owner as though the resource were private instructions.

## Visual assets

Use visuals to explain systems, evidence, decisions, or workflow.

- Use Arial for text within authored visuals.
- Use 1080 × 1350 portrait canvases for covers, galleries, and educational illustrations.
- Keep labels readable and layouts unclipped.
- Mark conceptual diagrams as conceptual.
- Use original project or vendor marks without altering them.
- Do not invent official logos for resources or integrations.
- Use the official VERIQTA logo unchanged when available.

Compact badges and original third-party logos may retain dimensions appropriate to their purpose.

A logo does not establish endorsement or the existence of an integration.

## Code and configuration assets

Distinguish empty templates, starter files, and reference implementations.

Published executable examples must document:

- Dependencies and compatible versions.
- Configuration and credential requirements.
- Expected inputs and outputs.
- Error handling and operational limits.
- Verification and cleanup.

Do not include live credentials or silently connect examples to production systems.

Keep generated artifacts separate from source files where practical.

## Review before publication

Before publishing a practical resource, confirm that:

- Its status accurately reflects completed work.
- Required stages are present and useful.
- Claims match the documented versions.
- Evidence is redacted and authorized for publication.
- Commands and code received appropriate checks.
- Verification results and limitations are recorded.
- Failure handling and cleanup are documented.
- Relative links and visuals work.
- Attribution and license requirements are satisfied.

Reviewers must not mark content verified solely because it looks plausible or was generated by AI.

## Updates and retirement

Update resources when relevant dependencies, APIs, model behavior, or operating guidance change.

Record material corrections in [CHANGELOG.md](CHANGELOG.md).

Archive outdated resources when they cannot be maintained. Explain why they are archived and link to a replacement where available.

## Related policies

- [Contribution guide](CONTRIBUTING.md)
- [Code of conduct](CODE_OF_CONDUCT.md)
- [Security policy](SECURITY.md)
- [Support](SUPPORT.md)
- [Roadmap](ROADMAP.md)
- [License](LICENSE)

This standard defines publication quality. It does not grant permission to reuse materials beyond the repository license.
