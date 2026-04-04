# Auracelle Orion v4 · Public Use Demo

**Cyber Governance Wargaming Simulation**  
Auracelle AI Governance Labs · E-AGPO-HT v2.0 Framework

---

## Overview

Auracelle Orion is a turn-based cyber governance wargaming simulation that stress-tests policy decisions across realistic supply chain and nuclear cybersecurity attack scenarios. Each 5-turn scenario compresses a full incident lifecycle — from initial threat entry through governance consolidation — into a structured decision environment that quantifies the quality of governance choices using the **Evans-Accelerated Governance Policy Optimization-Hierarchical Theory (E-AGPO-HT) v2.0** framework.

This repository hosts the public use demonstration edition of Auracelle Orion, available for exploration by practitioners, researchers, and policymakers working on cyber governance, critical infrastructure protection, and nuclear security.

**Live Demo:** [https://auracelle.github.io/Auracelle-Orion-Public-Use-Demo/](https://auracelle.github.io/Auracelle-Orion-Public-Use-Demo/)

---

## Scenarios

### AI Cybersecurity Domain

| Scenario | Class | Primary Stressors | λ Coupling |
|---|---|---|---|
| **MIRAGE CHAIN** | SolarWinds-class | SC-SBOM · SC-CONC · IFD/SWD | 0.15 |
| **IRONCLAD SIEGE** | Industroyer-class | SC-GREY · HW-PROV · SC-PATCH | 0.10 |
| **FRACTURE POINT** | XZ Utils-class | SC-SBOM · Q_coord · DEP-TRST | 0.05 |
| **PHANTOM CIRCUIT** | Nation-state implant | SC-GREY · HW-BOM · Attribution | 0.20 |

### Nuclear Cybersecurity Domain

| Scenario | Class | Primary Stressors | λ Coupling |
|---|---|---|---|
| **SAFEGUARD ZERO** | IAEA Safeguards-class | NUC-VERIFY · IFD-SCADA · IAEA-COORD | 0.25 |
| **FISSION GATE** | Stuxnet-class | NUC-CTRL · SC-GREY · OT-ENRICH | 0.20 |
| **YELLOWCAKE RUN** | Supply-chain mineral attack | SC-PROVENANCE · IAEA-ITDB · CHAIN-AUTH | 0.18 |

---

## How to Play

**Select a scenario** from the left panel. Each scenario begins with a severity briefing and propagation chain showing the attack vector.

**Intel Phase** — Before deciding, spend up to 3 intelligence tokens (left panel) to reveal hidden observables. Token types:
- 🔍 **Technical Observable** — reveals τ_bridge degradation, SBOM gaps, or component provenance scores
- 📡 **Adversarial Signal** — reveals adversary π_A confidence and attack timing
- ⬡ **Governance Quality** — reveals which Ψ_v2 component is most at risk

**Decision Phase** — Choose one of 4 governance response options. Each option shows explicit trade-off tags (positive, negative, neutral) and updates all domain scores.

**Consequence Phase** — Review the impact on IFD, SWD, SCTL, and GOV domains. Cascade alerts fire if the g-GCC threshold is approached. The counterfactual shows the cost of the path not taken.

**After-Action Review** — Full Ψ_v2 breakdown and decision history. Win threshold: Ψ_v2 ≥ 0.50.

**Governance Artifact Upload** — Upload your organisation's SOPs, IR plans, tabletop reports, or SOC documentation to stress-test them against the E-AGPO-HT framework.

---

## Scoring Framework

### Master g-GCC (Governance Cascade Coefficient)

```
g-GCC = w_IFD·IFD + w_SWD·SWD + w_SC·SCTL + λ·IFD·SWD
```

The λ nonlinear coupling term activates cross-domain amplification — when two domains are simultaneously stressed, their combined effect exceeds the sum of parts.

### Decision Quality Score Ψ_v2

```
Ψ_v2 = 0.30·Q_timing + 0.25·Q_coord + 0.15·Q_norm + 0.20·Q_sctl + 0.10·Q_acc + 0.05·Q_domain_sep
```

| Component | Weight | Description |
|---|---|---|
| Q_timing | 0.30 | Speed and appropriateness of initial response |
| Q_coord | 0.25 | Allied and institutional coordination quality |
| Q_norm | 0.15 | Regulatory and normative compliance |
| Q_sctl | 0.20 | Supply chain trust layer restoration |
| Q_acc | 0.10 | Attribution and accountability |
| Q_domain_sep | 0.05 | IFD/SWD domain separation bonus |

---

## Regulatory Frameworks Modelled

- **EO 14028** — US Executive Order on Improving the Nation's Cybersecurity (SBOM delivery)
- **NIS2 Directive** — EU 72-hour incident notification obligation
- **CISA KEV** — Known Exploited Vulnerabilities catalog patch SLA
- **EU Cyber Resilience Act** — Vendor SBOM and vulnerability disclosure obligations
- **IAEA Comprehensive Safeguards Agreement** — Nuclear material accountancy and notification
- **IAEA Additional Protocol** — Enhanced safeguards verification measures
- **Convention on Physical Protection of Nuclear Material (CPPNM)** — Nuclear transport security
- **NPT** — Non-Proliferation Treaty normative framework

---

## About Auracelle Orion

Auracelle Orion is the **cybersecurity governance platform** within the Auracelle suite. It is domain-portable — the underlying E-AGPO-HT governance function applies across any frontier technology domain (AI, Nuclear, Space, Biotech, Energy, Quantum). The platform's cybersecurity governance function remains constant; what changes is the domain subject matter being stress-tested.

Auracelle Orion is distinct from **Auracelle Lyra**, which applies a verification, validation, and audit governance function across the same frontier domains.

---

## Intellectual Property

© 2013–2026 Grace-Alice Evans · Auracelle AI Governance Labs  
All rights reserved. Proprietary simulation framework — E-AGPO-HT v2.0.

The Evans-Accelerated Governance Policy Optimization-Hierarchical Theory (E-AGPO-HT) is proprietary intellectual property of Grace-Alice Evans and Auracelle AI Governance Labs. This public demo is made available for evaluation and educational purposes only. Reproduction, adaptation, or commercial use of the framework, scenario architecture, scoring methodology, or simulation mechanics requires written authorisation from Auracelle AI Governance Labs.

**Affiliations:**  
UC Berkeley Center for Long-Term Cybersecurity (CLTC) · Non-Resident Senior Fellow  
NATO STO SAS-219 · Technical Role Member  
Bath Spa University · Doctoral Candidate

---

## Contact

**Grace-Alice Evans**  
Founder & Principal Investigator, Auracelle AI Governance Labs  
Non-Resident Senior Fellow, UC Berkeley CLTC  
Technical Role Member, NATO STO SAS-219  

[Auracelle AI Governance Labs](https://auracelle.github.io)
