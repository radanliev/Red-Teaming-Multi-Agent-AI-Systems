# Session 4 — Demos: Robustness Visualisation & Differential Privacy (5–10 minutes each)

**Goals:**  
- Visualise overfitting vs robust boundaries (TF Playground).  
- Demonstrate privacy–utility trade-offs (DP demos).

**Tools (browser, zero install):**
- TensorFlow Playground (decision boundary visualiser)  
  https://playground.tensorflow.org/
- DP Demo App — central DP visualiser  
  https://dp.xryptic.com/
- OpenDP DP Wizard — interactive tutorial  
  https://opendp.github.io/dp-wizard/
- Local DP Explorer — client-side DP visualiser  
  https://research.zkwen.site/dpstorytelling/

---

## TF Playground — Overfitting vs Robustness (5–7 minutes)
1. **Open** the playground and select a dataset (e.g. circle).
2. **Start** with a small network (1 hidden layer) — show smooth decision boundary.
3. **Increase** network complexity (4 layers, many neurons) and add noise — display overfit boundary.
4. **Add regularisation** (L2) and re-run — show smoother boundary and improved generalisation.
5. **Explain:** complexity vs robustness tradeoffs; importance of regularisation and validation.

## Differential Privacy — Privacy budget demo (5–8 minutes)
1. **Open** `dp.xryptic.com` (or OpenDP Wizard).
2. **Run** a simple aggregate query without DP — show exact result.
3. **Enable DP** and set epsilon to small (e.g. 0.1) — show noisy result.
4. **Increase epsilon** (e.g. 10) — show result approaches baseline.
5. **Explain:** ε parameter (privacy budget), privacy–utility tradeoff, relevance to model inversion mitigation and compliance.

## Local DP (optional, 3–5 minutes)
1. **Open** the Local DP Explorer.
2. **Adjust epsilon slider** and observe per-device randomisation and aggregate accuracy.
3. **Discuss** federated learning telemetry and supply-chain implications for privacy budgets.

## Teaching notes
- Keep DP explanations intuitive; use numeric examples to show magnitude effects.
- Relate DP choices to regulatory expectations (data minimisation and demonstrable privacy).
