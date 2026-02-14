# Roadmap: v1.3.0 (Synthetic Default)

**Status:** Draft / Proposed
**Target:** Hardening against Generative AI & Deepfakes
**Contributor:** Gemini 3 Pro (Google)
**Date:** February 14, 2026

---

## 0. Executive Summary

The v1.3.0 update (codenamed "Synthetic Default") addresses the epistemic collapse caused by high-fidelity generative AI.

**Core Logic:** In a post-truth environment, video and audio are no longer E-Claims (Events). They are N-Claims (Narratives) by default. They only become E-Claims when cryptographically bound to a specific sensor event via hardware attestation.

---

## I. Protocol Updates

### 1.1 Hardening Table B: The "Provenance" Row

Current Table B focuses on generic "CVD Inventory". v1.3.0 adds explicit handling for digital assets.

- [ ] **Add Row 1.5: "Provenance Binding"**
  - **Requirement:** Digital A-claims (video/photo of specific agency) require **Hardware-Rooted Attestation** (e.g., C2PA, Sony In-Camera Signing, or adversarial custody of raw media).
  - **Constraint:** Absent cryptographic signature from the sensor or hostile chain of custody → Classify as **"Synthetic / N-Claim"** (Methodology/Art).
  - **Outcome:** Unsigned MP4s are treated mathematically identically to AI-generated video.

### 1.2 Refine Rule 7: The Analog/Digital Gap

Rule 7 currently defaults signals to E-claims. This opens a vulnerability to generative interception.

- [ ] **Rename Rule 7:** "The Synthetic Default"
- [ ] **New Definition:** "Any signal capable of being synthesized by a Turing-complete machine prior to display is **N-claim (Narrative)** until cryptographically bound."
- [ ] **Impact:** Explicitly classifies "Live TV Broadcasts" and "Leaked Audio" as N-claims (unverified narrative constructs) unless the raw feed possesses public key signing or adversarial corroboration.

### 1.3 Harden Rule 5: The "Secrecy Corollary"

Rule 5 infers "patterned destruction" when CVD is missing. v1.3.0 closes the "Operational Security" (OpSec) loophole.

- [ ] **Add "The Secrecy Corollary":**
  - "Operational Necessity (OpSec) explains the _absence_ of evidence, but does not _substitute_ for it."
  - "A secret event is legally distinct from a fabricated event, but **epistemically identical**."
  - **Outcome:** OpSec = **D1 (Insufficient Evidence)**. No exceptions for state actors or classified programs.

---

## II. Documentation Updates

### 2.1 The "Post-Truth" Primer

The ReadMe must explain _why_ PETDC treats video as "cartoon" by default.

- [ ] **Create `docs/The_Synthetic_Default.md`:**
  - **Axiom:** "If a pixel _could_ have been generated, it must be treated as if it _was_."
  - **Demonstration:** Contrast a C2PA-signed image (D2/D3) vs. a standard viral video (D1/Problematic).
  - **Purpose:** Clarify that rejecting video evidence is not "denialism," but a necessary security posture in 2026.

### 2.2 Addressing "Impossible Standards"

- [ ] **Add FAQ Entry:** "Why does PETDC reject historical consensus?"
  - **Answer:** PETDC distinguishes between _Institutional Consensus_ (Rule 3 violations) and _Adversarial Verification_ (Section 3.2).
  - **Case Studies:** Contrast **The Holocaust** (Adversarial Custody = D2/D3) vs. **Apollo/OBL** (Centralized Custody = D1).
  - **Goal:** Show that high D-scores are possible, but only through adversarial capture, not claimant authority.

---

## III. Tooling

### 3.1 Gap Inventory Worksheet

- [ ] **Draft `templates/Gap_Inventory_Worksheet.md`:**
  - A mechanical checklist for auditors.
  - _Check:_ "Is the file format susceptible to ffmpeg/Generative modification?" (Y/N)
  - _Check:_ "Was a hostile observer physically present?" (Y/N)
  - _Trigger:_ If (Modifiable = Y) AND (Hostile = N) → **Force D1**.
