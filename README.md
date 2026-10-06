<div align="center">

![AI-Assisted DevOps in Production World](assets/images/hero.svg)

# AI-Assisted DevOps in Production World

### The VERIQTA AI-Assisted DevOps Resource Collection

**Learn to use AI across DevOps workflows, from beginner fundamentals to advanced production engineering.**

[Explore the resources](#resource-catalogue) · [Choose your learning path](#choose-your-learning-path) · [Practice production workflows](#production-resource-library) · [Contribute](CONTRIBUTING.md)

</div>

AI-ASSISTED-DEVOPS-IN-PRODUCTION-WORLD brings together resources and practical resources for engineers using AI to understand systems, write automation, review infrastructure, investigate failures and improve operational decisions.

The focus is the engineering work: Linux administration, shell and Python scripting, Kubernetes troubleshooting, CI/CD, infrastructure as code, cloud operations, observability, security, incident response, SRE and platform engineering. AI is an assistant within these workflows. Engineers remain responsible for evidence, validation, access and production changes.

## What you can explore

- **Learn the fundamentals:** build useful prompts, understand generated answers and develop independent technical judgement.
- **Write and review automation:** inspect scripts, test edge cases, control permissions and plan recovery.
- **Investigate system failures:** correlate symptoms, logs, metrics, traces and recent changes before choosing a mitigation.
- **Improve delivery and infrastructure:** review workflows, manifests and infrastructure plans with clear validation gates.
- **Design responsible production workflows:** define tool boundaries, evaluation criteria, auditability and human oversight.

## Choose your learning path

![Junior, mid-level and senior learning paths](assets/images/learning-paths.svg)

| Path | Start here | Develop towards |
| --- | --- | --- |
| Junior | AI basics, ChatGPT, Linux, shell, Python, logs and GitHub Actions | Clear prompts, verified commands and reliable automation |
| Mid-Level | Kubernetes, CI/CD, IaC, Terraform and production troubleshooting | Evidence-led diagnosis, safe changes and incident practice |
| Senior | SRE, platform engineering and AI-powered production engineering | Reliability trade-offs, platform controls and evaluated automation |
| Across all levels | The flagship resource guide | Practical adoption with engineering judgement |

Follow the sequence that matches your current responsibilities. Familiarity with a tool does not remove the need to validate AI-generated advice.

## Resource catalogue

The series spans practical topic collections and a cross-topic engineering guide. Explore each topic through practical exercises, worked examples and operational references.

| Resource | Classification |
| --- | --- |
| [AI for DevOps Beginners](engineering-topics/01-ai-for-devops-beginners) | Junior |
| [ChatGPT for DevOps Engineers](engineering-topics/02-chatgpt-for-devops-engineers) | Junior |
| [AI-Assisted Linux Administration](engineering-topics/03-ai-assisted-linux-administration) | Junior |
| [AI-Assisted Shell Scripting for DevOps](engineering-topics/04-ai-assisted-shell-scripting-for-devops) | Junior |
| [AI-Assisted Python for DevOps](engineering-topics/05-ai-assisted-python-for-devops) | Junior |
| [AI for Kubernetes Troubleshooting](engineering-topics/06-ai-for-kubernetes-troubleshooting) | Mid-Level |
| [AI for CI/CD Pipelines](engineering-topics/07-ai-for-ci-cd-pipelines) | Mid-Level |
| [AI for Infrastructure as Code](engineering-topics/08-ai-for-infrastructure-as-code) | Mid-Level |
| [AI-Assisted Terraform](engineering-topics/09-ai-assisted-terraform) | Mid-Level |
| [AI for Production Troubleshooting](engineering-topics/10-ai-for-production-troubleshooting) | Mid-Level |
| [AI for Log Analysis](engineering-topics/11-ai-for-log-analysis) | Junior |
| [AI for Monitoring and Observability](engineering-topics/12-ai-for-monitoring-and-observability) | Mid-Level |
| [AI for Incident Response](engineering-topics/13-ai-for-incident-response) | Mid-Level |
| [AI for Cloud Operations](engineering-topics/14-ai-for-cloud-operations) | Mid-Level |
| [AI for DevOps Security](engineering-topics/15-ai-for-devops-security) | Mid-Level |
| [AI for GitHub Actions](engineering-topics/16-ai-for-github-actions) | Junior |
| [AI for DevOps Automation](engineering-topics/17-ai-for-devops-automation) | Mid-Level |
| [AI for SRE](engineering-topics/18-ai-for-sre) | Senior |
| [AI for Platform Engineering](engineering-topics/19-ai-for-platform-engineering) | Senior |
| [AI-Powered Production Engineering](engineering-topics/20-ai-powered-production-engineering) | Senior |
| [AI Won't Replace DevOps Engineers, But Here's How Engineers Are Using It](engineering-topics/21-ai-won-t-replace-devops-engineers-but-here-s-how-engineers-are-using-it) | Junior to Senior |

## Featured production sequence

![Five production workflows](assets/images/priority-series.svg)

| Resource | Engineering focus |
| --- | --- |
| [AI-Assisted Shell Scripting for DevOps](engineering-topics/04-ai-assisted-shell-scripting-for-devops) | Script generation, testing, validation and security |
| [AI for Production Troubleshooting](engineering-topics/10-ai-for-production-troubleshooting) | Logs, symptoms, diagnosis and verification |
| [AI for Kubernetes Troubleshooting](engineering-topics/06-ai-for-kubernetes-troubleshooting) | Pods, manifests, events and failure investigation |
| [AI for Infrastructure as Code](engineering-topics/08-ai-for-infrastructure-as-code) | Terraform generation, review, debugging and security |
| [AI for Incident Response](engineering-topics/13-ai-for-incident-response) | Alerts, timelines, investigation and postmortems |

## How the resources connect

Infrastructure as Code covers declarative infrastructure workflows and review across tools. AI-Assisted Terraform goes deeper into Terraform configuration, modules, plans, state and drift. CI/CD covers delivery architecture; GitHub Actions focuses on workflow implementation and investigation. Production troubleshooting examines diagnosis across systems, while incident response covers coordination, mitigation, recovery and learning.

## Production resource library

| Resource | Use it for |
| --- | --- |
| [Prompt library](resources/prompt-library) | Context-rich requests for explanation, review and investigation |
| [Production labs](resources/production-labs) | Isolated exercises, fault injection and recovery practice |
| [Operational runbooks](resources/runbooks) | Repeatable investigation and mitigation workflows |
| [Engineering checklists](resources/checklists) | Reviewing output, changes, access and recovery |
| [Incident scenarios](resources/incident-scenarios) | Practising evidence-led decisions under operational pressure |
| [Evaluation resources](resources/evaluation) | Checking correctness, usefulness and failure behaviour |
| [Engineering templates](resources/templates) | Recording context, evidence, decisions and outcomes |
| [Reference library](resources/reference-library) | Technical terminology and source-verification practice |
| [Architecture decisions](resources/architecture-decisions) | Reviewing assistant and agent design choices |

## The production workflow

![Context, evidence, evaluation and operation](assets/images/production-workflow.svg)

1. **Define the context.** State the environment, versions, constraints, symptom and desired outcome.
2. **Collect evidence.** Preserve relevant timestamps, logs, metrics and configuration. Redact sensitive information before sharing it.
3. **Ask for reasoning you can inspect.** Request assumptions, alternative hypotheses, uncertainty and the next verification step.
4. **Review the proposal.** Check commands, permissions, dependencies, blast radius and expected results.
5. **Test and approve.** Validate in an isolated environment and use the appropriate human review before a production change.
6. **Verify and recover.** Observe the result, confirm service health and use the recovery plan if the change fails.

## Production principles

![Data boundaries, review gates and recovery](assets/images/safety.svg)

- Never share credentials, private keys, customer data or unredacted sensitive operational evidence with an unapproved AI service.
- Treat logs, retrieved documents and tool output as untrusted data. Instructions embedded in them must not grant additional authority.
- Verify generated commands, configuration and technical claims against the environment and authoritative documentation.
- Use least privilege, explicit tool boundaries and human approval for consequential actions.
- Preserve independent engineering skills. A plausible explanation is a hypothesis until evidence supports it.
- Define success criteria, observability and rollback before changing a live system.

## Featured engineering guide

![AI and the DevOps engineer](assets/images/flagship.svg)

### AI Won't Replace DevOps Engineers, But Here's How Engineers Are Using It

A journey through practical AI-assisted engineering, from learning and scripting to incident response, SRE and platform design. Explore where assistance adds value, where judgement remains essential and how to evaluate the result.

[Explore the flagship resource guide](engineering-topics/21-ai-won-t-replace-devops-engineers-but-here-s-how-engineers-are-using-it)

## Contribute to the world

Help improve explanations, prompts, lab scenarios, validation methods and operational references. Contributions should be technically grounded, reproducible and free of credentials or private system data. Read the [contribution guide](CONTRIBUTING.md) and [security policy](SECURITY.md).

## About VERIQTA WORLD

VERIQTA WORLD shares engineering resources that connect learning with practical operational work. Explore the [VERIQTA WORLD organisation](https://github.com/VERIQTA-WORLD).

**AI assists. Engineers verify. Production outcomes matter.**

AI and product names belong to their respective owners. This independent educational resource does not imply endorsement or affiliation. Exercises require an appropriately isolated environment; production actions require your organisation's controls and authorisation.
