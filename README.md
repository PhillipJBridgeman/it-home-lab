# Phillip’s Home Lab  
**Cumulative Learning, Operations Practice, and Certification Projects**

---

## Purpose

This repository documents a **long-term, evolving home lab** used to build and reinforce practical IT skills through **hands-on experimentation, troubleshooting, and structured documentation**.

The lab is designed to:

- Support **industry certification preparation**
- Practice **job-realistic IT tasks** and workflows
- Produce **interview-ready examples** grounded in real scenarios
- Strengthen **foundational systems knowledge**
- Serve as a **living technical reference** over time

This is not a short-term portfolio. It is a **career-grade learning environment**.

---

## Intended Audience

- **Personal learning and long-term reference**
- **Interview discussion and technical demonstrations**
- **Recruiters and hiring managers** evaluating hands-on capability
- Practice ground for **enterprise-style documentation**

---

## Scope & Philosophy

- General-purpose home lab that evolves alongside career goals
- Emphasis on **operational IT disciplines**:
  - Troubleshooting
  - Deployment
  - Diagnostics
  - Decision-making under constraints
- Not a production environment
- Not focused on exploitative security or niche DevOps tooling
- Technologies are explored **only when relevant to current objectives**

> The focus is on **thinking like an IT professional**, not collecting tools.

---

## Certification Alignment

Current and planned work aligns with both **exam objectives** and **real job duties**.

### Active Focus
- **CompTIA A+**
- **Microsoft AZ-900**

### Near-Term / Planned
- Network+
- Security+
- Linux+
- AZ-104
- Additional vendor or domain-specific certifications as appropriate

Labs and playbooks are explicitly mapped to:
- Exam domains
- Common Tier-1 / Tier-2 support tasks
- Operations and infrastructure fundamentals

---

## Lab Environment

### Active Systems
- Legacy desktop PC (Windows 7-era hardware)
- Windows 11 Pro desktop
- Windows 11 Home laptop
- Ubuntu desktop laptop
- Synology NAS
- Virtualization platforms:
  - VirtualBox
  - Hyper-V

### Cloud Platforms (Used Selectively)
- Microsoft Azure
- AWS
- Google Cloud
- Microsoft 365

Cloud usage is **deliberate and minimal**, prioritizing:
- Cost control
- Architectural correctness
- Tear-down after use

---

## Use of Linux

Linux is used for:
- Supporting legacy hardware
- CLI-first troubleshooting practice
- Reinforcing OS-agnostic fundamentals
- Preparation for Linux-focused certifications
- Understanding cross-platform behavior

---

## Repository Structure (Guidance)

```text
README.md               # This document
LICENSE
CONTRIBUTING.md
CODE_OF_CONDUCT.md
.github/
  ├─ ISSUE_TEMPLATE/
  ├─ PULL_REQUEST_TEMPLATE.md
  └─ workflows/
docs/                   # Diagrams, designs, reference material
labs/
  ├─ comptia_aplus/
  ├─ azure/
  └─ linux/
playbooks/              # Troubleshooting templates and completed playbooks
scripts/                # Automation snippets (PowerShell, Bash, Python)
assets/                 # Screenshots and photos (no secrets)
archive/                # Retired or superseded experiments
```

### Branching & Releases
- `main` — stable reference
- `develop` — ongoing work
- `feature/*` — experiments or isolated changes
- Semantic tags for milestones  
  *(e.g., v1.0 — CompTIA A+ readiness)*

---

## Troubleshooting Playbooks

Playbooks document **repeatable problem-solving**, not just fixes.

Each playbook should capture:
- Context and scope
- Environment and assumptions
- Symptoms and indicators
- Diagnostic steps and tools used
- Root cause
- Resolution and validation
- Lessons learned

Both **checklist** and **step-by-step** formats are encouraged where useful.

---

## Documentation Standards

- Emphasize **reasoning and decision-making**
- Capture **reproducible steps**
- Use screenshots or photos only when they add clarity
- Never store credentials, secrets, or sensitive data
- Favor depth when it improves repeatability
- Write so **another technician could reproduce the work without context**

---

## Repo & Collaboration Practices

- `README.md` — high-level orientation
- `CONTRIBUTING.md` — formatting, commit, and contribution standards
- Issue templates:
  - Bug
  - Enhancement
  - Lab request
- Pull request template:
  - Summary
  - Testing performed
  - Impact / risk
- Lightweight GitHub Actions may be used for:
  - Markdown linting
  - Spelling or formatting checks

---

## Roadmap / Future Additions

Planned expansions include:
- Structured lab exercises mapped to certification objectives
- Reusable playbook templates (Markdown / YAML)
- Infrastructure-as-Code examples (Terraform, ARM, Bicep)
- Configuration management samples (Ansible, PowerShell DSC)
- Containerized lab environments (Docker Compose / k3s)
- Automated cloud teardown scripts to minimize cost
- Architecture diagrams and system flows
- Certification progress trackers and study logs

---

## Current Phase & Immediate Goal

- Initial environment setup and hardware assessment
- Primary objective: **CompTIA A+ Core 1 readiness**
- Secondary objective: Build **Tier-1 troubleshooting documentation** that mirrors real support work

---

## Tone & Style Guidelines

- Professional, technical, methodical
- First-person where reflection adds value
- Neutral, operational tone where documentation clarity matters
- Written so content can be reused directly for:
  - Resume bullets
  - Interview explanations
  - Internal documentation examples

---

## Notes & Constraints

- All systems are **non-production**
- Misconfigurations are introduced intentionally for learning
- Cloud resources are ephemeral and destroyed when no longer needed

---

## Summary

This repository is a **living technical reference** documenting how systems fail, how problems are approached, and how resolutions are verified.

The emphasis is on **operational thinking, reproducibility, and professional documentation** rather than novelty or scale.

---

### Troubleshooting Playbook Header Template

```text
Title:
Date:
Author:
Environment:
Symptoms:
Diagnostic Steps:
Root Cause:
Resolution:
Verification:
Notes / Lessons Learned:
```
