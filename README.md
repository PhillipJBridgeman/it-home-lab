# Phillip’s Home Lab – Cumulative Learning & Certification Projects

## Purpose
A long-term, evolving environment to support practical skill development and certification-aligned projects. Primary goals:
- Pass industry certifications
- Practice job-like IT tasks
- Produce interview-ready examples
- Strengthen fundamentals and troubleshooting
- Maintain a long-term technical reference

## Audience
- Personal learning and reference
- Interview discussion and demonstrations
- Recruiters / hiring managers reviewing hands-on capability
- Documentation practice for enterprise IT roles

## Scope & Philosophy
- General-purpose home lab that evolves with career goals
- Prioritizes operational IT skills (troubleshooting, deployment, diagnostics, decision-making)
- Not a production environment; not focused on advanced DevOps or exploitative security
- Technologies explored when relevant to current objectives

## Certification Alignment
- Current focus: CompTIA A+, Microsoft AZ-900
- Near-term: Network+, Security+, Linux+, AZ-104, other vendor/domain certs
- Labs and projects map to exam objectives and real IT tasks

## Lab Environment
### Active Systems
- Legacy Desktop PC (Windows 7-era hardware)
- Windows 11 Pro Desktop
- Windows 11 Home Laptop
- Ubuntu Desktop Laptop
- Synology NAS
- Virtualization: VirtualBox, Hyper-V

### Cloud Platforms (used selectively)
- Microsoft Azure
- AWS
- Google Cloud
- Microsoft 365

## Use of Linux
- Use cases: legacy hardware support, CLI troubleshooting, OS-agnostic fundamentals, Linux cert prep

## Lab Structure (Repository guidance)
Suggested top-level repo layout:
- README.md (this document)
- LICENSE
- CONTRIBUTING.md
- CODE_OF_CONDUCT.md
- .github/
    - ISSUE_TEMPLATE/
    - PULL_REQUEST_TEMPLATE.md
    - workflows/ (CI or automation)
- docs/ (designs, diagrams, reference guides)
- labs/
    - comptia_aplus/
    - azure/
    - linux/
- playbooks/ (troubleshooting templates and completed playbooks)
- assets/ (screenshots, photos; no secrets)
- scripts/ (automation snippets)
- archive/ (retired experiments)

Branching & release basics:
- main — stable reference
- develop — ongoing changes and drafts
- feature/* — experimental work
- Use semantic tags/releases for major milestones (e.g., v1.0 — CompTIA A+ readiness)

## Troubleshooting Playbooks
Playbooks should capture:
- Title and context
- Environment and preconditions
- Symptoms
- Diagnostic steps and tools
- Root cause
- Resolution and verification
- Lessons learned
Provide both checklist and step-by-step variants.

## Documentation Standards
- Emphasize reasoning, decision-making, and reproducible steps
- Include screenshots/photos only when clarifying
- Never include passwords or secrets
- Prefer depth when it improves repeatability
- Write so another technician can reproduce results

## Repo & Collaboration Guidance
- README: high-level overview and quick start
- CONTRIBUTING.md: contribution rules, formatting, commit message conventions
- ISSUE_TEMPLATE: bug, enhancement, lab request
- PULL_REQUEST_TEMPLATE: summary, testing performed, impact
- Use GitHub Actions for lightweight checks (markdown lint, spelling)
- Track issues for requested labs, fixes, and roadmap items

## Roadmap / Future Additions
- Structured lab exercises mapped to exam objectives
- Playbook templates (YAML/Markdown)
- Infrastructure-as-code examples (Terraform, ARM, Bicep)
- Configuration examples (Ansible, PowerShell DSC)
- Containerized labs (Docker Compose / k3s)
- Automated lab teardown scripts to minimize cloud spend
- Visual architecture diagrams in docs/
- Progress tracker for certification objectives and study logs

## Current Phase & Goal
- Initial setup and hardware assessment
- Goal: Achieve CompTIA A+ Core 1 readiness and build Tier-1 troubleshooting documentation

## Tone & Style
- Professional, technical, methodical
- Mix of first-person and neutral documentation depending on context
- Written to support resume bullets and interview explanations without rewriting

## Notes
- All systems are non-production; misconfigurations introduced intentionally for practice
- Cloud resources are ephemeral and torn down when not required

## Summary
This repository is a living technical reference that documents how problems are approached and solved. Structure contributions around reproducible playbooks, clear documentation standards, and certification-aligned labs to maximize learning and employer-facing value.

Template snippet — Troubleshooting playbook header (use in playbooks/*.md):
- Title:
- Date:
- Author:
- Environment:
- Symptoms:
- Steps:
- Root cause:
- Resolution:
- Verification:
- Notes / Lessons learned:

