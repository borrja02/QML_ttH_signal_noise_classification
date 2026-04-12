# QML for Signal-Noise Classification in High Energy Physics

This repository provides a specialized research pipeline for the classification of $t\bar{t}H$ signals against Standard Model backgrounds. The project evaluates the efficacy of Quantum Machine Learning (QML) architectures in the context of high-dimensional particle physics data, specifically comparing variational quantum circuits with classical state-of-the-art benchmarks.

## Highlights and Reproducibility

The framework is designed as a modular and self-contained research tool. It includes automated data retrieval and preprocessing of HEP collision events, followed by a comparative analysis of multiple models. 

A key focus of this work is the exploration of quantum advantage through PCA-based dimensionality reduction. By utilizing custom Pauli-Feature Maps and Variational Quantum Classifiers (VQC), the pipeline identifies specific data regimes where quantum models demonstrate competitive performance over classical Deep Neural Networks. 

To ensure full reproducibility, the repository includes a comprehensive set of pre-trained weights and experimental logs. This allows for immediate verification of the results and performance metrics without the computational overhead of re-training the quantum circuits.

## Project Structure

* `QML_ttH_signal_noise_classification.ipynb`: The main research notebook containing the full pipeline, from data acquisition to final analytics.
* `saved_experiments/`: A directory containing the outputs of the experimental phase, including model weights and sensitivity analysis dataframes.
* `requirements.txt`: Environment specifications to ensure compatibility across different local setups.

## Usage Guide

### Prerequisites

The project was developed using Python 3.12.12. It is recommended to use a virtual environment to avoid dependency conflicts.

### Installation

1. Clone the repository:
   ```bash
   git clone [https://github.com/borrja02/QML_ttH_signal_noise_classification.git](https://github.com/borrja02/QML_ttH_signal_noise_classification.git)
2. Install the necessary libraries:
   ```bash
   pip install -r requirements.txt

### Running the Experiments
The main notebook is designed to be executable from start to finish. Upon the first run, the script will automatically check for the required HEP datasets in the local path; if they are not found, it will proceed to download them from the source repositories.

The results, including ROC curves and purity-significance metrics, are displayed within the notebook and can be compared against the historical data stored in the saved_experiments folder.
