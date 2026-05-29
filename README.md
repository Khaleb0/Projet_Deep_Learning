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

## Dataset
- **Flickr8k** — 8 000 images, 5 captions par image
- Images : `data/raw/Images/`
- Captions : `data/raw/captions.txt`

## Dépendances
```bash
pip install torch torchvision tqdm Pillow pandas matplotlib
```

## Avancement

| Étape | Description | Notebook | Statut |
|-------|-------------|----------|--------|
| 1 | Image Processing with CNN (ResNet50) | `notebooks/multimodal_project.ipynb` | ✅ Fait |
| 2 | Text Processing with Embeddings and RNN | `notebooks/multimodal_project.ipynb` | 🔲 À faire |
| 3 | Multi-Modal Fusion | `notebooks/multimodal_project.ipynb` | 🔲 À faire |
| 4 | Model Tuning & Optimization | `notebooks/multimodal_project.ipynb` | 🔲 À faire |
