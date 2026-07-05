<div align="center">

# Roshan Kumar
### Cloud Security & SOC

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&center=true&width=600&lines=Building+AWS+security+tooling+with+Python;Running+a+home+SOC+lab+with+Wazuh;CIS+Benchmarks+%7C+MITRE+ATT%26CK+%7C+boto3" alt="Typing SVG" />

</div>

---

## About Me

Final-year cybersecurity student building practical, working tools rather than following tutorials. My focus is Cloud Security, with SOC fundamentals as the base.

Recent work: built an AWS security assessment tool from scratch (Python, boto3) and set up a home SOC lab (Wazuh) to practice detection and triage against real attack techniques. Both are public, documented, and actively maintained.

Currently looking for a cybersecurity internship or entry-level role in Cloud Security or SOC operations.

---

## Featured Projects

### 🛡️ [CloudSentinel](https://github.com/r0shhh/CloudSentinel) — AWS Security Assessment Tool
Python tool that scans AWS infrastructure (S3, IAM, EC2, CloudTrail, RDS, VPC, EBS) across all regions for misconfigurations. Every check maps to a CIS AWS Foundations Benchmark v5.0.0 control, with severity sourced from AWS Security Hub's official documentation — not self-assigned.

- Config-driven plugin architecture using `importlib` — new checks require only a scanner function and one YAML entry, no core code changes
- Multi-region scanning with dynamic, region-scoped client creation
- 28 unit tests (`pytest` + `moto`) that caught real bugs during development
- Built collaboratively — feature branches, PR review, branch protection

**Stack:** Python, boto3, pytest, moto, Rich, YAML

---

### 🔍 [wazuh-detection-lab](https://github.com/r0shhh/wazuh-detection-lab) — SIEM & Threat Detection
Home SOC lab — Wazuh manager, Windows and Linux agents, Kali as the attacker — built to practice detection and triage against real MITRE ATT&CK techniques, not just tool installation.

First completed scenario — **T1110 SSH Brute Force**:
- Traced the actual detection rule chain (single-fail rule → correlation rule) before trusting any alert
- Predicted the expected alert before running the attack, then confirmed it
- Found independent corroborating log sources as defense-in-depth evidence
- Triaged by blast radius, ruled out a false lead via timestamp correlation
- Identified a real detection gap (threshold evasion) with concrete remediation

Documented real operational incidents along the way (agent version mismatches, disk corruption recovery).

**Stack:** Wazuh, Linux, Kali, MITRE ATT&CK

---

## Tech Stack

**Cloud & Security Tools**
<p>
  <img src="https://skillicons.dev/icons?i=aws,linux,bash" />
</p>

- AWS (IAM, S3, EC2, CloudTrail, RDS, VPC, EBS) — applied via CloudSentinel
- Wazuh, Splunk
- CIS Benchmarks, MITRE ATT&CK
- Networking fundamentals, Wireshark, Nmap

**Languages & Tooling**
<p>
  <img src="https://skillicons.dev/icons?i=python,git,github" />
</p>

- Python — boto3, pytest, moto, Rich
- Git/GitHub — branching, PR review, branch protection
- YAML-based config design
- C++, Bash

---

## Current Focus

```yaml
Active:
  - Applying for cybersecurity internships / entry-level roles
  - Expanding wazuh-detection-lab with more MITRE ATT&CK techniques
  - Maintaining CloudSentinel

Next up:
  - More detection scenarios (privilege escalation, lateral movement)
  - Deeper SOC triage/incident-response documentation
```

---

## Connect With Me

<p>
  <a href="https://www.linkedin.com/in/roshan-kumar-3b6136174/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="https://github.com/r0shhh">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
  </a>
</p>

<div align="center">

### Building real skills, one at a time.

</div>
