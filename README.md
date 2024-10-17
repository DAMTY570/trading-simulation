# trading-simulation

# Projet de Prédiction et Simulation de Trading

## Introduction
Ce projet vise à prédire les cours des actions d'Apple (AAPL), Amazon (AMZN) et Tesla (TSLA) en utilisant des réseaux de neurones récurrents de type LSTM (Long Short-Term Memory). L'objectif principal est de simuler des stratégies de trading basées sur les prédictions fournies par ces modèles et d'analyser les gains et les pertes obtenus dans différents scénarios de trading.

## Objectifs du Projet
- Utiliser les séries temporelles des prix de clôture des actions pour entraîner des modèles LSTM.
- Simuler des stratégies de trading basées sur les prédictions des modèles.
- Évaluer les performances des stratégies à travers des métriques financières telles que le solde final et l'évolution des transactions au fil du temps.

## Données Utilisées
Les données utilisées dans ce projet sont les prix de clôture quotidiens des actions AAPL, AMZN et TSLA, extraits pour la période allant du 1er janvier 2015 au 31 décembre 2022. Les données sont normalisées pour une meilleure performance des modèles de machine learning.

## Modèles Utilisés
- **LSTM** : Le modèle LSTM est utilisé pour capturer les dépendances temporelles dans les séries de prix de clôture des actions. Le modèle a été configuré avec différentes fenêtres de prédiction et ajustements d'hyperparamètres.
  
## Pipeline de Prédiction et de Simulation
1. **Préparation des Données** : Extraction des séries temporelles, normalisation, et création de séquences pour l'entraînement des modèles.
2. **Entraînement des Modèles LSTM** : Les modèles LSTM sont entraînés sur des données d'entraînement couvrant plusieurs années de prix de clôture.
3. **Prédiction** : Prédictions des prix de clôture futurs pour chaque action.
4. **Simulation de Trading** : Simulation des stratégies d'achat et de vente basées sur les prédictions.
    - **Achat** : Si le prix prédit pour le jour suivant est supérieur au prix actuel, acheter des actions avec tout le solde disponible.
    - **Vente** : Si le prix prédit est inférieur, vendre toutes les actions détenues.
5. **Analyse des Résultats** : Calcul du solde final et analyse des gains ou pertes réalisés.

## Résultats
Les résultats montrent des performances variées pour chaque action :
- **AAPL** : La simulation indique un solde final de 1 028 324 USD, avec une stratégie qui a généré un bénéfice.
- **AMZN** : Après ajustements, le solde final est de 1 000 000 USD, évitant les pertes observées dans la première simulation.
- **TSLA** : Un bénéfice notable de 1 116 590 USD a été réalisé, suggérant que la stratégie était efficace pour cette action.

## Améliorations Futures
- **Optimisation des Modèles** : Envisager l'utilisation de modèles plus avancés comme les Transformers pour capturer des dépendances à plus long terme.
- **Stratégies de Trading Plus Sophistiquées** : Intégrer des indicateurs techniques comme les moyennes mobiles ou les bandes de Bollinger pour améliorer la prise de décision.
- **Données Supplémentaires** : Intégrer des variables supplémentaires comme les nouvelles financières ou les volumes de transactions pour affiner les prédictions.

## Conclusion
Ce projet démontre le potentiel des modèles de deep learning, en particulier les LSTM, pour prédire les cours des actions et simuler des stratégies de trading. Bien que des résultats positifs aient été obtenus, il est crucial d'affiner les modèles et les stratégies de trading pour maximiser les bénéfices dans des conditions de marché réelles.

## Auteur
- **Abraham Krah** - Projet réalisé dans le cadre du D.U Big data, data science et analyse des risques sous Python.

## Licence
Ce projet est sous licence MIT.

