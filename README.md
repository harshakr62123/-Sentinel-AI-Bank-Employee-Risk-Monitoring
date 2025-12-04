# 🕵️‍♂️ Sentinel-AI: Bank Employee Risk Monitoring

A multi-model AI system for monitoring employee activity in banking environments.  
This project simulates real-time behavior patterns such as transaction frequency, access levels, login hours, and location data — then uses **five different deep learning models** to detect anomalies and risk activity.

Built using **Streamlit + PyTorch + Graph Neural Networks**.

---

## 🚀 Features

- ✔️ **Synthetic Behavior Simulation** of multiple employees  
- ✔️ **Real-time anomaly scoring** per employee  
- ✔️ **Model ensemble monitoring**
- ✔️ **Graph visualization using GNNs**  
- ✔️ **Interactive UI dashboard** for risk analytics  
- ✔️ **Complete explainability via multi-score risk display**

---

## 🧠 AI Models Included

This system uses **five independent anomaly detection models**, loaded and executed in parallel:

- **Time-Series Transformer** – detects sequential behavior risk  
- **Sequence VAE** – reconstruction error anomaly detection  
- **Contrastive Representation Encoder** – unsupervised feature learning  
- **Temporal Graph Neural Network (GCN)** – employee-resource graph insights  
- **Tabular MLP Classifier** – daily summary risk classifier  

Models are defined in `app.py` and loaded from the `/all_five_models/trained_models/` folder using a safe loader. :contentReference[oaicite:2]{index=2}

---

## 🖥️ UI Overview (Streamlit)

- Slider to choose **number of simulated employees**
- One-click **Run Simulation** button
- Table showing:

  - Transformer risk score  
  - VAE reconstruction loss  
  - Contrastive anomaly score  
  - Tabular risk probability  

- Histogram of risk score distributions  
- Employee graph visualization using `networkx`

---

## 📂 Project Structure

