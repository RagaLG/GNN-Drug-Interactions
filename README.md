# GNN-Drug-Interactions

Given the molecular representation of two drugs, the model will be able to predict the presence of interaction.

Running the GNN Model – ‘variational AE_adj.ipynb’

Requirements :

Python (Google Colab)
  
Torch version : 1.12.1
  
Deepchem version : 2.6.1

The data folder contains three different datasets, the model is trained independently on each dataset.
1) Data folder : The totalData file contains the SMILES string for each drug, save this file in a folder under the name ‘raw’, and run the first section to get the molecular graph information for each drug.
2) The Encoder-Decoder architecture uses Graph attention network to get the unique embeddings of the drugs.
3) The Classification Neural Net is then trained on the Train data and the model which performs well on the Validation set is selected, then tested on the test data.

‘Hyperparameter Tuning.ipynb’ file was used to find the optimal hyperparameters for the GAT layer and training.

File ‘model_GAT.pth’ – model trained on the encoder-decoder architecture.

File ‘model7.pth’ – Trained Classifier model.
