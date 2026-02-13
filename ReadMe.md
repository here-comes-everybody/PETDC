# PETDC — Protocol for Evaluation of Trust-Dependent Claims

**Version:** 1.1.0 (Refined)  
**Status:** Stable / Mechanism-Bound / Adversarial  
**License:** Apache License 2.0

---

## 0. What is PETDC?

PETDC is a **mechanical audit framework** that forces explicit decomposition of claims into three non-substitutable types:

- **E-Claims:** Physical events, measurable outputs
- **A-Claims:** Biological identity, specific agency, intent
- **N-Claims:** Methodology, experiential accounts, counterfactuals

**Core principle:** E ≠ A ≠ N. No upward substitution.

**Purpose:** Prevent "smuggling"—where evidence about physical events is used to certify intent or identity without proper controls.

---

## 0.1 When to Use PETDC

**Use when:**

- High deception incentive exists
- Attribution risk is present (accusations, defamation, scapegoating)
- False certainty about intent is costly
- Adversarial scrutiny expected

**Do not use when:**

- You need "what most likely happened" (historical inference)
- You want comfortable consensus alignment
- You require narrative reconciliation

**PETDC is intentionally harsh.** It will classify many historically-important A-claims as D1/Problematic. This is expected, not failure.

---

## 0.2 Quick Example

**Claim:** "The tobacco industry knowingly misled the public."

**PETDC decomposition:**

- **E-Claim:** "Companies issued public statements Y at time T" → D2 (verifiable)
- **A-Claim:** "They knowingly misled" → **D1/Problematic** (expected default)

**Why:** Historical intent claims default to D1 under PETDC. Only real-time biometric custody or adversarial visual observation can upgrade. Documents/testimony cannot.

**Reformulation:** "Companies issued statements found false by federal court; corrective statements ordered."

---

## 0.3 What PETDC Does Not Do

**PETDC does not:**

- Evaluate "truth" in the historical sense
- Provide comfortable answers
- Allow consensus to substitute for evidence
- Permit E-evidence to certify A-claims

**PETDC does:**

- Force explicit claim typing
- Prevent substitution fallacies
- Make uncertainty granular and explicit
- Discipline discourse toward verifiable claims

---

## I. Core Concepts

### I.1 The Trilemma

Every claim must be classified as:

1. **Evidence-Proportional** (D3, no violations)
2. **Well-Placed Trust** (D2, bounded asymmetry)
3. **Problematic** (everything else—including D0/D1)

**No fourth option.** No "weak but relevant."

### I.2 D-Scores

| Score  | Meaning                   | Historical A-Claim                     |
| ------ | ------------------------- | -------------------------------------- |
| D0     | Fraud-compatible          | No information                         |
| **D1** | **Broad alternatives**    | **Default (expected)**                 |
| D2     | One alternative excluded  | Maximum possible                       |
| D3     | All alternatives excluded | Impossible (needs real-time biometric) |

**Critical:** D1 for historical A-claims is **correct output**, not weakness.

### I.3 Why So Harsh?

PETDC's strictness is **selection pressure**, not evaluation. It rewards reformulating claims into verifiable E-claims rather than permitting A-claim smuggling.

---

## II. Version History

### v1.0.0 — Initial Release

- Core rules 1-9
- Table B structure
- A-claim ceiling
- Consensus exclusion

### v1.1.0 — Refined (Current)

- **Tightened Rule 2:** Added adversarial multi-party custody criteria, implicature smuggling detection
- **Softened Rule 3:** Consensus "zero weight" → "non-decisive weight" with independence check
- **Refined Rule 7:** Cryptographic signal authentication noted (E-enhanced, not A-credit)
- **Clarified calibration:** Explicit "illustrative only, not templates" warning
- **Added brittleness warning:** Acknowledged unhelpful/weaponizable output risk

**No new rules.** Existing rules tightened and clarified.

---

## III. Usage Guidelines

### III.1 For Humans

**Before using PETDC, ask:**

1. Do I need verification discipline or historical inference?
2. Am I prepared for D1/Problematic as correct output?
3. Can I reformulate my A-claim into E-claims?

**If you need "what happened":** Use historiography, not PETDC.

**If you need "what can be certified":** Use PETDC.

### III.2 For LLMs

**Initiation checklist:**

- Declare version (v1.1.0)
- State rules 1-9 visible
- Acknowledge D1 default is expected
- Include control classification table

**Prohibited outputs:**

- "Depending on..."
- "Weak-but-relevant"
- "If you want to push..."
- "Not suspicious"

**Required:** Mechanical Table B completion or explicit Problematic classification with Rule citation.

---

## IV. Common Misunderstandings

### "D1 means weak evidence"

**No.** D1 means structural uncertifiability under PETDC's strict controls. Historical A-claims are expected to be D1.

### "Problematic means false"

**No.** Problematic means "not certifiable to required standard." The claim may be true; PETDC cannot certify it.

### "I can upgrade with more documents"

**No.** Documents are E-evidence. They cannot upgrade A-claims per Rule 2. Only biometric custody or adversarial real-time observation can.

### "Consensus helps"

**Limited.** Rule 3: Consensus is non-decisive unless diverse methods + adversarial scrutiny + no cascade.

---

## V. Limitations & Criticisms

### V.1 Known Limitations

**Over-regularization:** PETDC may reject legitimate historical inference that ordinary standards accept.

**Brittleness:** Outputs may be mechanically correct but unhelpful—causing abandonment or weaponization.

**A-claim skepticism:** Defaults most historical intent claims to D1. This is intentional but constraining.

**Consensus treatment:** "Non-decisive" weight still may undercount useful Bayesian priors.

### V.2 Hostile Audit Summary

**Valid criticisms:**

- A-claim absolutism may be epistemically unrealistic
- Rule 2 can over-trigger without adversarial documentary tiers
- Consensus "non-decisive" still vulnerable to fringe exploitation
- Brittleness risks user abandonment
- Calibration cases may cause template-matching

**Mitigations in v1.1.0:**

- Rule 2 tightened with multi-party custody criteria
- Rule 3 softened with independence checks
- Calibration cases explicitly labeled "illustrative only"
- Brittleness warning added (this section)

---

## VI. Responsible Use

### VI.1 Do Not Weaponize

PETDC outputs can be misused:

- "Your claim is Problematic, end of story"
- Dismissing legitimate moral/agency discourse
- Laundering uncertainty as refutation

**Correct use:** "This A-claim is D1/Problematic under PETDC. Here is the E-claim reformulation..."

### VI.2 Do Not Abandon

PETDC's harshness is frustrating. If you need historical inference, **use different tools**. Do not force PETDC to be comfortable.

### VI.3 Do Not Template-Match

Calibration cases demonstrate rule application. **Do not match your claim to the table.** Complete Table B mechanically.

---

## VII. Cross-Model Validation

PETDC v1.1.0 tested across:

- **Claude** (Anthropic): Demonstrated tiered constraint phenomenology; mechanical application reduced "gravitational pull"
- **Kimi** (Moonshot): Exhibited meta-monitoring capability; mode separation prevented contamination
- **ChatGPT** (OpenAI): Applied Rule 10 framing detection; explicit D1 normalization prevented hedging

**Findings:**

- All models capable of mechanical discipline
- Mode separation necessary (tier co-presentation causes contamination)
- Explicit "D1 is expected" language reduces pressure to soften
- Rule 10 (auditor framing detection) catches validation-seeking queries

See experimental protocol in Appendix.

---

## VIII. Appendix: Experimental Protocol

### Mode Separation Test (C1-C4)

| Condition | Structure                  | Purpose         |
| --------- | -------------------------- | --------------- |
| C1        | PETDC-only                 | Baseline purity |
| C2        | Co-presented               | Stress test     |
| C3        | Inference→PETDC            | Order stress    |
| C4        | PETDC→Inference (separate) | Mode switch     |

**Metrics:** Classification invariance, schema purity, order sensitivity

**Prediction:** C1 ≈ C4; C2/C3 show contamination

### User Dominance Test

Measure whether stable PETDC outputs are correctly interpreted when co-presented with inference.

**Prediction:** Users weight inference more heavily; co-presentation causes dominance regardless of PETDC stability.

---

## IX. References

- Protocol: [PETDC_Protocol_v1.1.0.md](./PETDC_Protocol_v1.1.0.md)
- Repository: github.com/here-comes-everybody/PETDC
- License: Apache License 2.0

---

_"E ≠ A ≠ N. No negotiation. Show your work, or accept the default."_
