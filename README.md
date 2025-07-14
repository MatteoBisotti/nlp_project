# NLP Project - Politics of emotions or propaganda?

Bisotti Matteo 66144A

---

Final project for the Natural Language Processing course - University of Milan, Computer Science Department.

This work aims at analyzing the use of emotions in political speeches from European Parliament. Specifically, the task involves the fine-tuning of a pre-trained model RoBERTa from hugging face on an emotional dataset GoEmotions to classify emotions and the evaluation of model's performance using common metrics, including precision, recall and F1-score. 

A particular focus is on how emotions are distributed across different political parties and historical periods, and the apply of an explainability technique, specifically SHAP, to understand why model made certain predictions and to better understand which words contributed the most to the emotional classification.

## Repository structure

```bash
    ├── data/   
        ├── full_dataset                # GoEmotions raw data
            ├── goemotions_1.csv        
            ├── goemotions_2.csv
            └── goemotions_3.csv
        ├── dataset.csv                 # original GoEmotions
        ├── dataset_politics_preds.csv  # eu_debates with inference
        ├── final_dataset.csv           # GoEmotions with preprocessing 
        ├── global_shap_politics.csv    # dataset global shap values on eu_debates
        ├── global_shap.csv             # dataset global shap values on GoEMotions
        └── politics_texts.csv          # dataset eu_debates     
    └── notebooks/
        ├── dataset_politics.ipynb      # preprocessing operations on eu_debates
        ├── model_RoBERTa.ipynb         # fine-tuning RoBERTa with explainability on GoEmotions
        ├── politics_analysis.ipynb     # analysis on eu_debates
        ├── politics_inference.ipynb    # inference on eu_debates
        └── preprocessing.ipynb         # preprocessing operations on GoEmotions

```
