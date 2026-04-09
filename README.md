# 🩺 Prédiction du Diabète avec Machine Learning
Ce projet utilise un modèle de Support Vector Machine (SVM) pour prédire si un patient est atteint de diabète en fonction de mesures médicales.

## 📋 Présentation du Projet
L'objectif est d'analyser un jeu de données médicales (provenant de l'UCI Machine Learning Repository) et d'entraîner un modèle capable de classifier les patients en deux catégories :

0 : Non diabétique
1 : Diabétique
## 🛠️ Technologies et Bibliothèques
Le projet est développé en Python avec les bibliothèques suivantes :

Pandas & Numpy : Manipulation et analyse des données.
Scikit-Learn : Prétraitement (StandardScaler) et Modélisation (SVM).
Matplotlib/Seaborn (Optionnel) : Pour la visualisation.
## 🚀 Installation
Assurez-vous d'avoir Python installé.
Installez les dépendances nécessaires via le terminal de VS Code :
pip install numpy pandas scikit-learn
Placez le fichier diabetes.csv dans le même dossier que votre script.
## ⚙️ Étapes du Code
Analyse des données : Chargement du CSV et statistiques descriptives avec .describe().
Prétraitement : Normalisation des données avec StandardScaler pour que toutes les mesures soient sur la même échelle.
Entraînement : Utilisation d'un noyau linéaire (kernel='linear') avec l'algorithme SVM.
Évaluation : Calcul du score de précision (Accuracy) sur les données d'entraînement et de test.
## 📈 Résultats du Modèle
Le modèle compare les prédictions aux résultats réels pour donner un score de précision.

Précision Entraînement : training_data_accuracy
Précision Test : test_data_accuracy
## 🧪 Test avec de nouvelles données
Le script inclut un système de test manuel. Il suffit de modifier le tuple input_data pour tester un nouveau profil patient :

input_data = (5, 166, 72, 19, 175, 25.8, 0.587, 51)
# Résultat -> 'The person is diabetic'
