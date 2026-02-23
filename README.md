# 🛡️ AI-Based Security Log Anomaly Detection
# 🚀 [Version 2.0] Advanced AI Security Detection System
*Upgraded to the latest CIC-IDS2017 dataset for maximized detection rate.*

## 📊 Latest Analysis Summary
- **Target**: PortScan Attack Detection
- **Model**: RandomForest Classifier
- **Final Accuracy**: **99.99%**
- **Key Evidence**: Successfully identified primary entry points (Destination Port 46, Port 20).

---

# 📜 [Version 1.0] Initial Analysis Record
*(The following is the legacy KDD dataset analysis. The system has been upgraded to Version 2.0 above based on these foundational logs.)*


## Overview
This project applies industrial anomaly detection methodologies to cybersecurity by building a deep learning-based security log anomaly detection model.

Instead of treating the task as simple attack classification, the focus was on detecting abnormal patterns within structured network logs, similar to how manufacturing defects are identified in industrial inspection systems.

The experiment evaluates whether industrial CNN-based anomaly detection logic can be effectively transferred into a cybersecurity monitoring context.

---

## Dataset
NSL-KDD Benchmark Dataset  
A structured network traffic dataset containing labeled normal and attack records, commonly used for intrusion detection research.

---

## Security Objective
- Detect anomalous behavior in network logs
- Minimize false negatives (missed attacks)
- Maintain controlled false positive rates to reduce alert fatigue
- Validate feasibility of CNN-based anomaly detection for security monitoring systems

---

## Engineering Approach
- Preprocessed structured security log features for supervised anomaly detection
- Transformed 1D tabular network features into 2D matrix representations compatible with CNN architecture
- Adapted industrial defect detection CNN design into a security anomaly detection pipeline
- Stabilized model after resolving input dimension and architecture inconsistencies
- Evaluated detection performance using precision, recall, and F1-score

---

## Development Context
- Type: Self-Initiated Personal Research
- Development Time: 10-Minute High-Intensity Rapid Prototyping
- Built upon industrial AI anomaly detection training experience (60 hours)

---

## Performance
Accuracy: 0.96  
Precision: 0.96  
Recall: 0.96  
F1-Score: 0.96  

- <img width="729" height="568" alt="image" src="https://github.com/user-attachments/assets/7e08c6d7-fd1d-47c2-90fd-563e6ef34a8a" />


The results demonstrate that industrial-grade anomaly detection logic can be transferred to security log monitoring systems, achieving stable and high anomaly detection performance.

  
