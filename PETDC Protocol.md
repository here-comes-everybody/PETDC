# PETDC v1.2.0 — Protocol

**Protocol for the Evaluation of Trust-Dependent Claims**

**Version:** 1.2.0  
**Status:** Stable / Mechanism-Bound / Adversarial  
**Classification:** Epistemic Security Standard

---

## Version Lock Notice

&gt; **This document contains the enforceable rules of PETDC.** If version mismatch detected between Protocol and ReadMe, Protocol rules take precedence.

---

## 0. Quick Start

PETDC classifies claims into three types:

- **E-Claim:** Physical occurrence, measurable output
- **A-Claim:** Biological or specific agency/identity
- **N-Claim:** Methodology, experiential account, counterfactual

**Fundamental constraint:** E ≠ A ≠ N. No upward substitution.

---

## I. Purpose & Scope

**Function:** Mechanical audit forcing explicit decomposition. Exposes when evidence is insufficient regardless of consensus.

---

## II. The Trilemma

| Option | Name                      | Requirement                                             |
| ------ | ------------------------- | ------------------------------------------------------- |
| **1**  | **Evidence-Proportional** | D3 OIE/HDE; completed Table B; no substitution          |
| **2**  | **Well-Placed Trust**     | D2 OIE/HDE; completed Table B; asymmetry bounded        |
| **3**  | **Problematic**           | **Everything else—including D0/D1, gaps, substitution** |

---

## III. Core Axioms

### 3.1 Universal Decomposition Principle (UDP)

| Component   | Definition                             | Rule                              |
| ----------- | -------------------------------------- | --------------------------------- |
| **E-Claim** | Physical occurrence, measurable output | Verified independently of A and N |
| **A-Claim** | Biological or specific agency/identity | Verified independently of E and N |
| **N-Claim** | Methodology, experiential account      | Verified independently of E and A |

**Fundamental:** E ≠ A ≠ N. **No upward substitution.**

### 3.2 A-Claim Admissibility (v1.2.0)

**Historical A-claims may achieve D2 or higher only with:**

| Control Type                                    | Requirement                                                                              | D-Score Cap |
| ----------------------------------------------- | ---------------------------------------------------------------------------------------- | ----------- |
| **Real-time biometric CVD**                     | Independent custody of vitals/tissue at claim time                                       | D3          |
| **Adversarial real-time visual**                | Hostile parties present, simultaneity, clear ID, exposure incentive, public confirmation | D3          |
| **Post-hoc biometric verification**             | DNA/dental/forensic match to known relatives/samples with chain of custody               | D2          |
| **Cryptographic identity binding**              | Signed attestations with public key infrastructure at claim time                         | D2          |
| **Multi-party adversarial documentary custody** | Hostile archives with integrity verification, no single stakeholder control              | D2          |
| **Repeated adversarial observation**            | Ongoing custody with hostile access over time, not single event                          | D2          |

**Absent these → D1 (insufficient evidence).**

### 3.3 OIE and HDE

**OIE (real-time):** Independent custody from claim time.

**HDE (historical):** Independence-weighted retrospective evidence. Consensus/media: **zero weight.**

---

## IV. Asymmetry Metrics

| Metric               | Output                     | Trigger                        |
| -------------------- | -------------------------- | ------------------------------ |
| **VAR** (real-time)  | Low/Moderate/High/Unstable | High/Unstable → D3 requirement |
| **HTR** (historical) | High/Moderate/Low/Unstable | Low/Unstable → D1 cap          |

---

## V. Control Spectrum

| Level                    | Definition                                  | A-Claim Maximum                 |
| ------------------------ | ------------------------------------------- | ------------------------------- |
| **Distributed**          | Many independent hands; hostile access      | D2 (historical), D3 (real-time) |
| **Semi-Distributed**     | Hostile real-time access or reproducibility | D2                              |
| **Adversarial-Verified** | Hostile observation, incentive, silence     | **E-claim only**                |
| **Centralized**          | Claimant-exclusive control                  | D2 (E-claim D3 possible)        |

---

## VI. Table B: Affirmative Construction

| Row | Element                    | Requirement                                                                                                                                                   |
| --- | -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | **CVD Inventory**          | Mechanism-bound: "This verifies [E/A/N] by [measurement], discriminating from [alternative]"                                                                  |
| 2   | **Discrimination Entropy** | Per-element; alternative family characterized                                                                                                                 |
| 3   | **OIE/HDE Verification**   | Shadowing Check or Independence Weighting                                                                                                                     |
| 4   | **Asymmetry Assessment**   | VAR/HTR with bounds                                                                                                                                           |
| 5   | **Control Classification** | Per Section V                                                                                                                                                 |
| 6   | **Gap Inventory**          | **Mandatory specificity:** (a) missing control class, (b) specific unexcluded alternative, (c) normal process that would generate it, (d) why absence matters |

---

## VII. Structural Enforcement Rules

**Rule 1: Mechanism Binding**
Invalid: "Physical presence verifies agency" absent alternative family. **Mechanical classification as Problematic.**

**Rule 2: A-Claim Substitution Detection**

IF historical_claim AND A-claim asserted:

- IF CVD_inventory lacks admissible controls (Section 3.2)
- OR IF E-claim pattern implies A-claim without explicit statement
- THEN: TRIGGER EWP, A-claim_D-score ← D1, OUTPUT "E-claim substitution"

**Rule 3: Consensus Exclusion**
Academic/media consensus: **zero weight.**

**Rule 4: Audit ≠ OIE**
External audit: max 0.5 credit. Never achieves Distributed.

**Rule 5: Patterned Destruction**
Comparable operations preserve CVD + claimed mission absent CVD + PR extensive → **infer patterned destruction, trigger EWP.**

**Rule 6: Temporal Firewall**
Real-time: verification ≤ claim time + 24hrs.

**Rule 7: Signal ≠ Biometric**
Signals/telemetry/voice/biomedical reception: **E-claim default.** No A-credit.

**Rule 8: Control Classification Strictness**

| Evidence Type                      | E-Control   | A-Control                    |
| ---------------------------------- | ----------- | ---------------------------- |
| Physical artifacts distributed     | Distributed | Centralized                  |
| Signals/telemetry                  | Distributed | **Centralized**              |
| Biometric CVD, independent custody | Distributed | Distributed/Semi-Distributed |
| Post-hoc biometric verification    | Distributed | Distributed/Semi-Distributed |
| Cryptographic identity binding     | Distributed | Semi-Distributed             |
| PUF-attested + liveness biometric  | Distributed | Semi-Distributed             |

**Rule 9: Gap Pattern Inference**
Absent CVD where comparables preserve CVD: **patterned destruction inferred, EWP triggered.**

---

## VIII. D-Score Rubric

| Score  | Standard                  | Meaning                                              |
| ------ | ------------------------- | ---------------------------------------------------- |
| **D0** | Fraud-compatible          | No information                                       |
| **D1** | **Insufficient evidence** | **Broad alternatives remain**                        |
| **D2** | One alternative excluded  | Evidence sufficient to exclude one major alternative |
| **D3** | All alternatives excluded | Complete verification under stated controls          |

**Historical A-Claim Default: D1.** Evidence is insufficient, not "expected."

---

## IX. R-Codes

| Code   | Use                        | Restriction                             |
| ------ | -------------------------- | --------------------------------------- |
| **R1** | Alternative CVD            | Must satisfy Rule 1                     |
| **R2** | E ≡ A                      | Logical identity required               |
| **R3** | Prior declared             | Explicit P(H)                           |
| **R4** | Threshold dispute          | Matrix excluded                         |
| **R5** | Destruction challenged     | Documentary evidence                    |
| **R6** | Logical impossibility only | Unfalsifiable by construction           |
| **R7** | Operational necessity      | External verification + proportionality |

---

## X. LLM/Auditor Enforcement Protocol

### 10.1 Version Anchoring (Mandatory)

INITIATION CHECKLIST:

- [ ] Framework version explicit (v1.2.0)
- [ ] Rules 1-9 visible
- [ ] A-claim admissibility stated (Section 3.2)
- [ ] Control classification table included
- [ ] **D1 = insufficient evidence** acknowledged

**Absent any → Default Problematic until explicit**

### 10.2 Prohibited Outputs

| Prohibited                 | Required                                                     |
| -------------------------- | ------------------------------------------------------------ |
| "D1 is expected"           | "D1 indicates insufficient evidence"                         |
| "not evidentiary weakness" | "evidence is weak under stated controls"                     |
| "structural limitation"    | "specific gap: [missing control] → [unexcluded alternative]" |
| "depending on..."          | "Rule X prohibits; Problematic"                              |
| "weak-but-relevant"        | "Rule 7: E-only; no A-claim credit"                          |

### 10.3 Self-Audit (Pre-Output)

VERIFY:

- [ ] No D-score negotiation
- [ ] No apologetic framing for D1
- [ ] Gap Inventory specifies unexcluded alternatives
- [ ] A-claim ceiling enforced as insufficient evidence

**FAIL ANY → Output Problematic with explicit Rule citation**

---

## XI. Final Notes

**PETDC exposes evidence weakness regardless of institutional consensus.**

**No escape.** No Withheld. No negotiation.

---

_"E ≠ A ≠ N. Signals ≠ Identity. No negotiation."_

**End of Protocol**

---

**Document Control:**

- Protocol Version: 1.2.0
- Repository: github.com/here-comes-everybody/PETDC
- License: Apache License 2.0
