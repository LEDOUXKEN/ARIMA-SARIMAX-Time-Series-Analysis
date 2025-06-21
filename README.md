Projet: Modélisation ARIMA & SARIMAX pour les Séries Temporelles
Auteur
Fidèle Ledoux

Description
Ce projet porte sur l'analyse et la modélisation de séries temporelles à l'aide des modèles ARIMA et SARIMAX, appliqués à divers jeux de données (emploi, énergie nucléaire, etc.). Les exercices couvrent les étapes clés du traitement des données, de la stationnarisation, de l'identification des paramètres des modèles, et de l'évaluation des performances via des métriques comme le MSE. Les tests de diagnostic (Ljung-Box, Shapiro) valident les hypothèses des modèles. Les prévisions futures sont également générées pour chaque jeu de données.

Points clés
Pré-traitement : Gestion des valeurs manquantes, vérification de la stationnarité (test Dickey-Fuller), différenciation.

Modélisation : Utilisation d'ARIMA et SARIMAX, sélection des paramètres (p, d, q) via ACF/PACF.

Validation : Tests sur les résidus, métriques de performance (MSE, MAE).

Prévisions : Génération de prédictions futures et visualisation des résultats.

Exercices traités
Modélisation ARIMA pour les Données d'Emploi

Analyse d'une série temporelle de données financières sur l'emploi.

Application d'un modèle ARIMA, évaluation des performances et prévisions.

Modélisation ARIMA pour les Données Énergétiques

Analyse d'une série temporelle de production d'énergie nucléaire.

Application d'un modèle ARIMA pour la prévision.

## Technologies utilisées

- Python 3.9  
- pandas  
- numpy  
- matplotlib  
- seaborn  
- statsmodels  
- pmdarima (si applicable)

---
##  Étapes du projet

1. **Exploration des données**  
   - Visualisation de la série temporelle  
   - Détection de tendances ou saisonnalités

2. **Analyse de la stationnarité**  
   - Tests ADF (Augmented Dickey-Fuller)  
   - Transformation si nécessaire (différenciation)

3. **Identification des paramètres (p,d,q)**  
   - Analyse des autocorrélations (ACF)  
   - Analyse des autocorrélations partielles (PACF)  

4. **Modélisation avec ARIMA / ARMA / SARIMAX**  
   - Ajustement des modèles  
   - Évaluation avec AIC / BIC  
   - Comparaison des performances

5. **Analyse des résidus**  
   - Validation que les résidus se comportent comme un bruit blanc  
   - Diagnostic visuel et statistique

6. **Prévision**  
   - Génération des prédictions futures  
   - Visualisation et interprétation

---
##  Résultats

- Modèle final sélectionné basé sur des critères AIC/BIC optimisés  
- Résidus correctement distribués, validant les hypothèses  
- Prédictions cohérentes avec l’évolution observée de la série  

---
##  Exercice 1 : Modélisation ARIMA pour les Données d'Emploi

*Résumé :*  
Analyse d’une série temporelle représentant le nombre d’emplois sur une période donnée. Après vérification de la stationnarité, un modèle ARIMA est appliqué et validé à l’aide des critères AIC/BIC.

Visualisations:
<img width="509" alt="image" src="https://github.com/user-attachments/assets/806485a0-5b89-40e7-aee6-7efcb9200d45" />
<img width="349" alt="image" src="https://github.com/user-attachments/assets/9eae5ae4-05fb-477d-b81a-ba9730cf0a22" />

## Exercice 2 : Modélisation ARIMA pour les Données Énergétiques

*Résumé :*  
Étude d’une série temporelle sur la production d’énergie nucléaire. Détection de tendance, différenciation, puis modélisation ARIMA. Prédictions effectuées sur une période future.

Visualisations:
<img width="277" alt="image" src="https://github.com/user-attachments/assets/3c1179ea-e2eb-4e8a-834e-0b9e852e8886" />
<img width="518" alt="image" src="https://github.com/user-attachments/assets/ac53c920-e0a3-4e20-b7be-2fd63dfb6c1d" />
<img width="510" alt="image" src="https://github.com/user-attachments/assets/659342bd-77d6-4de4-9b08-8381c77bca0f" />
<img width="254" alt="image" src="https://github.com/user-attachments/assets/65d95faa-188e-42c2-8c92-e3d1fc3fcb4a" />


## Exercice 3 : ARMA sur les Données de Taux de Change

*Résumé :*  
Application d’un modèle ARMA sur une série de taux de change USD/EUR. Comparaison entre ARMA(p,q) et ARIMA, validation par analyse des résidus.

Visualisations:
<img width="560" alt="image" src="https://github.com/user-attachments/assets/64b6a2e0-3e46-4051-9a5b-5b2ce4376d98" />
<img width="469" alt="image" src="https://github.com/user-attachments/assets/b768e4c2-b96b-481c-9979-254c5a9889c2" />
<img width="731" alt="image" src="https://github.com/user-attachments/assets/1f85246c-ef48-42e0-b032-9c001ab36ffc" />

## Exercice 4 : Modèle SARIMAX sur les Températures Mensuelles

*Résumé :*  
Implémentation d’un modèle SARIMAX prenant en compte la saisonnalité des températures. Ce modèle permet une meilleure performance sur les séries avec composante périodique.

Visualisations:
<img width="548" alt="image" src="https://github.com/user-attachments/assets/3c7ea3f5-5aff-437b-b09e-c04bdef5c4c2" />
<img width="344" alt="image" src="https://github.com/user-attachments/assets/833c91bf-4a78-45e7-9846-95bcdc6f2d4b" />
<img width="600" alt="image" src="https://github.com/user-attachments/assets/b816f3b0-f1dc-49b4-8929-4ac8c5971ece" />
<img width="600" alt="image" src="https://github.com/user-attachments/assets/1f5e9f7f-0a7c-4ab1-b73f-395dcceb13a4" />

---

## Exercice 5 : Prévision des Indices Financiers

*Résumé :*  
Utilisation de SARIMAX pour la prévision d’indices boursiers avec variables exogènes. Résultats prometteurs avec une stabilité des prédictions.

Visualisations:
<img width="205" alt="image" src="https://github.com/user-attachments/assets/b3805962-036e-4989-85fd-910155fffd21" />
<img width="512" alt="image" src="https://github.com/user-attachments/assets/1ebc918a-7b7d-4e59-baaf-6b3390e83391" />
<img width="346" alt="image" src="https://github.com/user-attachments/assets/aa45defe-3f4d-4c4e-b3ed-c8becf4f45c7" />
<img width="605" alt="image" src="https://github.com/user-attachments/assets/efc33914-8c8b-4fd9-acb7-4d3a11104c93" />
<img width="601" alt="image" src="https://github.com/user-attachments/assets/d9482e33-90d4-4af9-a08f-c5665f3a7125" />
<img width="332" alt="image" src="https://github.com/user-attachments/assets/bd3d754c-3420-4ef7-89a2-9dd3ef4c100f" />
<img width="431" alt="image" src="https://github.com/user-attachments/assets/e9ce4ff7-ed85-4985-bde4-e4dcbec867f7" />
<img width="524" alt="image" src="https://github.com/user-attachments/assets/5ed1e179-8de0-452a-91c8-5b499c5375e2" />
<img width="622" alt="image" src="https://github.com/user-attachments/assets/09d16bd7-d067-4d77-9ab4-ce04e51ba8e4" />
<img width="503" alt="image" src="https://github.com/user-attachments/assets/47102431-e556-465d-9b91-631a4b21939d" />
<img width="276" alt="image" src="https://github.com/user-attachments/assets/4db4e903-1d42-42f2-ab17-4f5e2cbf4917" />

---
##  Compétences développées

- Manipulation et analyse de séries temporelles  
- Modélisation avec ARIMA, ARMA, SARIMAX  
- Analyse statistique (stationnarité, ACF, PACF)  
- Visualisation avancée avec matplotlib & seaborn  
- Validation et diagnostic de modèles statistiques

---

##  Structure du projet

```
 ARIMA_SARIMAX_Project
├── Exo1.to.5.ARIMA&SARIMAX.ipynb      # Notebook principal avec toutes les étapes
├── README.md                          # Fichier de documentation du projet
└── /data                              # (optionnel) Dossier contenant les jeux de données
    └── dataset.csv
```

---

##  Pistes d’amélioration

- Intégration d’un modèle Prophet (Facebook) ou LSTM (RNN) pour comparaison  
- Création d’une application Streamlit pour rendre les prévisions interactives  
- Automatisation des tests de stationnarité et du choix de paramètres  

---

# Licence

Ce projet est open-source et libre d’usage à des fins d'apprentissage ou de démonstration. Merci de mentionner l’auteur si réutilisé.
