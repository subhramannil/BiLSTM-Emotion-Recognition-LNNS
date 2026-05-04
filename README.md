# Affective Computing & Sentiment Analysis via BiLSTM

[![Kaggle](https://img.shields.io/badge/Kaggle-Notebook-blue?logo=kaggle)](https://www.kaggle.com/code/subhranilwayne/trustworthy-ai)
## 📌 Project Overview
This repository contains the code and methodology for an advanced deep learning model focused on Affective Computing and Sentiment Analysis. The core of the project utilizes a **Bidirectional Long Short-Term Memory (BiLSTM)** architecture to effectively capture sequential data dependencies and temporal context in textual data. 

To ensure the model's predictions are interpretable and transparent, **Explainable AI (XAI)** methodologies were integrated to evaluate and visualize the decision-making process.

**Note:** The research and methodology developed in this repository culminated in a peer-reviewed research paper published in *Springer LNNS (Lecture Notes in Networks and Systems)*.

## 🚀 Model Architecture & Pipeline
*   **Deep Learning Framework:** TensorFlow / Keras (Accelerated via Kaggle GPUs)
*   **Core Architecture:** BiLSTM-64 with Bahdanau Attention
*   **Explainability (XAI):** LIME Token Attribution, Attention Weight Visualization
*   **Robustness Evaluation:** Targeted perturbation attacks (tested against syntactic noise and semantic reversals)
*   **Validation Method:** 5-fold cross-validation

## 📊 Datasets & Performance
The architecture was rigorously benchmarked across multiple domains to demonstrate strong generalization, achieving competitive performance against TF-IDF baselines.

*   **IMDb Dataset:** 87.98% Accuracy (F1-Score: 0.88)
*   **Amazon Dataset:** 87.65% Accuracy (F1-Score: 0.88)
*   **Cross-Validation:** Demonstrated consistent generalization with a high accuracy of **0.8816 ± 0.0068**.
  
## 💻 How to Run (Kaggle Integration)
Because this model requires significant compute power for training, the primary codebase is hosted and executed on Kaggle.

1.  **View the Live Notebook:** You can view the full code, training logs, and XAI visualizations directly on Kaggle here: [Insert Your Kaggle Notebook Link Here]
2.  **Run Locally:** If you wish to run the `.ipynb` file provided in this repository locally, ensure you have Jupyter installed and run the following to install dependencies:
    ```bash
    pip install tensorflow keras nltk scikit-learn pandas numpy matplotlib
    ```
## 🔮 Future Scope
While the current architecture is highly robust against syntactic noise, future research directions include:
*   Integrating pre-trained contextual word embeddings (BERT, RoBERTa) to handle large semantic reversals.
*   Applying adversarial training to mitigate vulnerabilities.
*   Extending the approach to aspect-level and multilingual sentiment analysis.
*   Applying the robustness protocol to automatic attack methodologies like TextFooler and BERT-Attack.

### Ablation Study Results
An ablation study confirmed the critical importance of the attention mechanism:
*   **BiLSTM-64 + Attention:** 0.8818
*   **BiLSTM-64 (No Attention):** 0.8810

## 📄 Citation
If you utilize this framework for auditing NLP systems or find our research helpful, please cite our Springer LNNS publication:
> Subhranil Das, et al. **"Trustworthy Sentiment Analysis: A Lightweight BiLSTM with Custom Attention and XAI Integration"**. *Lecture Notes in Networks and Systems (LNNS), Springer*, 2026.

## 👨‍💻 Author
**Subhranil Das** 
*   https://www.kaggle.com/subhranilwayne
