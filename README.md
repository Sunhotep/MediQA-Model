

# **Bert-like Models Feasibility Exploration on Medical Short-Text Q&A Tasks**

In this project, I explored the feasibility of leveraging Bert-like models for machine reading comprehension (MRC) in specialized domains, specifically medical short-text Q&A tasks. The work focused on blending different classes of Bert-like models to improve performance when handling small medical datasets extracted from medical illustration videos.

Key accomplishments and findings include:

- **Model Exploration:** Selected and blended various Bert-like models to enhance performance on small text data from medical contexts.
- **Field-Specific MRC Model Training:** Attempted to train a specialized MRC model tailored to medical Q&A tasks, adjusting hyperparameters and evaluating performance.
- **Performance Testing:** Rigorous testing and evaluation of the model’s ability to comprehend and respond to medical questions.
- **Skill Development:** Improved my Natural Language Processing (NLP) capabilities by working closely with my supervisor and Ph.D. students. Gained a deeper understanding of deep learning (DL) and reinforcement learning (RL) formulas.
- **Research Contribution:** This research contributed to the Ningbo 2025 Science and Technology Innovation Program, advancing knowledge in the application of Bert-like models to medical tasks.

---

### **Prediction Steps**

To execute predictions with the trained model, follow these steps:

1. **Run the Prediction Scripts:**
   - For **关黄母颗粒** question-answering prediction:
     ```bash
     sh test_bert_ghm.sh
     ```
   - For **丁苯酚** question-answering prediction:
     ```bash
     sh test_bert_dbf.sh
     ```

2. **Adjust Storage Path**: When executing the script, make sure to change the storage address as prompted by `metrics.py` at line 730.

---

### **Parameters Overview**

- **`--lm`**: Specify the folder containing the pre-trained model to be loaded.
- **`--do_train`**: Activate training mode.
- **`--evaluate_during_training`**: Enable validation during training.
- **`--do_test`**: Activate prediction mode.
- **`--version_2_with_negative`**: Adapt the model for datasets that may contain both questions with answers and questions without answers.
- **`--threads`**: Specify the number of threads for data processing.
