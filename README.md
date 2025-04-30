# Projet-IA

# Détection de Tumeurs Cérébrales dans des Images IRM

## 📖 Description du projet
Ce dépôt contient un **notebook Colab** et un **script Python** pour réaliser un pipeline complet de détection de tumeurs cérébrales à partir d’images IRM. L’objectif est d’illustrer, de façon simple et progressive, toutes les étapes d’un projet de machine learning :

1. **Compréhension des données** : chargement, visualisation, exploration statistique et vérification de l’équilibre des classes.  
2. **Modélisation** : définition, entraînement et évaluation d’un petit réseau de neurones convolutif (CNN) pour classer automatiquement chaque IRM en « tumeur » ou « normal ».  
3. **Solution end-to-end** : sauvegarde et chargement du modèle, fonction de prédiction sur de nouvelles images avec affichage du résultat.  
4. **Storyline / cas d’usage** : résumé de la démarche, démonstration de la prédiction, bilan et perspectives.

## 🛠️ Prérequis
Pour démarrer ce projet, il vous faut :
- Des notions de base en Python et en notebooks Jupyter/Colab.  
- Avoir un compte Kaggle et une clé API pour télécharger le dataset.  
- Connaître très sommairement les concepts de convolution (CNN), de train/test split et de fonctions de perte en classification binaire.  
- Accès à Google Colab (inutile d’installer quoi que ce soit en local si vous travaillez dans Colab).

## 🚀 Comment démarrer
1. **Ouvrir le notebook**  
   - Cliquer sur « Open in Colab » ou importer le fichier `.ipynb` dans votre Drive.  
2. **Monter Google Drive** et copier votre `kaggle.json` dans `/content`.  
3. **Télécharger le dataset** depuis Kaggle (cellule d’installation).  
4. **Exécuter les cellules** dans l’ordre :
   - Exploration des images et vérification des classes.  
   - Préparation des tableaux `X, y` et visualisation.  
   - Définition et entraînement du CNN (10 époques).  
   - Évaluation sur l’ensemble de test et affichage des courbes d’apprentissage.  
   - Sauvegarde du modèle, rechargement et prédiction sur des exemples.  

## 🎯 Résultat attendu
Si vous suivez correctement toutes les étapes :
- Vous obtiendrez un **taux de précision d’environ 75–80 %** sur l’ensemble de test.  
- Vous aurez construit un **pipeline automatisé** capable de charger une nouvelle image IRM et de prédire « Tumeur » ou « Normal » avec un affichage graphique.  
- Vous disposerez d’un **notebook entièrement documenté** (explications et visualisations) et d’un **script Python** exécutable en un seul appel pour reproduire le même workflow.

## 📂 Structure du dépôt
- `brain_tumor_detection.ipynb` : Notebook Colab pas à pas  
- `brain_tumor_project.py` : Script Python autonome (chargement, entraînement, prédiction)  
- `requirements.txt` : Liste des dépendances Python  
- `/models` : Modèles enregistrés (.keras ou .h5)  
- `/examples` : Images de démonstration et captures d’écran  

---

> En respectant ce guide, vous aurez une introduction opérationnelle à la création, l’entraînement et le déploiement d’un modèle de deep learning simple, appliqué à la détection de tumeurs cérébrales.  
> Bonne exploration ! 🚀  
