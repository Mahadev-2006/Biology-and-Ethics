**🧬 Deep Learning-Based Off-Target Prediction for CRISPR-Cas9**

**❓ Why do unintended DNA edits still occur in CRISPR systems?**
CRISPR-Cas9 has transformed genome editing with its precision and efficiency. However, off-target effects—unintended DNA cuts—remain a critical limitation, potentially leading to harmful mutations and reduced therapeutic safety.

This project addresses that challenge by introducing a deep learning-based predictive system to identify off-target activity before it occurs.

**🚀 Project Overview**
This work presents a Feedforward Neural Network (FNN) model designed to predict CRISPR-Cas9 off-target effects with high efficiency.

Novel 8×23 image-like encoding of DNA and gRNA sequences
Trained on 50,000+ samples from CRISPOR and GUIDE-seq datasets
Achieved ROC-AUC: 0.82 with strong classification performance
Outperformed traditional ML baselines

The system provides a fast, scalable, and interpretable approach to improving CRISPR safety.

**🧠 Key Features**
🔬 Deep learning-based off-target prediction
🧩 Custom sequence encoding (8×23 matrix representation)
⚖️ Handles class imbalance effectively
📊 Multi-model comparison (FNN, CNN, LSTM, Random Forest)
🎯 High precision and recall across models

**📂 Dataset**
The model is trained using:
CRISPOR Dataset
GUIDE-seq Dataset
These datasets provide experimentally validated off-target sites and are widely used in CRISPR research .

**⚙️ Methodology**

**🔹 Data Processing**
DNA sequences (23 base pairs) converted into 8-bit one-hot encoded matrices
Combined datasets for improved generalization

**🔹 Model Architecture (FNN)**
Input: 184 features (8 × 23 encoding)
Hidden Layers: 3 Dense layers (ReLU)
Output: Sigmoid (Binary Classification)
Loss: Binary Crossentropy
Optimizer: Adam

**🔹 Other Models Evaluated**
CNN (captures local motifs)
LSTM (captures sequence dependencies)
Random Forest (baseline model)

**📊 Results**
Model	Accuracy	Precision	Recall	F1 Score
FNN	87%	0.87	0.85	0.85
CNN	86%	0.85	0.85	0.85
LSTM	84%	0.83	0.84	0.83
Random Forest	84%	0.83	0.83	0.83
FNN achieved the best overall performance
ROC-AUC score: 0.82
Robust performance despite class imbalance
(Refer to ROC curves and comparison charts in the project report for detailed visualization )

