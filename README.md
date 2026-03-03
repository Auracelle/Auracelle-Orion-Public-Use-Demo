# Auracelle Orion v4
### Cyber Governance Wargaming Simulation

**Auracelle AI Governance Labs**  
Grace-Alice Evans — Director & Principal Investigator  
Non-Resident Senior Fellow, UC Berkeley Center for Long-Term Cybersecurity

---

## Overview

Auracelle Orion is a domain-partitioned cyber governance wargaming simulation that stress-tests policy decisions across realistic supply-chain attack scenarios. Each scenario compresses a full incident lifecycle — from initial supply-chain entry through governance consolidation — into a structured decision environment that quantifies the quality of governance choices.

Orion is a product of Auracelle AI Governance Labs. It is designed for national governments, regulatory bodies, critical infrastructure operators, international institutions, and policy research communities who need evidence-based governance analysis, not generic dashboards.

---

## Platform Architecture

Orion operates across three architectural domains:

| Domain | Code | Scope |
|--------|------|-------|
| Infrastructure Domain | IFD | Physical plant, OT/ICS/SCADA, network hardware, power and cooling systems |
| Software Domain | SWD | Application stacks, firmware, cloud-native services, CI/CD pipelines, dependency graphs |
| Supply-Chain Trust Layer | SCTL | Directed trust graph connecting vendors, integrators, and operators across both domains |

The master governance stress scalar integrates both domain subscalars and the Supply-Chain Trust Layer stress index, with a cross-domain coupling term that captures nonlinear amplification when both domains are simultaneously stressed.

---

## Core Capabilities

- **Quantified Governance Scoring** — Every scenario produces a traceable score decomposable to its source composite across both domains
- **Counterfactual Policy Analysis** — Re-run scenarios with different configurations to measure the governance value of specific investments
- **Accelerated Decision-Making** — Domain-partitioned time compression quantifies decision quality under realistic incident pressure
- **Supply-Chain Propagation Modeling** — Models how compromise travels across organizational and sector boundaries via the SCTL
- **Regulatory Alignment Mapping** — Scenario outputs map directly to NIS2, EU CRA, US EO 14028, NERC CIP, CISA KEV, NIST CSF 2.0, OECD Recommendation on AI (2024), and WEF Global Cybersecurity Outlook 2025 frameworks
- **Live Data Integration** — Real-time grounding via World Bank, SIPRI, UN Comtrade, and US Export Controls APIs
- **Artifact Analysis** — Upload governance documents (policies, SBOMs, incident reports) for scored gap analysis against scenario archetypes

---

## Scenario Archetypes

| # | Archetype | Domain Profile | Dominant SCTL Stressor |
|---|-----------|---------------|----------------------|
| 01 | Critical Infrastructure Ransomware | IFD-Dominant | SC-PATCH |
| 02 | Software Supply-Chain Compromise | SWD-Dominant | SC-SBOM + SC-CONC |
| 03 | OT/ICS Targeted Attack | IFD-Dominant | SC-GREY + SC-PATCH |
| 04 | Cloud-Native Dependency Poisoning | SWD-Dominant | SC-SBOM + SC-CONC |
| 05 | Nation-State Hardware Implant Campaign | Cross-Domain | SC-GREY (dominant) |

---

## Platform Metrics

- **57+** governance features scored across three architectural zones
- **3** architectural domains (IFD, SWD, SCTL)
- **5** calibrated scenario archetypes
- **4** live data integrations
- **8** domain-partitioned response stages with independent time acceleration

---

## Regulatory Alignment

Orion scenario scoring maps directly to:

| Framework | Domain Mapping |
|-----------|---------------|
| NIS2 Directive (EU) 2022/2555 | Infrastructure Domain (IFD) — 72-hour notification, incident response |
| EU Cyber Resilience Act | Software Domain (SWD) — product liability, SBOM mandates |
| US Executive Order 14028 | Software Domain (SWD) — SBOM disclosure, federal software supply chain |
| NERC CIP | Infrastructure Domain (IFD) — critical infrastructure protection |
| CISA KEV Catalog | SCTL — SC-PATCH temporal stressor, mandatory 14-day patch SLA |
| Budapest Convention (Supply Chain Provisions) | SCTL — cross-border propagation, multilateral incident coordination |
| NIST CSF 2.0 · GV.SC | SCTL + both domains — Cybersecurity Supply Chain Risk Management governance function |
| OECD Recommendation of the Council on AI (2024) | Cross-domain — AI governance interoperability, safety, and risk management |
| WEF Global Cybersecurity Outlook 2025 | Cross-domain — supply chain interdependency resilience, geopolitical risk framing |

---

## Intended Users

- **National Governments & Regulators** — Assess readiness, justify policy investments, map to regulatory exposure
- **International Institutions** — Common simulation framework for multilateral crisis exercises
- **Critical Infrastructure Operators** — Identify governance investments that change outcomes under specific threat profiles
- **Defense & Intelligence Communities** — Stress-test frameworks against adversarial supply-chain and hardware implant scenarios
- **Academic & Policy Research** — Research-grade tool with Bayesian uncertainty reporting and full feature decomposition
- **Civil Society & Standards Bodies** — Evaluate how governance decisions affect public interest outcomes

---

## Getting Started

This repository publishes the Auracelle Orion simulation interface via GitHub Pages.

**To run locally:**
1. Clone or download this repository
2. Open `index.html` in any modern browser
3. No build step, server, or dependencies required — the simulation runs entirely client-side

**Live demo:**  
`https://[your-username].github.io/auracelle-orion`  
*(Update this URL after enabling GitHub Pages in repository Settings)*

---

## About Auracelle AI Governance Labs

Auracelle AI Governance Labs is an independent AI governance research institution. Orion was developed through independent synthesis of authoritative governance literature and over 20 years of practitioner experience across defense, intelligence, and critical infrastructure organizations including CIA, DHS, Army Intelligence and Security Command, San Francisco International Airport, and Maryland Department of Transportation.

Academic grounding provided through doctoral research in AI Governance Policy Optimization at Bath Spa University.

Engaged with NATO, UN agencies, OECD, WEF, and NIST governance communities.

---

## Intellectual Property Notice

The mathematical architecture, domain-partition methodology, scoring framework, governance feature taxonomy, and scenario design of Auracelle Orion constitute proprietary intellectual capital (IC) and intellectual property (IP) of Grace-Alice Evans and Auracelle AI Governance Labs.

This simulation interface is made available for institutional review and demonstration purposes. The underlying proprietary framework is withheld from public release.

**© 2026 Grace-Alice Evans · Auracelle AI Governance Labs · All Rights Reserved**  
Unauthorized reproduction, adaptation, or commercialization of any element of this work is prohibited.

---

*For institutional inquiries, partnership proposals, or demonstration requests, please contact Auracelle AI Governance Labs.*
