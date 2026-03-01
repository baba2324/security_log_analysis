[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Python](https://img.shields.io/badge/Python-3.x-blue)](https://www.python.org/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/joonyong-lee-72a392353)

# 🛡️ AI-Based Security Log Anomaly Detection

## 📊 Performance Metrics 
- **Accuracy**: 99.99% (Final system accuracy on CIC-IDS2017 dataset)
- **F1-Score / Precision / Recall**: Near-perfect performance optimized for industrial-grade security

## 🔍 Key Insights
- **Feature Importance**: Identified **Destination Port** as the most critical feature (e.g., Port 46 linkage)
- **Industrial Logic**: Successfully transferred manufacturing defect inspection logic to cybersecurity log analysis

- 
<details>
<summary><b>🔥 🛠️ Challenges & Troubleshooting (Click to Expand)</b></summary>
<br>

The core innovation of this project is **Domain Transfer**—applying manufacturing defect inspection algorithms to cybersecurity log analysis. During this process, I successfully resolved critical structural errors and data challenges.

### 🔴 Phase 1: Resolving 6 Critical Errors (Initial KDD Dataset Transfer)
1. **String Recognition Error:** * **Solution:** Implemented **`Label Encoding`** to convert categorical strings into machine-readable numeric values.
2. **Input Shape Mismatch:** * **Solution:** Applied **`Input Shape Synchronization`** to dynamically expand the pipeline to accommodate 41 features.
3. **Data Type Casting Error:** * **Solution:** Standardized the dataset structure through **`Data Type Casting`** (Float transformation) for stable matrix calculation.
4. **Target Classification Conflict:** * **Solution:** Engineered a **`Binary Classification`** logic, aggregating multiple cyber-attacks into a single 'Attack' label.
5. **Data Integrity Error (NaN/Infinity):** * **Solution:** Implemented robust **`Missing Value Imputation`** to replace garbage data with zero/mean values.
6. **Out of Memory (OOM) Error:** * **Solution:** Optimized memory usage by applying **`Batch Processing`**, splitting the data into manageable chunks for sequential training.

### 🔴 Phase 2: Resolving 2 Structural Errors (CIC-IDS2017 Dataset Upgrade)
1. **Dimensionality (Reshape) Error:** * **Solution:** Architected a larger input layer by expanding the dimension to a **`9x9 Matrix (81 slots)`** to fully encompass all 78 features.
2. **Missing Value (Null) Error in Matrix:** * **Solution:** Deployed **`Zero-Padding`** technique to precisely fill the remaining 3 empty matrix slots with '0', satisfying the rigid structural requirements of the deep learning model.

### 🔴 Phase 3: Model Validation (Handling Data Imbalance)
* **Class Imbalance Issue:** Real-world cybersecurity datasets are highly imbalanced (Normal traffic vastly outnumbers Attack traffic), risking an "Accuracy Paradox" where the AI simply guesses 'Normal' to achieve high accuracy.
* **Solution:** To prove the model's true anomaly detection capability, I evaluated the performance beyond simple accuracy. By focusing on **`F1-Score, Precision, and Recall`**, I validated that the model genuinely detects minority attack classes (like PortScan) without being biased toward the majority class.

</details>

## 🔮 Future Work & Goals
- **Smart Mobility Security**: Planning to extend this anomaly detection logic to **CAN bus and vehicle sensor data**
- **Cross-Industry Expansion**: Aiming to enhance security for next-generation autonomous systems and global industrial IoT platforms
 
## 👤 Contact / About Me
- **Industrial AI & Cybersecurity Specialist**
- **Email**: ddd567640@gmail.com
- - **LinkedIn**: [Jun-yong's Profile](https://www.linkedin.com/in/joonyong-lee-3349003b3?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app )

- **University**: Soonchunhyang University (Information Security)

---
### 📈 Analysis Evidence 


<img width="989" height="790" alt="177216040110416149775824926598" src="https://github.com/user-attachments/assets/01258c88-c5ff-47a7-8149-1729a65b4f0a" />


The results demonstrate that industrial-grade anomaly detection logic can be transferred to security log monitoring systems, achieving stable and high anomaly detection performance.

  
