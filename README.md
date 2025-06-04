🧬 Self-Interacting Protein (SIP) Prediction
This project focuses on in silico prediction of Self-Interacting Proteins (SIPs) using sequence-based features and machine learning models. It aims to classify whether a given protein sequence is self-interacting or not using a variety of classifiers.

📌 Objective
To build a robust classification pipeline using protein sequence encodings derived from:

BLOSUM62 substitution matrix

AAPHY7 physicochemical properties

And applying:

Feature extraction (FFT)

Dimensionality reduction (PCA)

Machine learning models (SVM, Random Forest, KNN, and custom ensemble methods)

🧰 Technologies Used
Python

Scikit-learn

NumPy / Pandas

Matplotlib

BioPython

TQDM

📁 Project Structure
Final_SIP_Proj.ipynb — Main notebook implementing the full pipeline

aa_phy7.txt — Contains AAPHY7 physicochemical feature vectors

blosum62.txt — Substitution matrix file used for encoding

protein_sequences.txt — Dataset of protein sequences (assumed)

🧪 Methods
Encoding: Protein sequences are transformed into numerical vectors using BLOSUM62 and AAPHY7 matrices.

Transformation: FFT is applied to capture frequency domain features.

Dimensionality Reduction: PCA is used to reduce feature space to various dimensions (e.g., 250D).

Classification:

SVM (Support Vector Machine)

Random Forest

KNN (with Leave-One-Out CV)

Random Projection Ensemble Classifier (custom)

🚀 How to Run
Clone the repository.

Make sure the required files (aa_phy7.txt, BLOSUM matrix) are in the appropriate directory.

Open Final_SIP_Proj.ipynb in Jupyter or Google Colab.

Install dependencies:

bash
Copy
Edit
pip install biopython scikit-learn tqdm
Run all cells.

📈 Evaluation Metrics
Accuracy

F1 Score

AUC-ROC

Average Precision

Matthews Correlation Coefficient (MCC)

📝 Future Work
Integration of 3D structural data from AlphaFold

Incorporation of Gene Ontology (GO) features

Deep Learning-based models for sequence embedding
