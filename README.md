NOTE:

  evrything is present in zip file.
  
Description

This project presents a Graph Neural Network (GNN)-based computational toxicology system designed to efficiently predict compound toxicity, thereby addressing the time and cost constraints of traditional laboratory testing. Leveraging a dataset of 378,709 SMILES representations with corresponding toxicity percentages (sourced from MP_data.csv and other publicly available datasets), the data was preprocessed by normalizing toxicity scores to a [0, 1] scale and removing invalid entries, resulting in 378,700 valid samples.

The hybrid GNN model, implemented using PyTorch Geometric, operates on molecular graphs where atoms are represented as nodes and bonds as edges, incorporating features such as atomic numbers and Morgan fingerprints. Additionally, RDKit is integrated for molecular visualization, enabling the display of chemical structures alongside predicted toxicity scores for improved interpretability.

The system not only predicts toxicity percentages but also classifies compounds as toxic or non-toxic based on the training data distribution. For example, the compound CCO (ethanol) yields a low toxicity score and is correctly classified as non-toxic. When benchmarked against alternative architectures such as standard GNNs and Transformer-based models, the proposed system achieves competitive performance, with an R² score of 0.57 on the test dataset.

By streamlining toxicity screening through AI-driven methods, this work has the potential to accelerate drug discovery, enhance chemical safety assessments, and scale to multi-endpoint predictions for broader applications in pharmaceutical and environmental domains.
