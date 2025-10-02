
# APT29 (Cozy Bear) — Sample CTI Brief (UK-focused)

Hi — I'm Tafadzwa. This repo contains a short, UK-focused cyber threat intelligence (CTI) brief I produced as a portfolio piece.  
It's deliberately compact (2–3 pages) and shows how I turn forensic/SOC findings and public sources into actionable intelligence for technical teams and leadership.

## What’s in this repo
- `APT29_CTI_Brief.docx` — editable Word version (good if you want to annotate).  
- `APT29_CTI_Brief.pdf` — printable/readable version for quick download.  
- `APT29_Detections_Appendix.docx` — Sigma rules, translated SIEM queries, and validation notes.  
- `img/` — screenshots exported from Uncoder.io.  
- `README.md` — this file.

## Purpose
This is a **portfolio artifact** meant to demonstrate:
- the CTI lifecycle (collection → analysis → dissemination),  
- ATT&CK-mapped TTPs,  
- sample **Sigma detection rules** and how they can be translated to Elastic/Splunk/Sentinel queries,  
- how to validate detections with Atomic Red Team / CALDERA in a lab.

**Note:** All findings are OSINT-based. This is not from any classified or internal telemetry.

## Quick summary (for recruiters / interviewers)
- **Actor:** APT29 (Cozy Bear) — Russian-attributed cyber espionage group.  
- **Focus:** cloud abuse, credential theft, phishing — relevant to UK government, research and critical sectors.  
- **Deliverables:** 2–3 page brief, Sigma rules, recommended mitigations and validation steps.

## How I built this
1. Collected public advisories and vendor writeups (MITRE, NCSC, CISA, vendor blogs).  
2. Mapped observed behaviours to MITRE ATT&CK techniques.  
3. Wrote a short executive summary and a technical appendix for SOC use.  
4. Authored **Sigma rules** and converted them into Elastic/Splunk/Sentinel queries using Uncoder.io.  
5. Outlined lab validation steps (Atomic Red Team, CALDERA).

## How to read / use the brief
- **Executive summary** = single page for leadership.  
- **TTP table + detections** = technical appendix for SOC/IR.  
- **Sigma rules** = portable detection logic; convert to Elastic, Splunk, or Sentinel queries with Uncoder.io and validate in a lab before production.

## Visuals
The brief and appendix include screenshots from Uncoder.io showing:
- Sigma (process_creation) translated into Elastic queries.  
- Sigma (PowerShell ScriptBlock / Event ID 4104) translated into KQL and Splunk queries.  

These visuals demonstrate how Sigma rules can be adapted across multiple SIEM platforms.

## Validation & emulation notes
- Use Atomic Red Team for lightweight technique tests; use CALDERA for higher-level emulation.  
- Always run emulations in an isolated lab — never on production systems.

## Caveats & limitations
- This is a **publicly-sourced portfolio exercise**, not a forensic report from a live engagement.  
- Detection snippets are intentionally simple and need tuning for real environments (to reduce false positives and fit log formats).

## References & further reading
- MITRE ATT&CK — APT29 group page  
- NCSC / CISA advisories (search "APT29")  
- Vendor threat reports (Mandiant, Google Cloud, CrowdStrike, etc.)

## Contact
- **Author:** Tafadzwa Victor Chipere  
- LinkedIn: https://www.linkedin.com/in/tafadzwa-chipere-cissp-ceh-cc-msc-8000351a5/  
- GitHub: https://github.com/TafadzwaVictor

**License:** Personal portfolio item — feel free to review and reuse for non-commercial learning with attribution. Don’t present this as official vendor/government reporting.
