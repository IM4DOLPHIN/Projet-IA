# Projet-IA

# Détection de Tumeurs Cérébrales dans des Images IRM

## 📖 Description du projet
Ce dépôt contient un **notebook Colab** et un **script Python** pour mettre en place, pas à pas, un pipeline complet de détection de tumeurs cérébrales sur des images IRM. L’objectif est :

1. **Comprendre les données**  
   - Chargement, visualisation, exploration statistique et vérification de l’équilibre des classes.  
2. **Modéliser**  
   - Définition, entraînement et évaluation d’un réseau de neurones convolutif (CNN) pour classer chaque IRM en « tumeur » ou « normal ».  
3. **Déployer en end-to-end**  
   - Sauvegarde et rechargement du modèle, création d’une fonction `predict_and_show` pour prédire et afficher le résultat sur de nouvelles images.  
4. **Storyline / cas d’usage**  
   - Présentation de la démarche, démonstration sur des exemples, bilan et pistes d’amélioration.

## 🛠️ Prérequis
- Des notions de base en **Python** et en **notebooks Jupyter/Colab**  
- **Compte Kaggle** et **clé API (`kaggle.json`)**  
  1. Sur Kaggle → Profil → **Account** → **Create New API Token**  
  2. Téléchargez le fichier `kaggle.json`  
- Connaissances élémentaires en **CNN**, **train/test split** et **binary cross-entropy**  
- Un compte **Google** pour exécuter le notebook sur **Google Colab**

## 🚀 Comment démarrer

1. **Ouvrir le notebook**
   Cliquez sur « Open in Colab » ou importez `projet_IRM.ipynb` dans votre Google Drive.

2. **Télécharger votre clé Kaggle (kaggle.json)**
   Rendez-vous sur [https://www.kaggle.com](https://www.kaggle.com), connectez-vous à votre compte, puis allez dans :
   **"My Account" → "Create New API Token"**
   Cela télécharge un fichier `kaggle.json`. Gardez-le précieusement.

3. **Importer votre `kaggle.json` dans Colab**
   Dans l'onglet latéral « Files » de Colab, glissez-déposez le fichier `kaggle.json` directement dans `/content` (sans sous-dossier).

4. **Configurer et télécharger le dataset**
   Exécutez les cellules qui :

   * installent la CLI Kaggle
   * copient `kaggle.json` dans le répertoire `~/.kaggle`
   * téléchargent et décompressent automatiquement le dataset depuis Kaggle.

5. **Exécuter les cellules du notebook dans l’ordre** :

   * 📊 **Analyse descriptive** : chargement, exploration visuelle, distribution des classes
   * 🤖 **Modélisation** : préparation train/test, définition du CNN, entraînement, courbes d'apprentissage
   * 💾 **Pipeline end-to-end** : sauvegarde, rechargement du modèle, prédictions sur de nouvelles images
   * 🎬 **Storyline / Démo** : test de `predict_and_show`, conclusion, démonstration visuelle

## 🎯 Résultat attendu
- Précision finale sur l’ensemble de test d’environ **75–80 %**.  
- Pipeline automatisé que vous pouvez relancer en une fois pour reproduire les mêmes étapes.  
- Fonction `predict_and_show(path)` permettant de charger n’importe quelle IRM et d’afficher « Tumeur » ou « Normal » avec le score de confiance.  

## 📂 Structure du dépôt
- `brain_tumor_detection.ipynb` : Notebook Colab complet  
- `brain_tumor_project.py` : Script Python autonome (chargement, entraînement, prédiction)  

> **Note** : tout s’exécute dans Colab, sans installation locale. Assurez-vous simplement d’avoir généré et importé votre `kaggle.json` avant de lancer le téléchargement du dataset.

---

> En respectant ce guide, vous aurez une introduction opérationnelle à la création, l’entraînement et le déploiement d’un modèle de deep learning simple, appliqué à la détection de tumeurs cérébrales.  
> Bonne exploration ! 🚀  
