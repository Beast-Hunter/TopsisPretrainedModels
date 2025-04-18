# 📊 Topsis: Pre-Trained Transformer Models for Text Classification

This project evaluates and compares multiple pre-trained Transformer models (BERT, DistilBERT, RoBERTa, ALBERT) on the AG News dataset for multi-class text classification using Hugging Face’s `pipeline`.

The evaluation includes metrics such as:
- ✅ Accuracy
- ⏱ Inference Time

---

## 🧾 Project Contents

- `Topsis_PreTrained_Models.ipynb`: Main notebook containing code to load models, perform classification, and evaluate them.
- ✅ Uses Hugging Face models already fine-tuned on AG News.
- ✅ Uses a subset of 200 test samples for fast comparison.

---

## 📚 Dataset: AG News

[AG News Dataset](https://huggingface.co/datasets/ag_news) contains 120,000 training and 7,600 test samples across four classes:

1. World
2. Sports
3. Business
4. Sci/Tech

This project uses `datasets` to load the test data directly.

---

## 🤖 Models Evaluated

The following models are evaluated using Hugging Face’s `pipeline("text-classification")`:
---

| Model        | Source (HuggingFace)                  |
|--------------|---------------------------------------|
| DeBERTa      | `microsoft/deberta-base`              |
| Electra      | `google/electra-small-discriminator`  |
| Longformer   | `allenai/longformer-base-4096`        |
| MobileBERT   | `google/mobilebert-uncased`           |
| TinyBERT     | `huawei-noah/TinyBERT_General_4L_312D`|

All models are loaded via `transformers.pipeline("text-classification", ...)` for simplicity.

---

## Results 

![TopsisScore](https://github.com/user-attachments/assets/638b6b19-8dd5-4d2a-a556-b1d638277260)

