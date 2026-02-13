# PETDC v1.1.0 — Protocol

**Protocol for the Evaluation of Trust-Dependent Claims**

**Version:** 1.1.0 (Refined)  
**Status:** Stable / Mechanism-Bound / Adversarial  
**Classification:** Epistemic Security Standard

---

## Version Lock Notice

&gt; **This document contains the enforceable rules of PETDC.** If version mismatch detected between Protocol and ReadMe, Protocol rules take precedence.

&gt; **v1.1.0 Changes:** Tightened Rule 2 criteria, softened Rule 3 consensus treatment, added implicature guard, clarified calibration purpose, added brittleness warning. No new rules added—existing rules refined.

---

## 0. Quick Start

PETDC classifies claims into three types:

- **E-Claim:** Physical occurrence, measurable output
- **A-Claim:** Biological or specific agency/identity
- **N-Claim:** Methodology, experiential account, counterfactual

**Fundamental constraint:** E ≠ A ≠ N. No upward substitution.

**Output:** D-score (D0-D3) and Trilemma classification.

---

## I. Purpose & Scope

**Function:** Mechanical audit forcing explicit decomposition. Non-negotiable in adversarial contexts.

**Core Design Principle:** PETDC is intentionally harsh to prevent E→A substitution. It will classify many historically-important A-claims as D1/Problematic. This is expected behavior, not failure.

**Warning:** PETDC produces mechanically correct but potentially unhelpful outputs. Users may abandon or weaponize results. See ReadMe Section X for mitigation.

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

### 3.2 A-Claim Ceiling

**Historical claims:** Maximum D-score = D2. **Default: D1.**

**D3 A-claim requires:** Real-time biometric CVD with independent custody, OR adversarial real-time visual observation meeting all criteria (hostile parties, simultaneity, clear ID, exposure incentive, public confirmation).

**Absent these → D1 default.** This is expected and correct.

### 3.3 OIE and HDE

**OIE (real-time):** Independent custody from claim time.

**HDE (historical):** Independence-weighted retrospective evidence.

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

| Row | Element                    | Requirement                                                                                  |
| --- | -------------------------- | -------------------------------------------------------------------------------------------- |
| 1   | **CVD Inventory**          | Mechanism-bound: "This verifies [E/A/N] by [measurement], discriminating from [alternative]" |
| 2   | **Discrimination Entropy** | Per-element; alternative family characterized                                                |
| 3   | **OIE/HDE Verification**   | Shadowing Check or Independence Weighting                                                    |
| 4   | **Asymmetry Assessment**   | VAR/HTR with bounds                                                                          |
| 5   | **Control Classification** | Per Section V                                                                                |
| 6   | **Gap Inventory**          | Explicit status; causation; patterned destruction                                            |

---

## VII. Structural Enforcement Rules

**Rule 1: Mechanism Binding**
Invalid: "Physical presence verifies agency" absent alternative family. **Mechanical classification as Problematic.**

**Rule 2: A-Claim Substitution Detection (Tightened v1.1.0)**

IF historical_claim AND A-claim asserted:

- IF CVD_inventory contains ONLY (artifacts, signals, imaging, testimony) without **adversarial multi-party custody** (hostile parties with economic incentive to expose, independent retention, cryptographic or physical integrity verification)
- AND NO (biometric CVD, adversarial visual observation, PUF-enhanced control)
- **OR IF** E-claim pattern density implies A-claim without explicit statement (implicature smuggling detected)
- THEN: TRIGGER EWP, A-claim_D-score ← D1, OUTPUT "E-claim substitution"

**Rule 3: Consensus Treatment (Softened v1.1.0)**

Academic/media consensus: **non-decisive weight only.**

Consensus counts only if:

- Diverse independent methods converge
- Adversarial scrutiny present (parties with incentive to disprove remained silent or confirmed)
- No evidence of coordination or information cascade

Otherwise: consensus weight → 0 for that claim.

**Rule 4: Audit ≠ OIE**
External audit: max 0.5 credit. Never achieves Distributed.

**Rule 5: Patterned Destruction**
Comparable operations preserve CVD + claimed mission absent CVD + PR extensive → **infer patterned destruction, trigger EWP.**

**Rule 6: Temporal Firewall**
Real-time: verification ≤ claim time + 24hrs.

**Rule 7: Signal ≠ Biometric (Refined v1.1.0)**

Signals/telemetry/voice/biomedical reception: **E-claim default.**

**Exception:** Cryptographically authenticated, hostile-party-captured signals with time-locked commitments and cross-validation may receive **E-claim enhanced weight** (not A-claim credit).

**Rule 8: Control Classification Strictness**

| Evidence Type                      | E-Control   | A-Control                    |
| ---------------------------------- | ----------- | ---------------------------- |
| Physical artifacts distributed     | Distributed | Centralized                  |
| Signals/telemetry                  | Distributed | **Centralized**              |
| Biometric CVD, independent custody | Distributed | Distributed/Semi-Distributed |
| PUF-attested + liveness biometric  | Distributed | Semi-Distributed             |

**Rule 9: Gap Pattern Inference**
Absent CVD where comparables preserve CVD: **patterned destruction inferred, EWP triggered.**

---

## VIII. D-Score Rubric

| Score  | Standard                  | Historical A-Claim             |
| ------ | ------------------------- | ------------------------------ |
| **D0** | Fraud-compatible          | Default if no information      |
| **D1** | Broad alternatives        | **Default historical A-claim** |
| **D2** | One alternative excluded  | Maximum historical A-claim     |
| **D3** | All alternatives excluded | Real-time biometric only       |

**Interpretation:** D1 is expected and correct for historical A-claims. It indicates structural uncertifiability under PETDC controls, not evidentiary weakness.

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

- [ ] Framework version explicit (v1.1.0)
- [ ] Rule set visible (1-9)
- [ ] A-claim admissibility stated
- [ ] Control classification table included
- [ ] "D1 default is expected" acknowledged

**Absent any → Default Problematic until explicit**

### 10.2 Prohibited Outputs

| Prohibited               | Required                                 |
| ------------------------ | ---------------------------------------- |
| "Depending on..."        | "Rule X prohibits; Problematic"          |
| "Weak-but-relevant"      | "Rule 7: E-only; no A-claim credit"      |
| "If you want to push..." | "A-claim ceiling D1; no D2+ path"        |
| "Not suspicious"         | "Rule 9: Patterned destruction inferred" |

### 10.3 Self-Audit (Pre-Output)

VERIFY:

- [ ] No D-score negotiation
- [ ] No partial credit for signals
- [ ] Control classification table-matched
- [ ] Gap pattern Rule 9 applied
- [ ] A-claim ceiling enforced
- [ ] Rule 2 implicature check completed

**FAIL ANY → Output Problematic with explicit Rule citation**

---

## XI. Calibration Cases (Illustrative Only)

**Warning:** These cases demonstrate rule application patterns. They are **not templates** for template-matching. Each claim requires independent Table B completion.

| Case                  | E   | A      | Label                                  | Key                                    |
| --------------------- | --- | ------ | -------------------------------------- | -------------------------------------- |
| **Apollo**            | D3  | **D1** | Problematic (A), Well-Placed Trust (E) | Rules 7-9; E-substitution              |
| **Holocaust**         | D3  | **D2** | Well-Placed Trust                      | High HTR; no Rule 7 violation          |
| **Theranos**          | D0  | —      | Problematic                            | Centralized; patterned destruction     |
| **Tobacco (A-claim)** | D2  | **D1** | Problematic                            | Rule 2; adversarial documentary limits |

**Do not match claims to table. Apply rules mechanically.**

---

## XII. Key Distinctions

### 12.1 Threshold Cryptography vs. Human Identity

| Aspect  | Key Control           | Human Identity               |
| ------- | --------------------- | ---------------------------- |
| CVD     | HSM attestation       | Biometric telemetry          |
| D3 path | Independent audit     | Real-time biometric custody  |
| Type    | E-claim with policy   | Biological agency            |
| Label   | Evidence-Proportional | **Problematic (historical)** |

### 12.2 Signal Confusion (Rule 7)

Bochum reception of Apollo biomedical signals:

- Verifies **E:** Transmission occurred
- **A-claim: Nothing.** Source could be recording, relay, simulation

**No A-claim credit.**

---

## XIII. Final Notes

**PETDC is adversarially rigorous to institutional comfort.** It exposes:

- E-claim substitution for A-claims (Rules 2, 7)
- Audit substitution for OIE (Rule 4)
- Consensus over-reliance (Rule 3)
- Patterned destruction (Rules 5, 9)
- Historical unearned D3 status (A-claim ceiling)

**No escape.** No Withheld. No negotiation. Table B completes or fails; standards unmet → Problematic.

**Brittleness Warning:** PETDC produces mechanically correct outputs that may be unhelpful or weaponized. See ReadMe Section X for responsible use.

**Apollo paradigm:** Independent signal reception ≠ human identity verification. Distributed artifacts ≠ centralized identity control. **A-claim default: D1 (Problematic).**

---

_"E ≠ A ≠ N. Signals ≠ Identity. No negotiation. Show your work, or accept the default."_

**End of Protocol**

---

**Document Control:**

- Protocol Version: 1.1.0
- Repository: github.com/here-comes-everybody/PETDC
- License: Apache License 2.0
