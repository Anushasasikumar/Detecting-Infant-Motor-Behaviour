# Detecting-Infant-Motor-Behaviour

## 📌 Project Overview
Built an infant health classification model using CNN+LSTM and CNN+Transformer architectures to detect normal vs. abnormal infants. Prioritized minimizing false negatives to ensure high-risk infants are  accurately identified.

## Dataset Description
This dataset contains 70 infant video recordings (.mp4) along with a corresponding label file that includes attributes such as Infant_ID, Name, Class, Weight (kg), and Height (cm). It provides both visual and tabular information necessary for analyzing infant health classification.

## 🧠 Key Objectives
   - Preprocess infant movement videos for behaviour classification.
   - Use Mediapipe to detect and visualize key body landmarks
   - Extract frame-level features and build deep learning models for classification.
   - Identify infants as normal or abnormal based on movement patterns.

## 🛠️ Tools & Technologies
- Programming Language: Python
- Libraries Used: Mediapipe, OpenCV, NumPy, Pandas, Matplotlib, TensorFlow/Keras
- Deep Learning Methods:
  - CNN + LSTM (for spatial–temporal sequence modeling)
  - CNN + Transformer (for attention-based movement understanding)

## 🎥 Data Preprocessing & Feature Extraction
- Loaded and preprocessed infant video recordings (.mp4 format).
- Extracted individual frames using OpenCV and resized them for model input.
- Applied Mediapipe Pose to detect body keypoints and visualize skeletal landmarks.
- Generated landmark coordinates and movement patterns as input features.
- Constructed sequential datasets suitable for temporal deep learning models.

## 🤖 Deep Learning Workflow
- Designed CNN-based feature extractors to capture spatial information from frames.
- Integrated LSTM layers to learn long-term temporal movement patterns.
- Built a CNN + Transformer model to leverage attention for detecting subtle motion differences.
- Trained and validated the models on labelled infant data (normal vs abnormal).

## 📊 Evaluation Metrics

Evaluated performance using:
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Compared model results to determine which architecture captured infant movement behaviour more effectively.

## ✅ Conclusion

This project demonstrates a complete deep-learning-based pipeline for analyzing infant movement behaviour using video data. By combining Mediapipe landmark extraction, CNN+LSTM, and CNN+Transformer,the system effectively identifies subtle movement patterns to classify infants as normal or abnormal. The evaluation metrics provide clear insights into model performance, supporting further improvements and potential real-world clinical applications.
