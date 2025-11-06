# Hybrid AI Approaches for Bitcoin Fraud Detection

This project explores and compares hybrid Artificial Intelligence (AI) techniques for detecting fraudulent transactions in the Bitcoin network. It leverages a combination of ensemble models, graph analytics, and Large Language Models (LLMs) to analyze the Elliptic dataset.

The core analysis is contained in the `enhanced_ml_gnn_llm_comparison.ipynb` notebook.

## Table of Contents
* [About the Project](#about-the-project)
* [Dataset](#dataset)
* [Technology Stack](#technology-stack)
* [Installation](#installation)
* [Usage](#usage)
* [License](#license)

---

## About the Project

This repository investigates the effectiveness of different advanced AI methodologies for identifying illicit activities in Bitcoin transactions. The primary goal is to compare the performance of:

* **Ensemble Models:** Combining multiple machine learning models to improve predictive accuracy.
* **Graph Analytics:** Utilizing Graph Neural Networks (GNNs) to model the relationships and transaction flows within the Bitcoin network.
* **Large Language Models (LLMs):** Exploring the capability of LLMs to understand transactional patterns and features for classification.

## Dataset

The project uses the **Elliptic Dataset**, a graph-based dataset of Bitcoin transactions. The dataset includes:
* `elliptic_txs_classes.csv`: Contains mappings of transaction IDs to their class (e.g., "licit", "illicit").
* `elliptic_txs_edgelist.csv`: Represents the transaction flow graph, linking different transactions.

## Technology Stack

The analysis is conducted using Python and the following key libraries:

* **Python**
* **Jupyter Notebook**
* **Pandas** & **NumPy**
* **Scikit-learn**
* **PyTorch Geometric** (or similar GNN library)
* **Transformers (Hugging Face)** (or similar LLM library)

## Installation

1.  Clone the repository:
    ```sh
    git clone [https://github.com/bharghav0210/Hybrid-AI-Approaches-for-Bitcoin-Fraud-Detection-Ensemble-Models-Graph-Analytics-and-LLMs.git](https://github.com/bharghav0210/Hybrid-AI-Approaches-for-Bitcoin-Fraud-Detection-Ensemble-Models-Graph-Analytics-and-LLMs.git)
    cd Hybrid-AI-Approaches-for-Bitcoin-Fraud-Detection-Ensemble-Models-Graph-Analytics-and-LLMs
    ```

2.  Install the required dependencies. It is recommended to use a virtual environment.
    ```sh
    # Add your installation command here.
    # If you create a requirements.txt file, you can use:
    pip install -r requirements.txt
    ```

## Usage

All analysis, models, and comparisons are detailed in the Jupyter Notebook:

1.  Launch Jupyter Notebook or Jupyter Lab:
    ```sh
    jupyter notebook
    ```
2.  Open and run the cells in `enhanced_ml_gnn_llm_comparison.ipynb` to see the complete workflow, from data preprocessing to model evaluation.

## License

This project is open-sourced under the MIT License.
