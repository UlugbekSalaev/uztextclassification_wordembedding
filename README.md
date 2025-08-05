## 📜 Project Description

Uzbek is a **morphologically rich, agglutinative language**, which leads to:  
- **Large vocabulary sizes**  
- **High OOV (Out‑Of‑Vocabulary) rates**  
- **Sparse feature representations** in classical NLP models

This project:  
1. **Preprocesses the dataset** with and without **morphological stemming** (UzMorph).  
2. **Trains and evaluates** the following text classification models:
   - **Bag‑of‑Words (TF‑IDF)**  
   - **Word2Vec embeddings**  
   - **FastText embeddings**  
   - **BERT (monolingual and multilingual)**  
3. **Compares the effect of stemming** on classification performance using macro F1‑score.  

## 📊 Results Summary

| Model        | Original F1 (%) | Stemmed F1 (%) | Gain |
|--------------|-----------------|----------------|------|
| Bag‑of‑Words | 73.4            | 78.2           | +4.8 |
| Word2Vec     | 76.1            | 80.3           | +4.2 |
| FastText     | 78.5            | 83.6           | +5.1 |
| BERT         | 85.2            | **87.4**       | +2.2 |

- **Morphological stemming improves all models**, especially n‑gram and embedding‑based methods.  
- **BERT achieves the highest overall F1‑score** but benefits less from stemming due to subword tokenization.  
