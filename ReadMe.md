# PETDC ReadMe

[**Accompanying Document: PETDC Protocol**](https://github.com/here-comes-everybody/PETDC/blob/main/PETDC%20Protocol.md)

---

## Version Lock Notice

&gt; **This document provides context, guidance, and application examples for PETDC.** For enforceable rules, consult the Protocol. **If version mismatch detected between Protocol and ReadMe, Protocol rules take precedence.** This ReadMe may update independently of Protocol versions.

---

## 0. Framework Positioning

### 0.1 What PETDC Is

PETDC is a **maximalist verification standard for adversarial contexts** where:

- Deception incentives are high
- Institutional capture is possible
- Evidence substitution is suspected
- Consequences of misplaced trust are severe

**Design principle:** Resist social negotiation of epistemic standards.

### 0.2 What PETDC Is Not

| Not This                    | Because                                                                    |
| --------------------------- | -------------------------------------------------------------------------- |
| **Universal epistemology**  | PETDC is conservative; most daily knowledge operates on weaker standards   |
| **Decision framework**      | PETDC classifies claims; it doesn't tell you whether to act on D1 evidence |
| **Everyday epistemology**   | Most daily decisions require acting on D1/D2 evidence                      |
| **Scientific methodology**  | Domain methods are appropriate for research; PETDC is for post-hoc audit   |
| **Legal evidence standard** | Courts balance error types differently; PETDC maximizes fraud detection    |

### 0.3 When to Apply PETDC

**High-value contexts:**

- Intelligence analysis of adversarial claims
- Fraud investigation
- Institutional accountability audits
- Historical revisionism disputes
- Synthetic media authentication
- High-stakes verification (cryptographic ceremonies, election integrity)

**Low-value contexts (PETDC often overkill):**

- Personal relationships (trust is decision, not verification exercise)
- Exploratory research (premature rigor inhibits discovery)
- Time-sensitive decisions (cost exceeds benefit)
- Aesthetic/ethical claims (not falsifiable structure)

### 0.4 Relationship to Other Standards

| Framework                       | Focus                               | PETDC Difference                                                     |
| ------------------------------- | ----------------------------------- | -------------------------------------------------------------------- |
| **Bayesian epistemology**       | Probability updating                | PETDC prevents category errors _before_ calculating likelihoods      |
| **Legal evidence**              | Balancing false positives/negatives | PETDC minimizes false positives only (assumes fraud-seeking context) |
| **Scientific peer review**      | Consensus convergence               | PETDC treats consensus as zero-weight (Rule 3)                       |
| **Intelligence Admiralty Code** | Source + info reliability           | PETDC adds E/A/N decomposition + control classification              |
| **Journalistic verification**   | Dual sourcing, attribution          | PETDC requires mechanism specification (Rule 1)                      |

**PETDC is stricter than all of these by design.** It's adversarial epistemology.

---

## XIV. Bayesian Interpretation (How to Use PETDC with Probability)

### 14.1 D-Scores as Likelihood Ratio Bounds

PETDC D-scores can be **approximated** as likelihood ratio bounds for "claim is true" vs. "claim is fraudulent":

| D-Score | Likelihood Ratio | Bits of Evidence | Interpretation                         |
| ------- | ---------------- | ---------------- | -------------------------------------- |
| **D0**  | ~1:1             | 0 bits           | No discrimination from fraud           |
| **D1**  | ~1:1 to 10:1     | 0-3.3 bits       | Weak discrimination; many alternatives |
| **D2**  | ~10:1 to 1000:1  | 3.3-10 bits      | One major alternative excluded         |
| **D3**  | &gt;1000:1       | &gt;10 bits      | All plausible alternatives excluded    |

**Critical:** These are **rough calibrations** for post-hoc analysis. D-scores are **categorical assignments**, not point estimates. Do not use "confidence intervals" or probabilistic language during classification.

### 14.2 Why PETDC Doesn't Use Probability Directly

**Reason 1: Category errors precede probability**
Computing $P(\text{Armstrong on moon} | \text{lunar samples exist})$ requires that lunar samples _can_ verify Armstrong's presence. Rule 7 says they can't (E≠A). Category error → probability calculation is meaningless.

**Reason 2: Control classification affects priors**
Centralized control means claimant can select evidence. This affects prior probability in ways standard Bayesian analysis doesn't capture.

**Reason 3: Adversarial context assumption**
Standard Bayesian reasoning assumes honest error vs. truth. PETDC assumes adversarial selection. Different probability space.

### 14.3 Integration Path

To use PETDC with Bayesian reasoning:

1. **Apply PETDC first** — Decompose E/A/N, check for substitution violations
2. **If Problematic** — Identify which claim is actually verified (often E when A was asserted)
3. **Calculate likelihood ratio** — For the _correct_ claim type, use D-score as LR bound
4. **Update** — Apply to appropriate prior

**Example (Apollo):**

- **Wrong:** $P(\text{Armstrong there} | \text{samples + signals})$
- **Right:** $P(\text{hardware there} | \text{samples + signals})$ (D3, LR &gt;1000:1) AND $P(\text{Armstrong there} | \text{signals only})$ (D1, LR ~1-10:1)

---

## XV. Decision Integration

### 15.1 Graduated Action Framework

PETDC classifies; you decide. General principles for using classifications:

| Classification                 | Institutional Use                                  | Personal Use                                     | Legal Use                            |
| ------------------------------ | -------------------------------------------------- | ------------------------------------------------ | ------------------------------------ |
| **Evidence-Proportional (D3)** | Can cite as established fact                       | High confidence                                  | Meets "beyond reasonable doubt"      |
| **Well-Placed Trust (D2)**     | Cite with caveat on remaining alternatives         | Reasonable confidence                            | May meet "preponderance of evidence" |
| **Problematic (D0-D1)**        | **Cannot cite as fact**; acknowledge as unverified | Low confidence; verify independently if critical | Insufficient for conviction          |

### 15.2 Cost-Benefit Considerations

**Achieving D3 is expensive.** When is it worth it?

**Worthwhile for D3 verification:**

- Precedent-setting legal cases (verified facts become binding)
- Foundational scientific claims (many studies build on them)
- National security claims (war/peace decisions)
- Cryptographic ceremonies (long-term security depends on them)
- Historical events with major policy implications

**Not worthwhile for D3:**

- One-off operational decisions
- Rapidly changing domains (verification obsolete before complete)
- Low-stakes personal decisions
- Exploratory research hypotheses

### 15.3 Institutional Adaptation Paths

**If Apollo A-claims are Problematic, then what?**

**Option 1: Accept D1 status**

- Teach as: "Evidence strongly suggests humans went, but identity verification didn't meet adversarial standards"
- Cite for E-claims only: "Lunar samples demonstrate hardware reached moon"
- Stop using for A-claim precedent

**Option 2: Upgrade to D2**

- Retrospective: Interview surviving witnesses under adversarial cross-examination
- Establish bounds on remaining alternatives
- Acknowledge gap frankly

**Option 3: Invest in D3 for future missions**

- International crew (distributed A-control)
- Real-time biometric CVD with hostile nation monitoring
- Adversarial visual observation provisions

**Most institutions will choose Option 1** (accept honest D1 status) for historical claims and Option 3 (design for D3) for future claims.

### 15.4 "So What?" for Each Case

**Apollo → Problematic (A-claim):**

- **Academic:** Stop citing as precedent for human spaceflight capability in adversarial debates
- **Policy:** Design Artemis for D3 (international crew, hostile monitoring)
- **Public:** Honest framing — "compelling evidence but not adversarially verified"

**Zoom attendance → Problematic:**

- **HR:** Video evidence insufficient for disciplinary action without corroboration
- **Legal:** Remote testimony requires additional authentication
- **Cultural:** Normalize "I need to verify you're actually there" requests

**Peer review → Often Problematic:**

- **Academic:** Distinguish "peer-reviewed" from "reproducible" explicitly
- **Policy:** Science-based policy requires D2+ (data sharing mandatory)
- **Funding:** Tie funding to verification tier achieved

### 15.5 Defense Against Nihilism Charge

**Objection:** "PETDC makes everything unknowable!"

**Response:**

1. **False.** Earth's shape is D3. Many E-claims are D3. Super Bowl 2024 achieved D3 for A-claims.

2. **Conflates decision with verification.** Acting on D1 evidence is often rational (cost-benefit). PETDC just forces you to acknowledge it's D1.

3. **Exposes existing nihilism.** Institutions _already_ don't have D3 for many claimed facts. PETDC reveals this; it doesn't create it.

4. **Provides upgrade path.** If you want D3, PETDC tells you exactly what's required. That's the opposite of nihilism.

**The real objection is to honesty.** PETDC forces explicit acknowledgment of verification gaps. Comfort ≠ knowledge.

---

## XVI. Positive Construction: Achieving D3

### 16.1 Case Study: D3 A-Claim for Historical Event

**Claim:** "George Washington crossed the Delaware River on December 25, 1776"

**Current status:** D1 (historical A-claim default)

**Path to D2:**

1. Multiple independent contemporary accounts from hostile parties (British officers, Hessian commanders)
2. Accounts include details that discriminate presence from absence (weather, timing, specific locations)
3. Accounts from parties with incentive to challenge if false
4. Physical evidence (boats, encampment sites) consistent with claim

**Result:** D2 achievable via adversarial historical method. One alternative excluded: "Event didn't happen." Remaining: "Different commanders led it," "Different date," etc.

**Path to D3:** **Impossible retroactively.** Would have required:

- Adversarial real-time visual observation (British officer embedded with Continental Army), OR
- Real-time biometric CVD with independent custody (not technologically possible in 1776)

**Lesson:** Most historical A-claims cap at D2. Accept this honestly.

### 16.2 Case Study: Designing D3 Future Mission

**Goal:** Verify humans land on Mars to D3 standard

**E-claim (hardware lands):**

- Distributed sample return
- Retroreflectors/equipment verifiable by hostile nations
- **Already achievable D3**

**A-claim (specific humans present):**

**Design requirements for D3:**

1. **International crew** (US, China, EU, Russia)
   - A-control becomes Distributed (hostile cross-verification)
   - Each nation has incentive to expose fraud by others

2. **Real-time biometric CVD with adversarial custody**
   - Vital signs monitored by hostile nation ground stations
   - Medical data transmitted to distributed receivers
   - Independent verification of biological signatures

3. **Adversarial visual observation**
   - Crew compartment has cameras controlled by different nations
   - Live feeds to hostile parties
   - Physical access to spacecraft by competing inspectors pre-launch

4. **Chain of custody for humans**
   - Pre-mission biometric baseline (DNA, retinal, fingerprint) recorded by multiple nations
   - Real-time comparison during mission
   - Post-mission verification by hostile parties

**Cost:** Substantially higher than single-nation mission

**Benefit:** A-claims achieve D3; no post-mission controversy possible

**Trade-off:** Worth it if Mars landing will be cited as precedent for human capability in adversarial contexts (e.g., competing with China). Not worth it if purely exploratory.

### 16.3 Case Study: D3 for Synthetic Era Video

**Claim:** "This video shows candidate X accepting a bribe"

**Pre-synthesis:** Security camera footage could achieve D2 via expert analysis

**Post-synthesis:** D1 default (pixel-perfect generation possible)

**Path to D2-D3:**

1. **Cryptographic camera timestamping**
   - Hardware-secured clock
   - Signed frames at capture time
   - Verifiable by third parties
   - Achieves: E-claim D3 (video created at time T)
   - Doesn't achieve: A-claim verification (could still be deepfake created at time T)

2. **Multi-angle adversarial recording**
   - Multiple parties recording simultaneously
   - Geometric consistency check across angles
   - Adversarial parties (competing campaigns) cross-verify
   - Achieves: A-claim D2 (coordinated multi-angle deepfake excluded)

3. **Real-time biometric broadcast**
   - Candidate wears verified biometric device
   - Heart rate, skin conductance transmitted to distributed monitors
   - Correlated with video events
   - Achieves: A-claim D3 (presence verified by biometric CVD)

**Implication:** High-stakes events (debates, testimony, negotiations) will need explicit verification infrastructure. Casual video will cap at D1 for A-claims.

### 16.4 Calibration: What D3 Costs

| Domain                        | D1 Cost                     | D3 Cost                                                               | Multiplier |
| ----------------------------- | --------------------------- | --------------------------------------------------------------------- | ---------- |
| **Academic paper**            | $50K (single lab)           | $500K (multi-lab replication, open data, adversarial review)          | 10x        |
| **Criminal trial evidence**   | $10K (police investigation) | $100K (adversarial forensics, independent custody, expert cross-exam) | 10x        |
| **Space mission**             | $1B (single nation)         | $10B (international crew, distributed monitoring)                     | 10x        |
| **Corporate financial audit** | $1M (standard audit)        | $10M (adversarial audit, real-time distributed monitoring)            | 10x        |
| **Election integrity**        | $100M (standard procedures) | $1B (end-to-end cryptographic verification, hostile observer access)  | 10x        |

**Pattern:** D3 costs ~10x more than D1. Sometimes worth it, often not.

**PETDC doesn't say you must always achieve D3.** It says: be honest about what tier you've achieved and act accordingly.

---

## XVII. Relation to Existing Frameworks

### 17.1 Intelligence Analysis Standards

**Admiralty Code (US Intelligence Community):**

- Source reliability: A (completely reliable) to F (unreliable)
- Information credibility: 1 (confirmed) to 6 (cannot be judged)

**PETDC differences:**

- Adds E/A/N decomposition (Admiralty doesn't distinguish claim types)
- Control classification (Distributed/Centralized) vs. source reliability
- Mechanical enforcement (Admiralty allows analyst judgment)

**Complementary use:** Apply PETDC to decompose claim, then use Admiralty for source rating.

### 17.2 Bayesian Epistemology

**Standard approach:** Update P(H|E) using likelihood ratios

**PETDC contribution:**

- **Pre-Bayesian filter** — Checks if E can verify H (E≠A≠N)
- **Control-adjusted priors** — Centralized control lowers prior on honest claim
- **Adversarial likelihood** — LR calculated assuming fraud-seeking context

**Integration:** PETDC → identify correct claim type → Bayesian update on that type

**Citations:**

- Jaynes, E.T. (2003). _Probability Theory: The Logic of Science_
- Pearl, J. (2009). _Causality_
- Yudkowsky, E. (2015). "A Technical Explanation of Technical Explanation"

### 17.3 Evidentiary Standards (Legal)

**US Criminal:** Beyond reasonable doubt (~90-95% confidence)
**US Civil:** Preponderance of evidence (~51% confidence)
**PETDC D3:** &gt;99.9% confidence (LR &gt;1000:1)

**Key difference:** Legal standards balance Type I vs. Type II errors. PETDC minimizes Type I only (false positives). This reflects different contexts:

- **Legal:** Punishing innocent is worse than freeing guilty
- **PETDC:** Trusting fraudulent claim is worse than withholding trust from honest claim

**When PETDC applies to legal:** Fraud prosecution, adversarial contexts where deception is alleged

### 17.4 Scientific Evidence Hierarchy

**Medical research pyramid:**

1. Meta-analyses (top)
2. Randomized controlled trials
3. Cohort studies
4. Case-control studies
5. Case reports (bottom)

**PETDC mapping:**

- Meta-analysis: Still requires checking each study for E/A/N decomposition
- RCT: Can achieve D3 for E-claims (treatment effect) but still D1 for A-claims (patient identity) unless biometric CVD
- Observational: Typically D1-D2 depending on control classification

**PETDC adds:** Control classification, adversarial verification, anti-consensus (Rule 3)

**Citations:**

- Guyatt, G.H. et al. (2008). "GRADE: an emerging consensus on rating quality of evidence"
- Ioannidis, J.P. (2005). "Why Most Published Research Findings Are False"

### 17.5 Philosophical Precedents

**Hume on testimony:** "No testimony is sufficient to establish a miracle, unless the testimony be of such a kind, that its falsehood would be more miraculous than the fact"

- **PETDC version:** No testimony achieves D3 (Rule 7: signals ≠ biometric)

**Descartes' evil demon:** Radical skepticism — what if all senses deceive?

- **PETDC response:** Not claiming sense deception; claiming category errors (E substituted for A)

**Wittgenstein on certainty:** "I know I have two hands"

- **PETDC:** Personal certainty ≠ adversarial verification standard

**Quine on underdetermination:** Evidence underdetermines theory

- **PETDC:** Makes this mechanical via $H_d$ (discrimination entropy)

**Goldman on social epistemology:** How do we trust expert testimony?

- **PETDC:** We don't (Rule 3: zero weight to consensus)

**Citations:**

- Hume, D. (1748). _An Enquiry Concerning Human Understanding_
- Goldman, A. (1999). _Knowledge in a Social World_
- Hardwig, J. (1985). "Epistemic Dependence"

### 17.6 What's Novel in PETDC

**Unique contributions:**

1. **E/A/N categorical decomposition** — Not in any existing framework
2. **Control classification independent of evidence type** (Rule 8) — Novel insight
3. **Mechanical anti-substitution rules** — Existing frameworks allow expert override
4. **Synthesis-era adaptation** — Explicit treatment of deepfakes as categorical change
5. **Patterned destruction inference** (Rule 9) — Systematic gap analysis
6. **Anti-consensus stance** (Rule 3) — Rare in academic epistemology
7. **Adversarial visual observation standard** — Operationalizes "seeing is believing" for synthetic era

**Prior art does not exist for:** A complete framework combining all seven elements above.

---

## XVIII. Meta-Questions

### 18.1 Verifying PETDC Itself

**Claim:** "PETDC correctly categorizes verification standards"

**E-claim:** PETDC produces classifications (D0-D3, Problematic/Well-Placed Trust/Evidence-Proportional)

- **Verification:** Apply PETDC to test cases, observe outputs
- **D-score:** D3 (mechanism is specified, reproducible)

**N-claim:** PETDC's classifications track actual verification quality

- **Verification:** Compare PETDC outputs to known fraud cases + known-true cases
- **Method:** Calibration studies (Section XVI examples show preliminary calibration)
- **D-score:** Currently D1 (insufficient independent validation)

**Meta-result:** PETDC's _normative_ claims (what _should_ count as verification) are not empirically verifiable — they're philosophical positions.

**Honest acknowledgment:** PETDC is a proposed standard, not a discovered fact. Its value is pragmatic (does it help avoid errors?) not metaphysical (does it track truth?).

### 18.2 Potential Failure Modes

**Where PETDC might err:**

1. **Overfitting to deception** — Assumes adversarial context; may be too strict for cooperative truth-seeking
2. **Categorical rigidity** — E/A/N boundaries may be fuzzy in practice
3. **D-score granularity** — 4 levels might be too coarse or too fine
4. **Temporal cutoff arbitrariness** — 24-hour real-time boundary is unprincipled
5. **Control classification edge cases** — Semi-Distributed category may need subdivision

**Improvement path:** Empirical calibration via fraud detection studies.

### 18.3 When to Abandon PETDC

**Red flags indicating framework failure:**

- **If D3 becomes routinely achievable cheaply** — Indicates standards too loose
- **If no historical events achieve D2+** — Indicates standards uselessly strict
- **If major fraud passes D3** — Indicates rules have loopholes
- **If cost/benefit consistently negative** — Indicates framework impractical

**Monitoring:** Track calibration cases. If fraud rate in D3-classified claims exceeds 0.1%, framework needs tightening. If useful true claims consistently land in Problematic, framework needs loosening.

### 18.4 Ideological Capture Risk

**PETDC could be weaponized for:**

- Blanket institutional dismissal (ignore all D1 claims regardless of cost-benefit)
- Motivated reasoning (apply strictly to opponent claims, leniently to favored claims)
- Paralysis (demand D3 for every decision)

**Safeguards:**

- Scope limitation (Section 0) — not for everyday decisions
- Symmetric application requirement — apply same standards to favored and disfavored claims
- Cost-benefit integration (Section XV) — acknowledge when D1 is sufficient

**Warning:** If you're only applying PETDC to claims you already distrust, you're using it wrong.

---

## Appendix A: Glossary

| Term                               | Definition                                                                         |
| ---------------------------------- | ---------------------------------------------------------------------------------- |
| **A-Bridge**                       | Constrained upgrade path from E to A requiring multi-modal, actor-binding evidence |
| **A-Claim**                        | Biological or specific agency/identity claim                                       |
| **Adversarial visual observation** | Hostile real-time witnessing meeting 5 criteria (Section 3.2)                      |
| **CVD**                            | Compelling Verifiable Data — mechanism-bound evidence                              |
| **D-Score**                        | Discrimination level (D0-D3) based on alternatives excluded                        |
| **E-Claim**                        | Physical occurrence, measurable output                                             |
| **EWP**                            | Evidence-Weight Penalty — triggered by substitution violations                     |
| **HDE**                            | Historical Data Evaluation — retrospective evidence assessment                     |
| **N-Claim**                        | Methodology, experiential account, counterfactual                                  |
| **OIE**                            | Observation Independent of Event — real-time independent custody                   |
| **PETDC**                          | Protocol for the Evaluation of Trust-Dependent Claims                              |
| **Problematic**                    | Trilemma Option 3 — anything not Evidence-Proportional or Well-Placed Trust        |
| **PUF**                            | Physical Unclonable Function — hardware-unique physical signature                  |
| **Shadowing Check**                | Verification that observation occurred simultaneously with claimed event           |
| **Trilemma**                       | Three exhaustive classification options (no fourth)                                |
| **VAR**                            | Verification Asymmetry Ratio — real-time metric                                    |
| **HTR**                            | Historical Trust Ratio — retrospective metric                                      |

---

## Appendix B: Quick Reference Card

### Claim Classification (30 seconds)

1. **What type?** E (physical) / A (biological/identity) / N (method/narrative)
2. **What evidence?** List CVD inventory
3. **What control?** Distributed / Semi-Distributed / Centralized
4. **Apply Rule 2** — Is A-claim supported by biometric CVD, adversarial observation, or PUF-enhanced control?
5. **Assign D-score** — D0 (fraud-compatible) / D1 (broad alternatives) / D2 (one excluded) / D3 (all excluded)
6. **Trilemma** — Evidence-Proportional (D3) / Well-Placed Trust (D2) / Problematic (D0-D1)

### Immediate Red Flags

- [ ] "Video proves presence" → **Rule 7 violation** (signals ≠ biometric)
- [ ] "Everyone agrees" → **Rule 3 violation** (consensus = zero weight)
- [ ] "We audited it" → **Rule 4 violation** (audit ≠ OIE)
- [ ] "Not suspicious" → **Rule 9 violation** (patterned destruction inference mandatory)

### When to Stop

- If classification is **Problematic** → Do not cite as fact. Acknowledge gap.
- If upgrade path unclear → Default D1. No negotiation.

---

## Appendix C: Use-Case Playbooks

### C.1 Identity Verification

**Context:** Remote employee onboarding, high-security access

**Common failure:** Video interview = D1 A-claim (Rule 7)

**D2 path:**

- PUF-attested device + liveness biometric
- Government ID verification via independent service
- Third-party background check (independent modality)

**D3 path:**

- In-person biometric enrollment with adversarial observer
- Real-time biometric monitoring during access
- Distributed custody of biometric templates

### C.2 Newsroom Verification

**Context:** Publishing video of breaking event

**Common failure:** Single-source viral video = D1 E-claim, D1 A-claim

**D2 path:**

- Multi-angle verification (independent recordings)
- Geometric consistency checks
- Timestamp verification (blockchain or hardware-secured)

**D3 path:**

- Cryptographic camera signatures
- Real-time broadcast to distributed receivers
- Adversarial party confirmation (competing news orgs)

### C.3 Court Exhibit Evaluation

**Context:** Digital evidence admissibility

**Common failure:** Screenshots, unverified chain of custody

**PETDC application:**

- E-claim: File existence, metadata properties
- A-claim: Who created it, when, where (requires biometric CVD or PUF-enhanced control)
- N-claim: Expert interpretation of content

**Recommendation:** Most digital evidence = D1 A-claim. Admit as E only unless biometric/PUF provenance established.

### C.4 Scientific Causality Claims

**Context:** "Treatment X causes outcome Y in population Z"

**E-claim:** Effect observed in study population (D3 achievable via RCT)
**A-claim:** Specific patients took specific doses (D1 unless biometric CVD)
**N-claim:** Mechanism of action, generalizability (often Problematic)

**Publication standard:** Require D3 E-claim (reproducible effect) + honest D1/D2 A-claim acknowledgment.

---

## Document Control

|                | Protocol                              | ReadMe                      |
| -------------- | ------------------------------------- | --------------------------- |
| **Version**    | 1.0 (semantic)                        | 2026-02-13 (dated)          |
| **Updates**    | Rules changes only                    | Context, examples, guidance |
| **Precedence** | **Supreme**                           | Subordinate                 |
| **Repository** | github.com/here-comes-everybody/PETDC | Same                        |
| **License**    | Apache License 2.0                    | Same                        |

**Version Check:** Before use, verify Protocol version matches ReadMe date. Mismatch → Protocol governs.

---

**End of ReadMe**
