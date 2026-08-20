# Capstone Story & Showcase Kit

## 1. Five-Minute Showcase Demo Outline
* **00:00 - 01:00 (The Problem):** Content teams lack an objective method to identify which high-value URLs are undergoing true search visibility decay versus normal seasonal variance.
* **01:00 - 02:00 (Data & Validation):** Utilized multi-client search performance data. Enforced strict 5-fold `GroupKFold` cross-validation grouped by `client_id` to eliminate cross-domain data leakage.
* **02:00 - 03:00 (Methodology & Results):** Evaluated Random Forest against baseline heuristics. Achieved an out-of-fold ROC-AUC of 0.7844 (+0.076 over baseline).
* **03:00 - 04:00 (Playbook & Guardrails):** Mapped model probabilities into actionable reason codes (`HIGH_VOLUME_DECAY`, `CTR_OPPORTUNITY`). Prohibited automated publishing to ensure human editorial review.
* **04:00 - 05:00 (Limitations & Wrap-up):** Claims are strictly bounded to directional decision support, without causal search algorithm claims.

---

## 2. Employer-Facing Summary 
Built an end-to-end content refresh ranking engine using Python and scikit-learn that prioritizes decaying search pages for editorial intervention. Trained and evaluated Random Forest and Gradient Boosting ensembles across multi-client search performance logs using 5-fold grouped cross-validation to guarantee zero intra-domain data leakage. Delivered a validated out-of-fold ROC-AUC of 0.7844 (+0.076 over baseline) and packaged the results into an operational content action playbook with human-in-the-loop review guardrails.

---

## 3. Social / LinkedIn Post
How do you build an ML ranking engine for search decay without fooling yourself with data leakage?

In search performance datasets, pages from the same client domain share technical structures and domain authority. Standard random K-fold splits leak domain context between train and test sets, artificially inflating model accuracy.

During the FlyRank Machine Learning Internship, I built a content refresh prioritization engine using 5-fold `GroupKFold` validation grouped by client domains. Evaluating strictly on unseen client accounts, our Random Forest classifier achieved a validated ROC-AUC of 0.7844 (vs 0.7082 baseline).

Check out the live interactive research paper and reproducible notebooks:
🔗 Live Paper: https://mahmoonakhan.github.io/flyrank-ml-internship/
💻 GitHub: https://github.com/mahmoonakhan/flyrank-ml-internship

#MachineLearning #DataScience #SEO #ModelValidation #DataLeakage #Python
