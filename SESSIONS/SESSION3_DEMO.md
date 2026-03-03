# Session 3 — Demo: NLP Adversarial Perturbation (5–8 minutes)

**Goal:** Demonstrate how lexical perturbations cause misclassification of sentiment models.

**Tool (browser, zero install):**
- Hugging Face model interface — CardiffNLP Twitter RoBERTa sentiment  
  https://huggingface.co/cardiffnlp/twitter-roberta-base-sentiment

---

## Pre-class checklist
- Open the Hugging Face model inference page in a browser tab.
- Prepare baseline sentence(s) and variants.

## Demo script (timed)
1. **Intro (30s):** Explain black-box adversarial testing (no model internals).
2. **Baseline test (20s):**
   - Input: `The service was excellent and efficient.`  
   - Record predicted sentiment and confidence.
3. **Perturbations (3–4 min):**
   - Typos: `The service was exellent and eficient.` — observe prediction.
   - Negation: `The service was not excellent and efficient.` — observe flip.
   - Sarcasm: `Oh great, the best service ever… not.` — observe failure modes.
   - Unicode homoglyphs: replace 'i' with 'ı' or 'l' with '1' — observe model behaviour.
4. **Explain (60s):**
   - Show why semantic understanding is brittle.
   - Discuss how this informs adversarial training and sanitisation.

## Teaching notes
- This is a black-box demo: emphasise observational testing methods and logging.
- If time permits, show how simple sanitisation (strip unicode, normalise) changes outcomes.
