Molecular Property Prediction using Graph Neural Networks (GNNs)
Project Overview

This project implements a Graph Neural Network (GNN) to predict quantum mechanical properties of small molecules using the QM9 dataset. The main goal is to demonstrate how GNNs can leverage the graph structure of molecules (atoms as nodes, bonds as edges) to learn meaningful representations and predict properties more accurately than traditional machine learning methods such as Random Forests using molecular fingerprints.

Dataset

Name: QM9 (Quantum Mechanics 9)

Source: QM9 Dataset

Composition: ~134,000 small organic molecules with up to 9 heavy atoms (C, O, N, F).

Target Properties: 13 quantum mechanical properties including:

Internal energy (U0)

Highest Occupied Molecular Orbital (HOMO)

Lowest Unoccupied Molecular Orbital (LUMO)

Dipole moment (μ)

Subset Used: For computational efficiency, a subset of 3,000 molecules was used in this project.

Project Structure
Molecular_GNN_Project/
│
├── notebooks/
│   └── Molecular_GNN.ipynb     # Main Colab notebook
│
├── src/                        # Optional if scripts separated
│   ├── model.py                # GNN model architecture
│   ├── train.py                # Training loop
│   ├── data_loader.py          # Data preprocessing and graph conversion
│   └── utils.py                # Utility functions (optional)
│
├── outputs/                    # Optional: trained models, plots
├── requirements.txt            # Python dependencies
└── README.md                   # Project documentation

Dependencies

Python packages required to run this project:

torch
torch-geometric
rdkit
numpy
pandas
scikit-learn
matplotlib


You can install all dependencies using:

pip install -r requirements.txt
