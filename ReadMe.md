# PETDC — Protocol for Evaluation of Trust-Dependent Claims

**Version:** 1.3.0  
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

**v1.3.0 Hardening:** R7 eliminated. Template governance. Self-referential external custody. Gap Inventory registration. Framework temporal firewall.

---

## 0.1 When to Use PETDC

**Use when:**

- High deception incentive exists
- Attribution risk is present (accusations, defamation, scapegoating)
- False certainty about intent is costly
- Adversarial scrutiny expected

**PETDC is harsh.** It will classify many claims as D1/Problematic. This indicates **insufficient evidence**, not "expected outcome."

**Do not use for:**

- Action justification under uncertainty (no R7 lane)
- First-person mental state certification (no admissible controls)
- Bayesian likelihood output (D-scores only)

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
- **Justify action under uncertainty (v1.3.0: R7 removed)**

**PETDC does:**

- Force explicit claim typing
- Prevent substitution fallacies
- Make uncertainty granular and explicit
- Expose evidence weakness
- **Require external custody for self-referential audits (v1.3.0)**

---

## I. Core Concepts

### I.1 The Trilemma

Every claim must be classified as:

1. **Evidence-Proportional** (D3, no violations)
2. **Well-Placed Trust** (D2, bounded asymmetry)
3. **Problematic** (everything else—including D0/D1)

**No fourth option. No R7.**

### I.2 D-Scores

| Score  | Meaning                                              |
| ------ | ---------------------------------------------------- |
| D0     | Fraud-compatible                                     |
| **D1** | **Insufficient evidence; broad alternatives remain** |
| D2     | One alternative excluded                             |
| D3     | All alternatives excluded                            |

**Critical:** D1 indicates **audit failure**, not "expected outcome."

### I.3 A-Claim Admissibility (v1.3.0)

Historical A-claims may achieve D2+ with:

- Real-time biometric CVD (D3)
- Adversarial real-time visual observation (D3)
- **Post-hoc biometric verification** (D2)
- **Cryptographic identity binding** (D2)
- **Multi-party adversarial documentary custody** (D2)
- **Repeated adversarial observation** (D2)

**Absent these → D1 (insufficient evidence).**

### I.4 Template Governance (v1.3.0)

Gap Inventory process models are **version-locked**. Novel processes require escalation. Prevents arbitrary "normal process" invention.

### I.5 Self-Referential Restriction (v1.3.0)

PETDC auditing itself requires **external custody**. No framework self-certification without adversarial review.

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

### v1.2.0 — Hardened

- **Removed apologetic D1 language** ("expected," "not weakness," "structural")
- **D1 now explicitly "insufficient evidence"**
- **Broadened A-claim admissibility:** post-hoc biometric, cryptographic binding, multi-party custody, repeated observation
- **Tightened Gap Inventory:** mandatory specificity for unexcluded alternatives
- **Added prohibited outputs table**

### v1.3.0 — Ungameable (Current)

- **R7 removed:** No action lane, preserves Trilemma integrity
- **Template governance:** Exhaustive process model list, escalation required
- **Gap Inventory registration:** Immutable public record
- **Self-referential external custody:** Framework cannot self-certify
- **Framework temporal firewall:** Version locked at audit initiation
- **Mechanical "adversarial" test:** Demonstrated, not inferred

---

## III. Usage Guidelines

### III.1 For Humans

**Before using PETDC, ask:**

1. Do I need evidence audit or historical inference?
2. Am I prepared for D1/Problematic as **insufficient evidence**?
3. Can I reformulate my A-claim into E-claims?
4. **Am I seeking action justification? (If yes, PETDC is wrong tool)**

**If you need "what happened":** Use historiography, not PETDC.

**If you need "what can be certified":** Use PETDC.

**If you need "what to do":** Use decision framework outside PETDC scope.

### III.2 For LLMs

**Initiation checklist:**

- Declare version (v1.3.0)
- State rules 1-8 visible
- Acknowledge **D1 = insufficient evidence**
- Acknowledge **R7 removed**
- Include control classification table
- **Acknowledge self-referential restriction (10.4)**

**Prohibited outputs:**

- "D1 is expected"
- "not evidentiary weakness"
- "structural limitation"
- "depending on..."
- **"likely" / "probably" (Bayesian language)**

**Required:** Mechanical Table B completion or explicit Problematic classification with Rule citation.

**Self-referential audits:** Require external custody declaration.

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

### "R7 allows action under uncertainty"

**No.** R7 removed v1.3.0. PETDC is epistemic only. Action justification outside scope.

---

## V. Limitations

### V.1 Known Limitations

**Over-regularization:** PETDC may reject legitimate historical inference that ordinary standards accept.

**Brittleness:** Outputs expose evidence weakness that may be uncomfortable.

**A-claim skepticism:** Defaults most historical A-claims to D1. This is intentional.

**No action guidance:** v1.3.0 explicitly removes action lane. Users must seek separate decision frameworks.

**Self-referential cost:** Auditing PETDC with PETDC requires external custody, increasing overhead.

---

## VI. Responsible Use

### VI.1 Do Not Weaponize

PETDC outputs can be misused:

- "Your claim is Problematic, end of story"
- Dismissing legitimate discourse

**Correct use:** "This A-claim is D1/Problematic. Here is the E-claim reformulation..."

### VI.2 Do Not Apologize

D1 is **insufficient evidence**, not "expected outcome." Do not soften the audit.

### VI.3 Do Not Confuse Epistemic with Decision

PETDC certifies evidence. It does not justify action. **R7 removed v1.3.0.**

---

## VII. References

- Protocol: [PETDC_Protocol_v1.3.0.md](./PETDC_Protocol_v1.3.0.md)
- Repository: github.com/here-comes-everybody/PETDC
- License: Apache License 2.0

---

_"E ≠ A ≠ N. Signals ≠ Identity. No negotiation. No R7."_
