# Enhanced Transformer-Based Sentiment Analysis using Multi-Task Learning

A research project that extends transformer-based sentiment analysis by introducing multi-task learning, sarcasm detection, aspect-based sentiment analysis, emotion detection, and explainability.

This work was developed as part of an academic research project and is based on experiments conducted on the Amazon Reviews 2023 (All-Beauty) dataset.

---

## Project Highlights

- Multi-task learning for sentiment classification and sarcasm detection
- Five-class sentiment prediction
- Aspect-Based Sentiment Analysis (ABSA)
- Emotion intensity detection
- SHAP-based model explainability
- Sliding-window processing for long reviews
- Confidence-weighted loss for noisy labels

---

## Model Architecture

- Backbone: **Microsoft DeBERTa-v3-base**
- Multi-task learning framework
- Shared transformer encoder
- Sentiment Classification Head
- Sarcasm Detection Head

Additional inference modules:

- Aspect-Based Sentiment Analysis
- Emotion Detection (DistilRoBERTa)
- SHAP Explainability

---

## Dataset

- Amazon Reviews 2023 (All-Beauty)
- Approximately 50,000 product reviews
- Stratified Train/Validation/Test split (70/15/15)

---

## Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- Pandas
- NumPy
- Scikit-learn
- SHAP
- Matplotlib
- VADER Sentiment

---

## Repository Contents

| File | Description |
|------|-------------|
| `improved_sentiment.ipynb` | Final enhanced transformer implementation |
| `NLP_09.ipynb` | Data preprocessing and intermediate experiments |
| `NLP_Exp10.ipynb` | Baseline transformer implementation |
| `IEEE_Sentiment_Paper.pdf` | Research paper describing the methodology and results |

---

## Key Improvements over Baseline

- Upgraded from RoBERTa to DeBERTa-v3-base
- Binary → Five-class sentiment classification
- Added sarcasm detection using multi-task learning
- Added Aspect-Based Sentiment Analysis
- Added emotion recognition
- Added SHAP explainability
- Improved handling of long reviews using sliding-window tokenization

---

## Performance

| Metric | Score |
|---------|--------|
| Binary Accuracy | **94.59%** |
| Precision | **96.77%** |
| Recall | **95.57%** |
| F1 Score | **96.17%** |
| ROC-AUC | **98.34%** |
| Five-Class Accuracy | **72.52%** |

---

## Future Work

- FastAPI deployment
- Web application interface
- Multimodal sentiment analysis
- Cross-domain evaluation
- Human-annotated sarcasm dataset
- Model optimization

---

## Authors

- Ninad Gawade
- Soham Gurav
- Pranav Patil

---

## Citation

If you use this work, please cite the accompanying research paper included in this repository.
