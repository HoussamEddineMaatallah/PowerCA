# PowerCast: Prévision de la demande énergétique

Projet de prévision de la consommation électrique française avec un modèle Transformer et JAX/Flax. Ce projet inclut un pipeline de données, un modèle de deep learning depuis zéro, de l'interprétabilité avec SHAP, et une interface Streamlit.

## Structure
- `data/` : Données (ignorées par git).
- `notebooks/` : Notebooks d'exploration (EDA).
- `src/` : Modules source (modèles, entraînement).
- `app/` : Application Web Streamlit.

## Installation de l'environnement

Création d'un environnement virtuel :
```bash
python -m venv venv
# Sous Windows
venv\Scripts\activate
# Sous Linux/Mac
source venv/bin/activate
```

Installation des dépendances :
```bash
pip install -r requirements.txt
```

## Téléchargement des Données
Le projet utilise les données éco2mix de l'Open Data RTE.
```bash
python src/data/download_rte_data.py
```
