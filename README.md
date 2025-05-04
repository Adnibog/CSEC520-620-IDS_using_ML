#**Final Project - CSEC 520/620: Intrusion Detection using Machine Learning**
Team Name: Inferno  
Dataset: [2017-SUEE Dataset (SUEE1.pcap)](https://github.com/vs-uulm/2017-SUEE-data-set)  


## 📌 Project Overview

This project applies machine learning techniques to detect DoS-based intrusions in network traffic captured in the **SUEE1** PCAP file. The traffic includes anonymized web server connections (TCP ports 80 and 443) along with synthetic attacks such as **slowloris**, **slowhttptest**, and **slowloris-ng**.

### Pipeline Summary:
- Packet parsing and feature extraction using Scapy
- Data preprocessing, labeling, and cleaning
- Exploratory data analysis and visualization
- Feature importance analysis and clustering
- Model training and evaluation (baseline and ensemble methods)

> 🔧 **Note:**  
> - Mount **Google Drive** before running the notebook to access the PCAP file and store results.  
> - Install Scapy using `!pip install scapy` since it's not included in Colab by default.  
> - Run all cells **sequentially** to avoid runtime errors.  
> - The code cells for **loading and processing the PCAP file** and **data preprocessing** are **intentionally commented out**.  
>   - These steps are computationally expensive and only need to be run once.  
>   - After generating and saving the processed CSV file, you can skip these cells in future runs for faster execution.  
>   - Uncomment and run them only if you need to reprocess the raw PCAP data.


## 📁 Dataset Description

- **Source:** Ulm University – 2017 SUEE Dataset  
- **File Used:** `SUEE1.pcap`  
- **Traffic Type:** TCP (HTTP and HTTPS)  
- **Classes:** Benign vs. DoS Attack  
- **Packets:** ~2.09 million  

## ⚙️ Tools & Technologies

| Tool                | Purpose                                  |
|---------------------|------------------------------------------|
| **Google Colab**    | Development environment                  |
| **Scapy**           | PCAP parsing, feature extraction         |
| **Pandas, NumPy**   | Data manipulation                        |
| **Matplotlib, Seaborn** | Visualization                      |
| **Scikit-learn**    | ML models, evaluation, clustering        |
