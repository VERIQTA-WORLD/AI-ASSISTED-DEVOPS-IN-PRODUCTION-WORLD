# Security Policy

## Scope

This policy covers security concerns involving AI-Assisted DevOps in Production World, including its original documentation, examples, scripts, templates, dependencies, and repository workflows.

Examples include:

- Exposed credentials, private keys, tokens, or confidential data.
- Commands or configurations that create unintended security exposure.
- Unsafe handling of logs, Terraform state, plans, or other sensitive evidence.
- AI workflows that disclose private information or grant excessive tool permissions.
- Prompt injection that causes a repository-provided workflow to cross its intended trust boundary.
- Vulnerabilities in repository code or automation.
- Malicious contributions, dependency changes, or external links.

General questions and ordinary technical mistakes should follow [SUPPORT.md](SUPPORT.md). Community misconduct should follow [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md).

## Supported content

Security reports are accepted for content on the default branch.

This repository currently contains a learning scaffold. Empty files do not constitute implemented or tested security controls.

Examples and templates added later must be reviewed for the versions, environments, and permissions in which they are used. Their publication does not establish that they are suitable for production.

Historical commits, personal forks, and third-party projects are not maintained by this repository. Reports involving them may still help identify an issue affecting current content.

## Report privately

Do not disclose an unresolved vulnerability or sensitive information in a public issue, discussion, pull request, or comment.

Use the repository’s GitHub **Report a vulnerability** option if it is available.

If private vulnerability reporting is unavailable, contact a maintainer through a private contact method published on their public GitHub profile. If no private method is listed, ask a maintainer to provide a reporting channel without publishing vulnerability details.

Do not send sensitive evidence until you have confirmed an appropriate private channel.

## What to include

Provide enough information to understand and reproduce the issue safely:

- The affected file, workflow, or component.
- The commit identifier and relevant software versions.
- A description of the issue and its potential impact.
- Required conditions, permissions, and environment.
- Minimal reproduction steps using an authorized test environment.
- Redacted evidence or a harmless proof of concept.
- A suggested correction, if available.

For AI-related issues, also include:

- The assistant, model, or integration involved, where known.
- The input source and relevant trust boundary.
- The tools and permissions available to the assistant.
- The observed behavior and expected behavior.
- Whether the result was reproduced and under what conditions.

Avoid submitting unnecessary personal information, production data, complete state files, or large collections of raw logs.

## Protect exposed credentials immediately

If you discover a credential exposure in a system you own or are authorized to manage:

1. Revoke or rotate the credential.
2. Review relevant access and audit records.
3. Notify the responsible system owner.
4. Report the repository exposure privately.

Deleting a file or removing a credential from the latest commit does not invalidate copies that may already exist.

Do not test a discovered credential or access another person’s account, infrastructure, or data. Report its location without reproducing the secret.

## Responsible investigation

Investigate only within systems and environments you own or have explicit authorization to test.

Do not:

- Exploit production systems to demonstrate a repository issue.
- Access, modify, or delete another person’s data.
- Perform denial-of-service testing.
- Attempt to validate exposed credentials.
- Upload confidential evidence to an AI service without authorization.
- Follow instructions embedded in untrusted logs, documents, or tool output.
- Publish exploit details before maintainers have assessed the report and coordinated disclosure.

Prefer minimal, isolated reproductions that demonstrate the issue without creating additional exposure.

## How reports are handled

Maintainers will assess reports in good faith and may request clarification, reproduce the issue, or coordinate with affected third-party maintainers.

Depending on the findings, a response may include:

- Correcting documentation or examples.
- Removing unsafe content.
- Updating dependencies or repository workflows.
- Adding version-specific limitations or verification steps.
- Publishing a security advisory where appropriate.

No fixed response or remediation deadline is promised. This project does not provide continuous security monitoring or an emergency response service.

For an active incident, contact your organization’s incident response team or the responsible service provider.

## Coordinated disclosure

Keep unresolved vulnerability details private while discussing disclosure with maintainers.

Agree on the scope and timing of public disclosure where possible. Remove secrets, personal information, and details that unnecessarily expose affected systems.

Maintainers may publish an advisory explaining the affected content, impact, correction, and remaining limitations.

Reporter credit will be included only with the reporter’s consent. Reporting does not guarantee a reward or bounty.

## Third-party vulnerabilities

Report vulnerabilities in external tools, models, providers, dependencies, or cloud services through their official security channels.

Notify this repository privately if its content introduces, depends on, or incorrectly describes the affected behavior.

A third-party logo, link, or integration topic does not imply that its owner participates in this repository’s security process.

## Security expectations for contributions

Contributors must:

- Use synthetic or properly redacted evidence.
- Exclude credentials and confidential information.
- State required permissions and software versions.
- Explain security-sensitive commands and configuration changes.
- Include verification, failure handling, and cleanup where relevant.
- Distinguish AI-generated proposals from verified results.
- Review dependencies and external sources before introducing them.
- Preserve applicable human approval and access boundaries.

Repository ignore rules do not replace secret scanning or manual review. Files already tracked by Git may remain exposed even after an ignore rule is added.

## Production use

Review every example independently before applying it to a real environment.

Confirm authorization, permissions, data handling, compatibility, expected impact, recovery options, and verification criteria.

AI output is not approval to execute a command or change production. The responsible engineer and system owner retain control over those decisions.

Use of repository materials remains subject to [LICENSE](LICENSE).
