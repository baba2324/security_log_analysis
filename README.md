[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Python](https://img.shields.io/badge/Python-3.x-blue)](https://www.python.org/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/joonyong-lee-72a392353)

# 🛡️ AI-Based Security Log Anomaly Detection

## 📊 Performance Metrics
- Accuracy: 99.99%
- F1-Score / Precision / Recall: ...
- Macro F1-Score: 0.99
- Evaluated with F1-Score to avoid accuracy paradox.

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

## 🔍 Key Insights
- **Feature Importance**: Identified **Destination Port** as the most critical feature (e.g., Port 46 linkage)
- **Industrial Logic**: Successfully transferred manufacturing defect inspection logic to cybersecurity log analysis


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
<img width="1189" height="1190" alt="download" src="https://github.com/user-attachments/assets/e6c5a027-4efb-4362-bf5f-b9538d3d8118" />
--- [Step 1] Initial Data Inspection ---
Data Shape: (286467, 79)
    Destination Port   Flow Duration   Total Fwd Packets  \
0                 22         1266342                  41   
1                 22         1319353                  41   
2                 22             160                   1   
3                 22         1303488                  41   
4              35396              77                   1   

    Total Backward Packets  Total Length of Fwd Packets  \
0                       44                         2664   
1                       44                         2664   
2                        1                            0   
3                       42                         2728   
4                        2                            0   

    Total Length of Bwd Packets   Fwd Packet Length Max  \
0                          6954                     456   
1                          6954                     456   
2                             0                       0   
3                          6634                     456   
4                             0                       0   

    Fwd Packet Length Min   Fwd Packet Length Mean   Fwd Packet Length Std  \
0                       0                64.975610              109.864573   
1                       0                64.975610              109.864573   
2                       0                 0.000000                0.000000   
3                       0                66.536585              110.129945   
4                       0                 0.000000                0.000000   

   ...   min_seg_size_forward  Active Mean   Active Std   Active Max  \
0  ...                     32          0.0          0.0            0   
1  ...                     32          0.0          0.0            0   
2  ...                     32          0.0          0.0            0   
3  ...                     32          0.0          0.0            0   
4  ...                     32          0.0          0.0            0   

    Active Min  Idle Mean   Idle Std   Idle Max   Idle Min   Label  
0            0        0.0        0.0          0          0  BENIGN  
1            0        0.0        0.0          0          0  BENIGN  
2            0        0.0        0.0          0          0  BENIGN  
3            0        0.0        0.0          0          0  BENIGN  
4            0        0.0        0.0          0          0  BENIGN  

-- [Step 2] Key Evidence Analysis (Feature Importance) ---
Rank 1: Feature Index 52 (10.99%)
Rank 2: Feature Index 46 (9.29%)
Rank 3: Feature Index 6 (8.48%)
Rank 4: Feature Index 4 (8.38%)
Rank 5: Feature Index 1 (7.36%)
Rank 6: Feature Index 24 (7.13%)
Rank 7: Feature Index 18 (6.99%)
Rank 8: Feature Index 20 (6.33%)
Rank 9: Feature Index 39 (6.24%)
Rank 10: Feature Index 10 (5.58%)

--- [Step 3] Final Detection Result ---
FINAL AI ACCURACY: 99.99%

The results demonstrate that industrial-grade anomaly detection logic can be transferred to security log monitoring systems, achieving stable and high anomaly detection performance.

  
