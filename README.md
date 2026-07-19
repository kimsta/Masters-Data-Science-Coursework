# Kim Ståhlberg | Data Science Portfolio

Data Scientist with an MSc in Data Science (University of Helsinki, 2026) and a BSc in Statistics. This repository showcases production-ready architecture, applied machine learning, graph analytics, and statistical modeling.

**Contact:** [stahlberg.kim@gmail.com](mailto:stahlberg.kim@gmail.com)

---

## Featured Projects

### 1. Algorithmic Trade-Offs in Multi-Modal Travel Cost Computation (Master's Thesis)
*Grade: 5/5 | University of Helsinki*
A systems-level trade-off analysis evaluating classical graph algorithms against neural approximation for large-scale routing across a historical, multi-modal network.
* **Architecture:** Engineered a Siamese Interaction Network for Regression (SINfR) to reframe memory-bound graph traversal as a parallelized tensor operation.
* **Performance:** Bypassed the $O(N^2)$ memory constraints of traditional CPU-bound routing, reducing peak memory usage to a constant ~1 GB while achieving a throughput of ~5.8 million paths per second on GPU.
* **Repository:** [View Technical Specs & Research Link](https://github.com/kimsta/historical-multimodal-routing-msc-thesis)
* **Tech Stack:** Python, PyTorch, GeoPandas, NetworkX, NetworKit, pandana.

### 2. Quantitative Integration Engine
A full-stack, polymorphic Monte Carlo integration engine built to dynamically evaluate complex probability mixture models without deterministic numerical quadrature.
* **Backend:** Built with FastAPI and SciPy, utilizing strictly typed Pydantic V2 Discriminated Unions to enforce mathematical parameters before execution.
* **Frontend & Deployment:** Decoupled React/Vite SPA with Plotly.js visualization, orchestrated via a multi-stage Docker build and unified bridged network.
* **Repository:** [View and run the code here](https://github.com/kimsta/quant-integration-engine)
* **Tech Stack:** FastAPI, React, Docker, SciPy, Pydantic.

### 3. Algorithmic Fairness Audit: Healthcare Risk Prediction
A rigorous fairness audit and mitigation pipeline for a Heart Failure prediction model, designed to identify and correct safety disparities in medical diagnostics.
* **The Problem:** Identified a critical 4.5x Safety Disparity for young female patients compared to older males via intersectional auditing.
* **The Solution:** Engineered a hybrid mitigation strategy using Decoupled Classifiers and Threshold Tuning, reducing safety risk by ~50% without requiring additional data collection.
* **Repository:** [View and run the code here](https://github.com/kimsta/fairness_bias_audit)
* **Tech Stack:** Python, Scikit-learn, Pandas, Fairness Metrics.

### 4. Privacy-Preserving ML & Membership Inference Defense
A security audit demonstrating data leakage in Neural Networks and implementing Differential Privacy (DP-SGD) to secure the model against attacks.
* **The Attack:** Simulated a Membership Inference Attack (MIA) via a counterfactual "Shadow Model," proving standard SGD models leak critical training data.
* **The Defense:** Implemented Differential Privacy (Opacus, $\epsilon=1.0$), successfully masking individual data points (Privacy Gap: ~0.00) while maintaining >90% validation accuracy.
* **Repository:** [View and run the code here](https://github.com/kimsta/privacy_audit_mia)
* **Tech Stack:** Python, PyTorch, Opacus, Scikit-learn.

### 5. Automated NLP Pipeline for Text Classification (VATT)
Designed and delivered a complete two-stage NLP pipeline to classify thousands of unstructured, Finnish-language free-form text entries for a public research institute.
* **Architecture:** Programmatic labeling utilizing the Google Gemini API to bootstrap training data for custom `spaCy` models.
* **Outcome:** The first-stage binary filter achieved a 93% F1-score, and the final multi-label classifier achieved a ~90% F1-score, automating a massive manual structuring task.
* **Repository:** [View Public Sentiment Demo here](https://github.com/kimsta/spaCy_NLP_Sentiment_Demo)
* **Tech Stack:** Python, spaCy, Scikit-learn, Google Gemini API.

### 6. Automated ANOVA Pipeline (BioMedicum Helsinki)
Architected an automated statistical pipeline in R for the Koistinaho Lab to process complex experimental biomedical data.
* **Architecture:** Developed the core analytics engine and data validation logic to automatically select and execute distinct ANOVA models based on dynamic user input.
* **Repository:** [View Core Logic Demo here](https://github.com/kimsta/R_Automated_ANOVA)
* **Tech Stack:** R, Tidyverse, rstatix, broom, R Shiny.

### 7. Padel Analytics & Match Predictor (Interactive Dashboard)
An end-to-end data pipeline, statistical inference engine, and interactive dashboard built to quantify player skill and predict pairwise match outcomes from sparse amateur sports data.
* **Architecture:** Custom ETL pipeline routing raw text scores into a local SQLite database, serving an interactive `Shiny` frontend.
* **Statistical Modeling:** Implemented a Bradley-Terry model to predict pairwise outcomes. Applied Penalized Ridge Regression (L2 penalty) via `tidymodels` to solve complete separation and multicollinearity inherent in sparse datasets. 
* **Inference:** Utilized Beta-Binomial models for Bayesian updating to quantify the mathematical certainty of true skill levels across limited sample sizes.
* **Repository:** [View Technical Specs Here](https://github.com/kimsta/Padel_Project) | **Live App:** [View Interactive Dashboard](https://kimst.shinyapps.io/padel-stats/)
* **Tech Stack:** R, Shiny, SQLite, tidymodels, glmnet.

---

## Technical Skills

* **Languages:** Python, R, SQL
* **Deep Learning & Privacy:** PyTorch, PyTorch Geometric, Opacus
* **Graph & Geospatial:** GeoPandas, NetworkX, NetworKit, pandana, igraph, graph-tool
* **ML & Advanced Statistics:** Scikit-learn, SciPy, statsmodels, tidymodels, glmnet, spaCy
* **Data Engineering & Databases:** FastAPI, Pydantic, SQLite, Docker, Kubernetes, Spark, MLflow
* **Frontend & Interactive UI:** React, Vite, Shiny, bslib, Plotly.js, DT, Matplotlib
* **Version Control:** Git, GitHub

---
*Copyright (c) 2026 Kim Ståhlberg. Licensed under the MIT License.*
