---

## 2) `SESSIONS/SESSION1_DEMO.md`
Purpose: short, repeatable teacher script for Session 1 demo (5–8 minutes).

```markdown
# Session 1 — Demo: Real-Time Evasion Attack (5–8 minutes)

**Goal:** Demonstrate how small changes to the input/environment can cause misclassification (evasion).

**Tools (browser, zero install):**
- Primary: TensorFlow.js Webcam Transfer Learning  
  https://storage.googleapis.com/tfjs-examples/webcam-transfer-learning/dist/index.html
- Alternative (if bandwidth or browser issues): Google Teachable Machine  
  https://teachablemachine.withgoogle.com/

---

## Pre-class checklist (1–2 minutes)
- Ensure presenter laptop has a webcam and stable Wi-Fi.
- Open the TF.js demo in the browser tab and keep Teachable Machine as fallback.

## Demo script (timed)
1. **Intro (30s):** Explain the objective — show how small input changes cause misclassification.
2. **Train quick classifier (60–90s):**
   - Create three classes: `Phone`, `Notebook`, `Empty`.
   - Capture ~20–30s of examples per class (fast capture).
3. **Verify baseline (30s):**
   - Show classifier correctly recognising objects.
4. **Evasion manipulations (2–3 min):**
   - Change lighting (dim/bright) — note confidence shift.
   - Rotate the object (angle change) — note instability.
   - Place patterned background behind object — note misclassification.
   - Partially occlude (cover part of object) — demonstrate mislabel.
5. **Explain (60s):**
   - Connect the observations to decision boundary fragility.
   - Map to attack surface: input channel + preprocessing vulnerabilities.
6. **Wrap (30s):**
   - Tie into next activity: using MITRE ATLAS to map attack vectors.

## Teaching notes
- Keep it visual — audience must see confidence/probability changes.
- Highlight that no system compromise was necessary; this is an inference-time evasion.
- If webcam is unavailable, use pre-recorded video frames and feed them.
