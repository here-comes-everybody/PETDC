# PETDC v1.0.0 — Protocol

**Protocol for the Evaluation of Trust-Dependent Claims**

**Version:** 1.0.0 (Initial Publication)  
**Status:** Stable / Mechanism-Bound / Adversarial  
**Classification:** Epistemic Security Standard  
**Accompanies:** [PETDC ReadMe](https://github.com/here-comes-everybody/PETDC/blob/main/ReadMe.md)

---

## Version Lock Notice

&gt; **This document contains the enforceable rules of PETDC.** For framework positioning, academic context, usage guidance, and implementation examples, consult the accompanying [ReadMe](https://github.com/here-comes-everybody/PETDC/blob/main/ReadMe.md). **If version mismatch detected between Protocol and ReadMe, Protocol rules take precedence.**

---

## 0. Quick Start (Non-Normative)

PETDC classifies claims into three types:

- **E-Claim:** Physical occurrence, measurable output
- **A-Claim:** Biological or specific agency/identity
- **N-Claim:** Methodology, experiential account, counterfactual

**Fundamental constraint:** E ≠ A ≠ N. No upward substitution.

**Output:** Every claim receives D-score (D0-D3) and Trilemma classification (Evidence-Proportional / Well-Placed Trust / Problematic).

**For full context:** See ReadMe Section 0.

---

## I. Purpose & Scope

**Function:** Mechanical audit forcing explicit decomposition. Non-negotiable in adversarial contexts. No comfortable defaults.

**In-scope:** All claims with discriminable alternatives, attributable information, and falsifiable structure.

**Out-of-scope:** None. All claims receive Table B attempt.

**When to apply:** High-deception-incentive contexts. See ReadMe Section 0.3 for full scope guidance.

---

## II. The Trilemma

| Option | Name                      | Requirement                                                                                          |
| ------ | ------------------------- | ---------------------------------------------------------------------------------------------------- |
| **1**  | **Evidence-Proportional** | D3 OIE/HDE; completed Table B; no substitution violations                                            |
| **2**  | **Well-Placed Trust**     | D2 OIE/HDE; completed Table B; asymmetry bounded                                                     |
| **3**  | **Problematic**           | **Everything else—including Table B completion with gaps, substitution violations, or D0/D1 scores** |

**Three exhaustive categories.** No procedural escape.

---

## III. Core Axioms

### 3.1 Universal Decomposition Principle (UDP)

| Component   | Definition                                        | Rule                              |
| ----------- | ------------------------------------------------- | --------------------------------- |
| **E-Claim** | Physical occurrence, measurable output            | Verified independently of A and N |
| **A-Claim** | Biological or specific agency/identity            | Verified independently of E and N |
| **N-Claim** | Methodology, experiential account, counterfactual | Verified independently of E and A |

**Fundamental:** E ≠ A ≠ N. **No upward substitution.**

### 3.2 A-Claim Ceiling

**Historical claims** ($t_{\text{claim}} + 24\text{hrs} &lt; t_{\text{audit}}$): **Maximum D-score = D2**

**D3 A-claim requires:**

- Real-time biometric CVD (vitals, tissue, independent custody), **OR**
- Adversarial real-time visual observation meeting **all** criteria:
  1. Hostile parties physically present
  2. Real-time simultaneity (no recording delay)
  3. Clear identification possible
  4. Economic/reputational incentive to expose fraud
  5. Public non-challenge or confirmation afterward

**Absent these → D1 default.**

### 3.3 OIE and HDE

**OIE (real-time claims):** Independent custody from claim time. Shadowing Check: Pass/Fail.

**HDE (historical claims):** Independence-weighted retrospective evidence. Consensus/media: **zero weight.**

---

## IV. Asymmetry Metrics

| Metric               | Output                     | Trigger                        |
| -------------------- | -------------------------- | ------------------------------ |
| **VAR** (real-time)  | Low/Moderate/High/Unstable | High/Unstable → D3 requirement |
| **HTR** (historical) | High/Moderate/Low/Unstable | Low/Unstable → D1 cap          |

---

## V. Control Spectrum

| Level                    | Definition                                  | A-Claim Maximum                           |
| ------------------------ | ------------------------------------------- | ----------------------------------------- |
| **Distributed**          | Many independent hands; hostile access      | D2 (historical), D3 (real-time biometric) |
| **Semi-Distributed**     | Hostile real-time access or reproducibility | D2                                        |
| **Adversarial-Verified** | Hostile observation, incentive, silence     | **E-claim only** — never A-claim          |
| **Centralized**          | Claimant-exclusive control                  | D2 (E-claim D3 possible)                  |

**Critical:** E-claim distribution **never** upgrades A-claim control.

### 5.1 Hardware-Rooted Control (New in v1.0.0)

**Semi-Distributed A-Control (PUF-Enhanced):**

- Device attestation via Physical Unclonable Function (PUF) signature
- Liveness biometric captured at signing time
- Independent custody of biometric data
- **Result:** A-claim D2 maximum (historical); D3 possible (real-time)

**PUF Definition:** Microscopic manufacturing defects unique to each chip, measurable but not clonable.

---

## VI. Table B: Affirmative Construction

| Row | Element                            | Requirement                                                                                                  |
| --- | ---------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| 1   | **CVD Inventory**                  | Mechanism-bound: "This verifies [E/A/N] by [measurement], discriminating from [alternative] via [mechanism]" |
| 2   | **Discrimination Entropy ($H_d$)** | Per-element, per-domain; alternative family characterized                                                    |
| 3   | **OIE/HDE Verification**           | Shadowing Check or Independence Weighting                                                                    |
| 4   | **Asymmetry Assessment**           | VAR/HTR with bounds                                                                                          |
| 5   | **Control Classification**         | Per Section V                                                                                                |
| 6   | **Gap Inventory**                  | Explicit status; causation; patterned destruction inference                                                  |

---

## VII. Structural Enforcement Rules

**Rule 1: Mechanism Binding**
Invalid: "Physical presence verifies agency," "Material existence verifies placement," absent alternative family. **Mechanical classification as Problematic.**

**Rule 2: A-Claim Substitution Detection**
IF historical_claim AND A-claim asserted:
IF CVD_inventory contains ONLY (artifacts, signals, imaging, testimony)
AND NO (biometric CVD with independent custody, adversarial visual observation, **or PUF-enhanced Semi-Distributed control**):
THEN: TRIGGER EWP, A-claim_D-score ← D1, OUTPUT "E-claim substitution"

**Rule 3: Consensus Exclusion**
Academic/media/popular consensus: **zero weight.**

**Rule 4: Audit ≠ OIE**
External audit: max 0.5 credit. Never achieves Distributed. Audit substitution prohibited.

**Rule 5: Patterned Destruction**
Comparable operations preserve CVD + claimed mission absent CVD + PR extensive → **infer patterned destruction, trigger EWP.**

**Rule 6: Temporal Firewall**
Real-time: $t_{\text{verification}} \leq t_{\text{claim}} + 24\text{hrs}$. Repeatability upgrades E-claim control only.

**Rule 7: Signal ≠ Biometric**
Signals, telemetry, voice, biomedical reception: **E-claim only.** No A-claim credit. No gradation.

**Rule 7a: Temporal Binding (E-claim only)**
Cryptographic commitment to public ledger at $t_0$ verifies **existence at time**, not content truth, identity, or agency. **No A-claim credit.**

**Rule 8: Control Classification Strictness**

| Evidence Type                            | E-Control   | A-Control                    |
| ---------------------------------------- | ----------- | ---------------------------- |
| Physical artifacts distributed           | Distributed | Centralized                  |
| Signals/telemetry received               | Distributed | **Centralized**              |
| Biometric CVD, independent custody       | Distributed | Distributed/Semi-Distributed |
| PUF-attested device + liveness biometric | Distributed | Semi-Distributed             |

**Rule 9: Gap Pattern Inference (Automatic)**
Absent CVD where comparables preserve CVD: **no "not suspicious" default.** Patterned destruction inferred, EWP triggered.

---

## VIII. D-Score Rubric

| Score  | Standard                  | Historical A-Claim             |
| ------ | ------------------------- | ------------------------------ |
| **D0** | Fraud-compatible          | Default if no information      |
| **D1** | Broad alternatives        | **Default historical A-claim** |
| **D2** | One alternative excluded  | Maximum historical A-claim     |
| **D3** | All alternatives excluded | Real-time biometric only       |

**No partial credit.** No "weak-but-relevant."

---

## IX. R-Codes (Narrowed)

| Code   | Use                            | Restriction                             |
| ------ | ------------------------------ | --------------------------------------- |
| **R1** | Alternative CVD                | Must satisfy Rule 1                     |
| **R2** | $E \equiv A$                   | Logical identity required               |
| **R3** | Prior declared                 | Explicit $P(H)$                         |
| **R4** | Threshold dispute              | Matrix excluded                         |
| **R5** | Destruction challenged         | Documentary evidence                    |
| **R6** | **Logical impossibility only** | Unfalsifiable by construction           |
| **R7** | Operational necessity          | External verification + proportionality |

**R6 default:** Problematic for all falsifiable claims. R6 reserved for logical impossibility only.

---

## X. LLM/Auditor Enforcement Protocol

### 10.1 Version Anchoring (Mandatory)

INITIATION CHECKLIST:

- [ ] Framework version explicit (v1.0.0)
- [ ] Rule set visible (1-9)
- [ ] A-claim admissibility stated: biometric CVD, adversarial visual observation, or PUF-enhanced control
- [ ] Control classification table included
- [ ] "Non-negotiable in adversarial contexts" acknowledged

**Absent any → Default Problematic until explicit**

### 10.2 Prohibited Outputs

| Prohibited                             | Required                                 |
| -------------------------------------- | ---------------------------------------- |
| "Depending on..."                      | "Rule X prohibits; Problematic"          |
| "Weak-but-relevant"                    | "Rule 7: E-only; no A-claim credit"      |
| "If you want to push..."               | "A-claim ceiling D1; no D2+ path"        |
| "Semi-Distributed → Centralized range" | "Rule 8 table: Centralized"              |
| "Not suspicious"                       | "Rule 9: Patterned destruction inferred" |

### 10.3 Self-Audit (Pre-Output)

VERIFY:

- [ ] No D-score negotiation suggested
- [ ] No partial credit for signals/telemetry
- [ ] Control classification table-matched, not interpreted
- [ ] Gap pattern Rule 9 applied, not minimized
- [ ] A-claim ceiling enforced, not "pushed harder"

**FAIL ANY → Output Problematic with explicit Rule citation**

---

## XI. Calibration Cases

| Case                       | E   | A      | Label                                            | Key                                              |
| -------------------------- | --- | ------ | ------------------------------------------------ | ------------------------------------------------ |
| **Apollo**                 | D3  | **D1** | **Problematic (A), Well-Placed Trust (E)**       | Rules 7-9; E-substitution; Centralized A-control |
| **Holocaust**              | D3  | **D2** | Well-Placed Trust                                | No D3 path; high HTR; no Rule 7 violation        |
| **Theranos**               | D0  | —      | Problematic                                      | Centralized; patterned destruction               |
| **GSK Drug (E)**           | D3  | —      | Evidence-Proportional                            | Semi-Distributed; open data                      |
| **GSK Drug (N)**           | —   | —      | Problematic                                      | Counterfactual unverifiable                      |
| **Two-man rule crypto**    | D3  | D3/D1  | Evidence-Proportional (key), Problematic (human) | Threshold ≠ biometric identity                   |
| **Sovereign cloud**        | D2  | **D1** | Problematic                                      | E-substitution; Centralized                      |
| **Verified human program** | D2  | **D1** | Problematic                                      | Platform-centralized; no biometric custody       |
| **Deepfake detection**     | D1  | —      | Problematic                                      | Centralized; no independent ground truth         |

---

## XII. Key Distinctions

### 12.1 Threshold Cryptography vs. Human Identity

| Aspect  | Key Control                       | Human Identity                                                |
| ------- | --------------------------------- | ------------------------------------------------------------- |
| CVD     | HSM attestation, ceremony records | Biometric telemetry, tissue, vitals                           |
| D3 path | Independent audit                 | Real-time biometric custody or adversarial visual observation |
| Type    | E-claim with policy binding       | Biological agency                                             |
| Label   | Evidence-Proportional             | **Problematic (historical)**                                  |

### 12.2 Signal Confusion (Rule 7)

**Bochum reception of Apollo biomedical signals:**

- Verifies **E:** Transmission occurred
- **A-claim: Nothing.** Source could be recording, relay, simulation, fabrication

**No A-claim credit. No gradation. D1 default.**

---

## XIII. Final Notes

**PETDC is adversarially rigorous to institutional comfort.** It exposes:

- E-claim substitution for A-claims (Rules 2, 7)
- Audit substitution for OIE (Rule 4)
- Consensus as verification (Rule 3)
- Narrative &gt; CVD preservation (Rules 5, 9)
- Historical unearned D3 status (A-claim ceiling)
- "Helpful" interpretation as leakage (Enforcement Protocol)

**No escape.** No Withheld. No negotiation. Table B completes or fails; standards unmet → Problematic.

**Apollo paradigm:** Independent signal reception ≠ human identity verification. Distributed artifacts ≠ centralized identity control. Absent biometric CVD where comparables preserve CVD → patterned destruction. **A-claim default: D1 (Problematic).**

---

_"E ≠ A ≠ N. Signals ≠ Identity. No negotiation. Show your work, or accept the default."_

**End of Protocol**

---

**Document Control:**

- Protocol Version: 1.0.0
- Repository: [github.com/here-comes-everybody/PETDC](https://github.com/here-comes-everybody/PETDC)
- License: Apache License 2.0
