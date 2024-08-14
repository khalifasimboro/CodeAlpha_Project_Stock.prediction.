# Prédiction des Prix d'Actions avec un Modèle LSTM

## Description du Projet

Ce projet a pour objectif de prédire les prix futurs d'actions de la compagnie American Airline en utilisant un réseau de neurones récurrents, plus précisément un modèle LSTM (Long Short-Term Memory). Ce type de modèle est particulièrement adapté à la modélisation des séries temporelles, telles que les prix d'actions, car il peut capturer les dépendances à long terme dans les données.

## Structure du Projet

- **Data Preprocessing :**
  - Chargement des données historiques des prix d'actions.
  - Nettoyage des données (gestion des valeurs manquantes, etc.).
  - Normalisation des données pour améliorer la performance du modèle.

- **Construction du Modèle :**
  - Création d'un modèle LSTM en utilisant TensorFlow/Keras.
  - Ajout de couches LSTM, suivies de couches denses pour la prédiction.
  - Compilation du modèle avec l'optimiseur Adam et la fonction de perte `mean_squared_error`.

- **Entraînement du Modèle :**
  - Séparation des données en ensembles d'entraînement et de test.
  - Entraînement du modèle sur les données historiques avec validation croisée pour éviter le surapprentissage.
  - Sauvegarde du modèle entraîné pour une utilisation ultérieure.

- **Évaluation du Modèle :**
  - Évaluation des performances du modèle sur l'ensemble de test.
  - Calcul des métriques d'erreur (RMSE, MAPE, etc.) pour évaluer la précision des prédictions.

- **Prédiction et Visualisation :**
  - Utilisation du modèle entraîné pour prédire les prix futurs.
  - Comparaison des prédictions avec les valeurs réelles et tracé des graphiques pour une analyse visuelle.

## Prérequis

Avant de commencer, assurez-vous d'avoir installé les dépendances suivantes :

- Python 3.6 ou supérieur
- Pandas
- NumPy
- Scikit-learn
- TensorFlow/Keras
- Matplotlib

Vous pouvez installer toutes les dépendances nécessaires en exécutant :

```bash
pip install -r requirements.txt
```

## Utilisation

Pour exécuter le projet, suivez les étapes suivantes :

1. **Prétraitement des Données :**
   - Utilisez `data_preprocessing.py` pour charger et préparer vos données.

2. **Entraînement du Modèle :**
   - Exécutez `train_model.py` pour entraîner le modèle sur vos données préparées.

3. **Prédiction :**
   - Utilisez `predict.py` pour faire des prédictions avec le modèle entraîné.

4. **Visualisation :**
   - Exécutez `plot_results.py` pour visualiser les prédictions par rapport aux valeurs réelles.

## Exemple de Résultats

Voici un exemple de comparaison entre les prix d'actions réels et les prédictions effectuées par le modèle LSTM :

![Graphique des Prédictions vs Valeurs Réelles](./images/predicted_vs_actual.png)

## Conclusion

Ce projet démontre l'efficacité des modèles LSTM pour la prédiction des prix d'actions à partir de séries temporelles. Bien que les modèles LSTM puissent offrir de bonnes performances, il est important de noter que la prédiction des marchés financiers reste une tâche complexe et sujette à de nombreuses variables externes imprévisibles.

## Contribution

Les contributions sont les bienvenues ! Si vous avez des suggestions d'amélioration, n'hésitez pas à ouvrir une issue ou une pull request.

## Licence

Ce projet est sous licence MIT - voir le fichier [LICENSE](LICENSE) pour plus de détails.
