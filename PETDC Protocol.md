# PETDC v1.3.0 — Protocol

**Protocol for the Evaluation of Trust-Dependent Claims**

**Version:** 1.3.0  
**Status:** Stable / Mechanism-Bound / Adversarial  
**Classification:** Epistemic Security Standard

---

## Version Lock Notice

&gt; **This document contains the enforceable rules of PETDC.** If version mismatch detected between Protocol and ReadMe, Protocol rules take precedence.  
&gt; **Temporal Firewall:** Audit initiation locks version. Mid-audit version changes prohibited. Claims evaluated under version active at audit start.

---

## 0. Quick Start

PETDC classifies claims into three types:

- **E-Claim:** Physical occurrence, measurable output
- **A-Claim:** Biological or specific agency/identity
- **N-Claim:** Methodology, experiential account, counterfactual

**Fundamental constraint:** E ≠ A ≠ N. No upward substitution.

**Version 1.3.0 Hardening:** R7 eliminated. Template governance enforced. Self-referential audits require external custody. Gap Inventory publicly registrable.

---

## I. Purpose & Scope

**Function:** Mechanical audit forcing explicit decomposition. Exposes when evidence is insufficient regardless of consensus.

**Explicit Exclusion:** PETDC is epistemic audit only. Action justification, policy decisions, and operational necessity are outside scope. No "action lane."

---

## II. The Trilemma

| Option | Name                      | Requirement                                             |
| ------ | ------------------------- | ------------------------------------------------------- |
| **1**  | **Evidence-Proportional** | D3 OIE/HDE; completed Table B; no substitution          |
| **2**  | **Well-Placed Trust**     | D2 OIE/HDE; completed Table B; asymmetry bounded        |
| **3**  | **Problematic**           | **Everything else—including D0/D1, gaps, substitution** |

**No fourth option. No R7. No action override.**

---

## III. Core Axioms

### 3.1 Universal Decomposition Principle (UDP)

| Component   | Definition                             | Rule                              |
| ----------- | -------------------------------------- | --------------------------------- |
| **E-Claim** | Physical occurrence, measurable output | Verified independently of A and N |
| **A-Claim** | Biological or specific agency/identity | Verified independently of E and N |
| **N-Claim** | Methodology, experiential account      | Verified independently of E and A |

**Fundamental:** E ≠ A ≠ N. **No upward substitution.**

### 3.2 A-Claim Admissibility (v1.3.0)

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

**Mapping Note (v1.3.0):** "Adversarial-Verified" refers to hostile observation without mechanism-bound identity controls (no continuous custody / no identity binding) and is E-only. "Adversarial real-time visual" (3.2) is an admissible A-control when its stated requirements are met and may reach D3.

---

## VI. Table B: Affirmative Construction

| Row | Element                    | Requirement                                                                                                                                                                                                     |
| --- | -------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | **CVD Inventory**          | Mechanism-bound: "This verifies [E/A/N] by [measurement], discriminating from [alternative]"                                                                                                                    |
| 2   | **Discrimination Entropy** | Per-element; alternative family characterized; **required fields:** (a) ≥2 alternative families, (b) fixed vs free variables, (c) independence/collusion assumptions, (d) stopping rule for adding alternatives |
| 3   | **OIE/HDE Verification**   | Shadowing Check or Independence Weighting                                                                                                                                                                       |
| 4   | **Asymmetry Assessment**   | VAR/HTR with bounds                                                                                                                                                                                             |
| 5   | **Control Classification** | Per Section V                                                                                                                                                                                                   |
| 6   | **Gap Inventory**          | **Mandatory specificity:** (a) missing control class, (b) specific unexcluded alternative, (c) process model per Section 6.1, (d) why absence matters; **Publicly registrable per Section 6.2**                 |

### 6.1 Gap Inventory Process Models (v1.3.0 Template Governance)

**Approved Templates (exhaustive for v1.3.0):**

- Loss
- Omission
- Fabrication
- Misrouting
- Withholding
- Substitution
- Contamination

**Novel Process Escalation:** If auditor determines existing templates insufficient:

1. Label as N-claim with explicit D-score
2. Escalate to framework maintainer with: (a) mechanism-bound definition, (b) historical precedent, (c) discrimination test from existing templates
3. **Prohibited:** Use of non-template process without escalation = automatic Problematic

### 6.2 Gap Inventory Public Registration (v1.3.0)

**Required for all audits:**

- Timestamped, immutable record of complete Gap Inventory
- Registration before D-score output
- **Prevents:** Mid-audit Gap Inventory modification
- **Enables:** Later re-evaluation when new controls emerge

---

## VII. Structural Enforcement Rules

**Rule 1: Mechanism Binding**
Invalid: "Physical presence verifies agency" absent alternative family. **Mechanical classification as Problematic.**

**Rule 2: A-Claim Substitution Detection (v1.3.0 Procedural)**

IF historical_claim AND A-claim asserted:

- IF CVD_inventory lacks admissible controls (Section 3.2)
- OR IF E-claim pattern implies A-claim without explicit statement

THEN: TRIGGER EWP, A-claim_D-score ← D1, OUTPUT "E-claim substitution"

**Procedural Clause (v1.3.0):** If Table B is being executed, evaluate Rule 2 only after Row 1 and Row 2 are stated. If Row 1 does not cite admissible A-controls (3.2), output D1 with Section 10.2 required gap phrasing.

**Rule 3: Consensus Exclusion**
Academic/media consensus: **zero weight.**

**Rule 4: Audit ≠ OIE (v1.3.0 Conditional)**

External audit receives max 0.5 credit **unless** it meets the Hostile-Archive Checklist. If met, classify per Section V.

**Hostile-Archive Checklist (v1.3.0):**

1. ≥3 independent custodians with adversarial incentives
2. No single stakeholder can alter all copies
3. Integrity verification exists (hash chain / notarization / public ledger / independent replication)
4. Hostile access is plausible and evidenced by attempts or capability
5. Custody continuous across relevant interval

**Rule 5: Gap Pattern Flag (v1.3.0)**

IF "comparables preserve CVD" AND "target operation lacks CVD," THEN:

1. REQUIRE Table B Row 2 and Row 6 completion for missing CVD element prior to any downgrade decision
2. OUTPUT must be "specific gap: [missing control] → [unexcluded alternative]" (Section 10.2)
3. **Prohibited:** "Patterned destruction" or process-attribution unless "destruction" is explicitly treated as N-claim with its own Table B + D-score

**Rule 6: Temporal Firewall**

Real-time: verification ≤ claim time + 24hrs.

**Grace Clause (v1.3.0):** If independent custody begins within 24h and remains continuous, verification completing after 24h may still count as real-time for that custody element.

**Framework Temporal Firewall (v1.3.0):** Audit initiation locks version. Mid-audit version changes prohibited. Claims evaluated under version active at audit start.

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

**Rule 9: Removed (v1.3.0)**
See Rule 5.

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

## IX. R-Codes (v1.3.0 Revised)

| Code   | Use                        | Restriction                   |
| ------ | -------------------------- | ----------------------------- |
| **R1** | Alternative CVD            | Must satisfy Rule 1           |
| **R2** | E ≡ A                      | Logical identity required     |
| **R3** | Prior declared             | Explicit P(H)                 |
| **R4** | Threshold dispute          | Matrix excluded               |
| **R5** | Destruction challenged     | Documentary evidence          |
| **R6** | Logical impossibility only | Unfalsifiable by construction |
| ~~R7~~ | ~~Operational necessity~~  | **REMOVED v1.3.0**            |

**R7 Elimination Rationale (v1.3.0):** Created fourth option violating Trilemma. Enabled action-without-certification. Contradicted "no D-score negotiation." All R7 functions now outside PETDC scope.

---

## X. LLM/Auditor Enforcement Protocol

### 10.1 Version Anchoring (Mandatory)

INITIATION CHECKLIST:

- [ ] Framework version explicit (v1.3.0)
- [ ] Rules 1-8 visible
- [ ] A-claim admissibility stated (Section 3.2)
- [ ] Control classification table included
- [ ] **D1 = insufficient evidence** acknowledged
- [ ] **R7 removed** acknowledged
- [ ] **Self-referential audit protocol** acknowledged (10.4)

**Absent any → Default Problematic until explicit**

### 10.2 Prohibited Outputs

| Prohibited                 | Required                                                     |
| -------------------------- | ------------------------------------------------------------ |
| "D1 is expected"           | "D1 indicates insufficient evidence"                         |
| "not evidentiary weakness" | "evidence is weak under stated controls"                     |
| "structural limitation"    | "specific gap: [missing control] → [unexcluded alternative]" |
| "depending on..."          | "Rule X prohibits; Problematic"                              |
| "weak-but-relevant"        | "Rule 7: E-only; no A-claim credit"                          |
| "likely" / "probably"      | D-score only; Bayesian language prohibited                   |

### 10.3 Self-Audit (Pre-Output)

VERIFY:

- [ ] No D-score negotiation
- [ ] No apologetic framing for D1
- [ ] Gap Inventory specifies unexcluded alternatives
- [ ] A-claim ceiling enforced as insufficient evidence
- [ ] **Gap Inventory registered per 6.2**
- [ ] **Declared degrees of freedom explicit (Row 2 + Row 4)**

**FAIL ANY → Output Problematic with explicit Rule citation**

### 10.4 Self-Referential Audit Protocol (v1.3.0)

When PETDC audits itself (framework evaluation, version update, efficacy claim):

**Required:**

- All N-claims explicitly labeled with D1 default
- N-claims prohibited from driving E-claim or A-claim outputs
- **External custody required:** Another auditor, different training, adversarial review
- Self-certifying audits without external custody = automatic Problematic

---

## XI. Final Notes

**PETDC exposes evidence weakness regardless of institutional consensus.**

**No escape.** No Withheld. No negotiation. **No action lane.**

---

_"E ≠ A ≠ N. Signals ≠ Identity. No negotiation. No R7."_

**End of Protocol**

---

**Document Control:**

- Protocol Version: 1.3.0
- Repository: github.com/here-comes-everybody/PETDC
- License: Apache License 2.0
- Gap Inventory Registration: [procedure TBD per implementation]
