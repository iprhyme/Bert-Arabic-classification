# Bert-Arabic-classification

📋 Project Overview
1️⃣ Dataset
The KALIMAT Corpus contains Arabic texts from the Alwatan newspaper across six categories:
Culture, Economy, International News, Local News, Religion, Sports.
Dataset Statistics:
Culture: 2,495 documents
Economy: 3,265 documents
International: 1,689 documents
Local: 3,237 documents
Religion: 3,475 documents
Sports: 4,095 documents


2️⃣ Key Techniques
✅ Preprocessing: Normalization, noise removal, and special token handling.
✅ Text Classification: Fine-tuned Asafaya BERT (Arabic BERT) for classification tasks.
✅ Text Generation: Fine-tuned Masked Language Model (MLM) to predict contextually appropriate words.
✅ Evaluation: Leveraged BLEU and ROUGE scores for text generation quality.

3️⃣ Model Architecture
Classification Model

Base Model: Asafaya BERT (bert-base-arabic)
Classifier layers:
128-Dense Layer with ReLU activation.
Dropout Layer (0.3) to prevent overfitting.
AdamW Optimizer with a learning rate of 1e-5.


Text Generation Model

Base Model: Asafaya BERT for MLM (bert-base-arabic)
Fine-tuned using a masked language model approach with a 15% token masking rate.
Optimized with AdamW.


📊 Results
🔹 Text Classification
Accuracy: 94%
F1-Score: 94%


🔹 Text Generation
BLEU Score: 70%
ROUGE-1 F1: 91%
ROUGE-2 F1: 88%
ROUGE-L F1: 90%


🟡 Comparison with Traditional ML
Previous ML models achieved:
Accuracy: 81%
F1-Score: 82%
🚀 The BERT-based model demonstrated significant performance gains.
