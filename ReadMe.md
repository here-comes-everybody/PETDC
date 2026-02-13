# PETDC — Protocol for Evaluation of Trust-Dependent Claims

**Version:** 1.2.0  
**Status:** Stable / Mechanism-Bound / Adversarial  
**License:** Apache License 2.0

---

## 0. What is PETDC?

PETDC is a **mechanical audit framework** that forces explicit decomposition of claims into three non-substitutable types:

- **E-Claims:** Physical events, measurable outputs
- **A-Claims:** Biological identity, specific agency, intent
- **N-Claims:** Methodology, experiential accounts, counterfactuals

**Core principle:** E ≠ A ≠ N. No upward substitution.

**Core function:** Expose when evidence is insufficient, regardless of consensus.

---

## 0.1 When to Use PETDC

**Use when:**

- High deception incentive exists
- Attribution risk is present (accusations, defamation, scapegoating)
- False certainty about intent is costly
- Adversarial scrutiny expected

**PETDC is harsh.** It will classify many claims as D1/Problematic. This indicates **insufficient evidence**, not "expected outcome."

---

## 0.2 Quick Example

**Claim:** "The tobacco industry knowingly misled the public."

**PETDC decomposition:**

- **E-Claim:** "Companies issued public statements Y at time T" → D2 (verifiable)
- **A-Claim:** "They knowingly misled" → **D1/Problematic (insufficient evidence)**

**Why:** Historical A-claims default to D1 when admissibility criteria unmet. Documents/testimony cannot certify intent.

---

## 0.3 What PETDC Does Not Do

**PETDC does not:**

- Evaluate "truth" in the historical sense
- Provide comfortable answers
- Allow consensus to substitute for evidence
- Permit E-evidence to certify A-claims
- Apologize for D1 classifications

**PETDC does:**

- Force explicit claim typing
- Prevent substitution fallacies
- Make uncertainty granular and explicit
- Expose evidence weakness

---

## I. Core Concepts

### I.1 The Trilemma

Every claim must be classified as:

1. **Evidence-Proportional** (D3, no violations)
2. **Well-Placed Trust** (D2, bounded asymmetry)
3. **Problematic** (everything else—including D0/D1)

**No fourth option.**

### I.2 D-Scores

| Score  | Meaning                                              |
| ------ | ---------------------------------------------------- |
| D0     | Fraud-compatible                                     |
| **D1** | **Insufficient evidence; broad alternatives remain** |
| D2     | One alternative excluded                             |
| D3     | All alternatives excluded                            |

**Critical:** D1 indicates **audit failure**, not "expected outcome."

### I.3 A-Claim Admissibility (v1.2.0)

Historical A-claims may achieve D2+ with:

- Real-time biometric CVD (D3)
- Adversarial real-time visual observation (D3)
- **Post-hoc biometric verification** (D2)
- **Cryptographic identity binding** (D2)
- **Multi-party adversarial documentary custody** (D2)
- **Repeated adversarial observation** (D2)

**Absent these → D1 (insufficient evidence).**

---

## II. Version History

### v1.0.0 — Initial Release

- Core rules 1-9
- Table B structure
- A-claim ceiling

### v1.1.0 — Refined

- Tightened Rule 2
- Softened Rule 3 consensus treatment
- Added Rule 10 framing detection
- Mode separation protocols

### v1.2.0 — Hardened (Current)

- **Removed apologetic D1 language** ("expected," "not weakness," "structural")
- **D1 now explicitly "insufficient evidence"**
- **Broadened A-claim admissibility:** post-hoc biometric, cryptographic binding, multi-party custody, repeated observation
- **Tightened Gap Inventory:** mandatory specificity for unexcluded alternatives
- **Added prohibited outputs table**

---

## III. Usage Guidelines

### III.1 For Humans

**Before using PETDC, ask:**

1. Do I need evidence audit or historical inference?
2. Am I prepared for D1/Problematic as **insufficient evidence**?
3. Can I reformulate my A-claim into E-claims?

**If you need "what happened":** Use historiography, not PETDC.

**If you need "what can be certified":** Use PETDC.

### III.2 For LLMs

**Initiation checklist:**

- Declare version (v1.2.0)
- State rules 1-9 visible
- Acknowledge **D1 = insufficient evidence**
- Include control classification table

**Prohibited outputs:**

- "D1 is expected"
- "not evidentiary weakness"
- "structural limitation"
- "depending on..."

**Required:** Mechanical Table B completion or explicit Problematic classification with Rule citation.

---

## IV. Common Misunderstandings

### "D1 means expected outcome"

**No.** D1 means **insufficient evidence**. Audit failed.

### "Problematic means false"

**No.** Problematic means "not certifiable to required standard." Evidence is weak.

### "I can upgrade with more documents"

**No.** Documents are E-evidence. They cannot upgrade A-claims per Rule 2. Only admissible controls (Section 3.2) can.

### "Consensus helps"

**No.** Rule 3: Consensus is zero weight.

---

## V. Limitations

### V.1 Known Limitations

**Over-regularization:** PETDC may reject legitimate historical inference that ordinary standards accept.

**Brittleness:** Outputs expose evidence weakness that may be uncomfortable.

**A-claim skepticism:** Defaults most historical A-claims to D1. This is intentional.

---

## VI. Responsible Use

### VI.1 Do Not Weaponize

PETDC outputs can be misused:

- "Your claim is Problematic, end of story"
- Dismissing legitimate discourse

**Correct use:** "This A-claim is D1/Problematic. Here is the E-claim reformulation..."

### VI.2 Do Not Apologize

D1 is **insufficient evidence**, not "expected outcome." Do not soften the audit.

---

## VII. References

- Protocol: [PETDC_Protocol_v1.2.0.md](./PETDC_Protocol_v1.2.0.md)
- Repository: github.com/here-comes-everybody/PETDC
- License: Apache License 2.0

---

_"E ≠ A ≠ N. Signals ≠ Identity. No negotiation."_
