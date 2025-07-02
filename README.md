# Comparative Study of Graph Neural Networks for Intrusion Detection on the UNSW-NB15 Dataset

This project presents a comparative analysis of MLP, GCN, GAT, and an advanced GAT model on the UNSW-NB15 cybersecurity dataset. It applies graph-based learning techniques for detecting anomalous network activity using node-level classification and feature engineering.

## 🌟 Objective

To evaluate and compare the performance of Graph Neural Network models on the UNSW-NB15 dataset, specifically for intrusion detection using metrics like accuracy, precision, recall, and F1-score.

## 📊 Models Compared

### ✅ MLP (Multilayer Perceptron)

Acts as a baseline non-graph neural model.

Performance used to benchmark GNN effectiveness.

### ✅ GCN (Graph Convolutional Network)

Learns via neighborhood aggregation from a constructed KNN graph.

Demonstrates improved structural learning over MLP.

### ✅ GAT (Graph Attention Network)

Incorporates attention mechanisms to assign learnable weights to neighbor nodes.

Offers interpretability and finer control.

### ✅ Advanced GAT

Includes enhancements like:

Residual connections

Batch normalization

Deeper architecture

Outperforms standard GAT in precision and recall.

## 🧪 Dataset

UNSW-NB15: A modern benchmark dataset for intrusion detection.

Features: 49 attributes (both categorical and numerical).

Preprocessing includes:

Label encoding of categorical features

Standardization using StandardScaler

SMOTE for oversampling the minority class

## 🔧 Setup & Installation

### 📦 Requirements

Python 3.8+

PyTorch

PyTorch Geometric

Scikit-learn

Pandas, Matplotlib, Seaborn

Install all dependencies:

pip install -r requirements.txt

## 🚀 How to Run

### Launch the notebook
jupyter notebook "Comparative Study of GNN for UNSW-NB15.ipynb"

Follow the sequential cells to:

Load and preprocess the data

Create graph representations

Train and evaluate MLP, GCN, GAT, and Advanced GAT

Visualise results

## 📈 Results Summary

Model

Accuracy

MLP

0.8517

GCN

0.8754

GAT

0.8524

Advanced GAT

### ✅ Best performance (improved precision/recall)

Conclusion: Advanced GAT outperforms standard GAT and MLP, and rivals or surpasses GCN in overall classification metrics.

## 🔬 Ablation Studies

The impact of each architectural enhancement on GAT was tested:

GAT w/o Residual Connections

GAT w/o Normalization Layers

These were evaluated independently to quantify their influence on model robustness.

## 📁 Project Structure

.
├── Comparative Study of GNN for UNSW-NB15.ipynb  # Main notebook
├── README.md                                     # Project documentation

## 📊 Visualizations

Correlation heatmaps before and after preprocessing

Feature distributions

Precision-Recall curves

Confusion matrices

Attention visualizations for GAT models

## 🤝 Contributing

Contributions and improvements are welcome via pull requests.

📜 License

This project is licensed under the MIT License.
