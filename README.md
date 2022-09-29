# Satellite_Images_Embeddings

### Embeddings:

Embeddings of 1024 features generated using the satellite images of the top 5 municipalities with most dengue cases in Colombia. 
The embeddings were generated usign dimensionality reduction methods such as:

1. Supervised Contrastive Learning:
- Code to create the model: Contrastive_learning.ipynb
- Code to generate the embeddings: Features_Contrastive_learning.ipynb


2. Variational Autoencoder
- Code to create the model: Variational_Autoencoder.ipynb
- Code to generate the embeddings: Features_Variational_Autoencoder.ipynb

3. Autoencoder
- Code to create the model: Autoencoder.ipynb
- Code to generate the embeddings: Features_Autoencoder.ipynb


The embeddigns can be found in the folder `Embeddings/` with the names:

- Features of Supervised Contrastive Learning: `embeddings_contrastive_learning_1024features.csv`

- Features of Variational Autoencoder: `embeddings_vae_1024features.csv`

- Features of Autoencoder: `embeddings_autoencoder_1024features.csv`

All labels used to train the models can be found in the folder: `Dengue_dataset/`

- Labels with dengue cases per inhabitans for regression: `cases_per_inhabitants.csv`
- Labels with peak or not peak of dengue for binary classification: `binary_classes.csv`
- Labels with increase, decrease or stable dengue cases across weeks for multi-class classification: `multiclass_labels.csv`
- Labels with dengue cases across weeks and other sociodemographic/socioeconomic variables per municipality: `dengue_data_all_municipalities.csv`


### Machine Learning models with the dataset:

1. LSTM for regression of dengue cases using the embeddigns.

2. LSTM for multiclass classification using the emebeddings.

3. Binary classification + Contrastive learning.

