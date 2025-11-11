# FaceMatch-AntiFraud-SNN
Identity fraud is a growing threat in social welfare systems. This project develops a deep-learning identity verification system using Siamese Neural Networks (SNN) to detect impersonation, duplicates, and fraudulent SRD grant applications.
A baseline CNN classifier was implemented for comparison under identical training conditions.
PROJECT OVERVIEW
This system verifies whether two facial images belong to the same person, using:
-ResNet50 to extract deep facial embeddings
-Siamese Neural Network (SNN) with ArcFace-style margin loss
-Hard negative mining for stronger discriminatory capability
-Threshold-tuned decision logic (0.4 / 0.5 / 0.6 / 0.8)
-Evaluation on LFW (Labelled Faces in the Wild)
The SNN shows significantly stronger performance for fraud detection compared to the CNN baseline.
FEATURES
✅ Face preprocessing (resize, normalization, RGB conversion)
✅ ResNet50 embedding model
✅ Cosine-similarity SNN with margin
✅ Contrastive/ArcFace-style loss
✅ Hard negative pair generation
✅ Full evaluation suite
-Accuracy
-Precision
-Recall
-F1-Score
-ROC-AUC
-Confusion Matrix
-Threshold testing
✅ Model comparison: CNN vs SNN
✅ Visualization tools (heatmaps, ROC curves, bar charts)
📊 Performance Summary
| Metric    | CNN   | SNN       |
| --------- | ----- | --------- |
| Accuracy  | 0.736 | **0.832** |
| Precision | 0.514 | **0.946** |
| Recall    | 0.158 | **0.392** |
| F1-Score  | 0.241 | **0.554** |
| AUC       | 0.646 | **0.650** |
SNN beats CNN on every metric, especially precision, which is critical in fraud detection (fewer false acceptances).
🛠️ Tech Stack
-Python
-TensorFlow / Keras
-OpenCV
-NumPy / Pandas
-Matplotlib / Seaborn
-LFW Dataset
🎓 Academic Context
This project was developed as part of a research study on:
AI-driven biometric identity verification for youth SRD grant fraud detection in South Africa.
