# ECG Heartbeat Categorization with Deep Learning  

This project implements **deep neural network models** to classify heartbeats from **electrocardiogram (ECG) signals** into different categories of arrhythmia. The dataset combines signals from two well-known sources:  

- **MIT-BIH Arrhythmia Dataset**  
- **PTB Diagnostic ECG Database**  

The goal is to accurately identify abnormal heart rhythms and support the development of **computer-aided diagnosis systems** in cardiology.  

---

## 🎯 Project Goal  

- Train a **deep learning model** to categorize ECG heartbeat signals.  
- Detect and classify arrhythmia types from ECG recordings.  
- Explore **transfer learning** for improving classification accuracy.  
- Provide insights into the most distinguishing features of ECG waveforms.  

---

## 📂 Dataset Overview  

### 1. **MIT-BIH Arrhythmia Dataset**  
- 48 half-hour excerpts of two-channel ECG recordings  
- 47 subjects (recorded between 1975–1979)  
- 109,446 heartbeat samples classified into **5 categories**:  
  - **N** – Normal beats  
  - **S** – Supraventricular ectopic beats  
  - **V** – Ventricular ectopic beats  
  - **F** – Fusion beats  
  - **Q** – Unknown beats  

### 2. **PTB Diagnostic ECG Database**  
- ECG signals including normal and myocardial infarction cases  
- Used for **transfer learning experiments** and model generalization  

### 📌 Key Notes  
- Each sample corresponds to a **single segmented heartbeat**.  
- Preprocessed and standardized for training deep neural networks.  
- Large enough for both **training and validation** of deep learning models.  

---

## 🧭 Workflow  

### 1. Data Preprocessing  
- Load ECG signals and segment into heartbeat samples  
- Normalize amplitude values  
- Encode heartbeat categories (N, S, V, F, Q)  

### 2. Model Development  
- **Baseline Models**: CNN and LSTM for temporal signal classification  
- **Advanced Models**:  
  - Deep CNN for feature extraction  
  - Transfer learning across datasets (MIT-BIH → PTB)  

### 3. Training & Evaluation  
- Train/test split  
- Loss function: Categorical Crossentropy  
- Optimizer: Adam  
- Metrics: Accuracy, F1-score, Confusion Matrix  

### 4. Interpretation  
- Visualize ECG signals with predicted labels  
- Compare predictions vs. ground truth  

---


---

## 🚀 How to Run  

1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/ecg-heartbeat-categorization.git
   cd ecg-heartbeat-categorization
