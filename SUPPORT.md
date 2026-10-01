# Support

Use this guide to ask questions, report technical problems, and suggest improvements to AI-Assisted DevOps in Production World.

Support focuses on the repository’s learning materials and documented workflows. It does not provide managed operations, emergency incident response, or authorization to change production systems.

## Current repository status

The repository is at the scaffold stage.

Public navigation, catalogues, and visual assets are available. Individual learning files, exercises, projects, case files, scripts, and configuration templates are intentionally empty.

An empty file is not a working example. Collection titles containing “50 Problems” or “100 Incidents” describe planned content, not completed cases.

Check [ROADMAP.md](ROADMAP.md) and [CHANGELOG.md](CHANGELOG.md) before reporting missing content.

## Where to ask

| Request | Channel |
|---|---|
| Question about published material | GitHub Discussions, if enabled |
| Reproducible error in instructions or code | GitHub Issue |
| Broken link or incorrect navigation | GitHub Issue |
| Suggested exercise, topic, or improvement | GitHub Issue |
| Security vulnerability or exposed secret | Private reporting process in [SECURITY.md](SECURITY.md) |
| Harassment or community misconduct | Private reporting process in [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) |
| Permission to reuse restricted materials | Permission process in [LICENSE](LICENSE) |

If Discussions is unavailable, open a clearly labeled question issue.

Use private channels for sensitive concerns. Do not include confidential details in a public issue.

## Before opening a request

1. Read the relevant resource and its status.
2. Search existing issues and discussions.
3. Check the documented prerequisites and versions.
4. Confirm that you are using the intended environment.
5. Collect a minimal, redacted reproduction.

Do not execute destructive commands or repeat a production failure solely to prepare a support request.

## Reporting a technical problem

Use a descriptive title and include:

- The affected file or resource path.
- The commit identifier, if known.
- What you expected to happen.
- What actually happened.
- Minimal reproduction steps.
- Relevant tool, provider, operating system, and runtime versions.
- Whether the environment is local, a lab, staging, or production.
- Redacted error output.
- Checks you have already completed.

Include only the evidence needed to understand the problem.

### Suggested issue format

**Resource:**  
Path or link to the affected material.

**Repository revision:**  
Commit identifier, if known.

**Environment and versions:**  
Relevant operating system, tools, providers, and dependencies.

**Expected behavior:**  
What the instructions or example led you to expect.

**Actual behavior:**  
What you observed.

**Reproduction steps:**  
A minimal sequence that can be followed in an authorized environment.

**Redacted evidence:**  
Relevant error output, configuration excerpts, or test results.

**Checks already completed:**  
What you verified and what remains uncertain.

## Questions about AI-assisted workflows

An AI response may differ from the example because models, context, tools, and services change.

When asking about an AI interaction, include where available:

- The exercise and workflow stage.
- The assistant or service and model identifier.
- The date of the interaction.
- The redacted prompt and relevant context.
- The relevant part of the response.
- Tool access available to the assistant.
- The claim or recommendation you are questioning.
- Independent verification results.

Do not submit an entire conversation when a short excerpt is sufficient.

A support discussion does not make an AI recommendation verified or authorize its execution.

## Protect sensitive information

Before posting, inspect evidence for:

- Passwords, tokens, private keys, and credentials.
- Customer records and personal information.
- Private repository content.
- Confidential infrastructure details.
- Sensitive values in Terraform state or plans.
- Secrets in environment variables, logs, screenshots, or AI conversations.

Replace sensitive values with clear placeholders. Preserve enough structure to explain the problem, and identify substitutions that may affect reproduction.

If a secret was exposed, revoke or rotate it through the responsible owner and follow [SECURITY.md](SECURITY.md). Editing the public message alone does not invalidate the credential.

## Suggesting new content

Explain:

- The engineering problem.
- The intended learner and prerequisites.
- Why AI assistance would be useful.
- The evidence that would be available.
- How an engineer would review and verify the answer.
- Expected permissions, costs, failure scenarios, and cleanup.

Prefer a specific problem over a general request for more prompts.

Proposals should align with [RESOURCE-STANDARD.md](RESOURCE-STANDARD.md).

## Production incidents

For an active production incident, follow your organization’s incident response process and contact the responsible system owner.

This repository does not offer continuous monitoring, on-call coverage, incident command, or guaranteed response times.

Repository guidance and support replies do not replace your change approval process. You remain responsible for authorization, impact assessment, verification, and recovery planning.

## Third-party tools and services

Use official support channels for account access, billing, service outages, licensing, or defects in external products.

If the repository’s instructions are incorrect or omit a relevant limitation, report the affected resource here as well.

A listed tool, logo, or integration does not imply a support agreement with its owner.

## Response expectations

Maintainers review requests as availability permits.

There is no guaranteed response or resolution time. A request may require more evidence, be redirected to another project, or remain unresolved.

Requests may be closed when they are duplicates, outside scope, no longer reproducible, or missing information needed for investigation.

Please avoid repeated messages asking for updates. Add relevant new evidence to the existing request instead.

## Community expectations

Keep questions and feedback respectful. Discuss technical claims and evidence without personal attacks.

Follow [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) in issues, discussions, and reviews.

## Related documents

- [Resource standard](RESOURCE-STANDARD.md)
- [Roadmap](ROADMAP.md)
- [Changelog](CHANGELOG.md)
- [Security policy](SECURITY.md)
- [Code of conduct](CODE_OF_CONDUCT.md)
- [Contribution guide](CONTRIBUTING.md)
- [License](LICENSE)
