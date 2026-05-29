# Deep Learning Project — Multi-Modal Classification (Images + Text)

## Structure du projet

```
Projet_DL/
│
├── data/
│   ├── raw/                  # Données brutes téléchargées (MS COCO, Flickr, etc.)
│   └── processed/            # Données prétraitées (images redimensionnées, tokens, etc.)
│
├── notebooks/                # Notebooks Jupyter d'exploration et de prototypage
│
├── src/
│   ├── cnn/                  # Modèle CNN (ResNet / VGG / EfficientNet + fine-tuning)
│   ├── rnn/                  # Modèle RNN/LSTM/GRU + embeddings (Word2Vec, GloVe, BERT)
│   ├── fusion/               # Module de fusion multi-modale (concaténation + FC layers)
│   └── utils/                # Fonctions utilitaires (chargement données, métriques, etc.)
│
├── models/
│   ├── checkpoints/          # Sauvegardes intermédiaires pendant l'entraînement
│   └── pretrained/           # Poids pré-entraînés (ResNet, BERT, etc.)
│
├── results/
│   ├── figures/              # Courbes d'apprentissage, matrices de confusion, etc.
│   ├── logs/                 # Logs d'entraînement
│   └── metrics/              # Résultats chiffrés (accuracy, F1, etc.)
│
├── report/                   # Rapport théorique et mathématique
├── presentation/             # Slides de présentation finale
│
└── README.md
```

## Étapes
1. Image Processing with CNN (preprocessing → CNN model → fine-tuning)
2. Text Processing with Embeddings and RNN (tokenization → embeddings → LSTM/GRU)
3. Multi-Modal Fusion (concaténation → FC layers → softmax)
4. Model Tuning & Optimization (hyperparameter search, regularization, cross-validation)
