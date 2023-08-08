# OCR6
## OpenClassRooms projet 6: Implémentez un modèle de scoring
### Données
Voici [les données](https://www.kaggle.com/c/home-credit-default-risk/data) dont vous aurez besoin pour réaliser le dashboard.

### Mission   
L’entreprise souhaite mettre en œuvre un outil de “scoring crédit” pour calculer la probabilité qu’un client rembourse son crédit, puis classifie la demande en crédit accordé ou refusé. Elle souhaite donc développer un algorithme de classification en s’appuyant sur des sources de données variées (données comportementales, données provenant d'autres institutions financières, etc.).

1. Construire un modèle de scoring qui donnera une prédiction sur la probabilité de faillite d'un client de façon automatique.
   - **Création d'une classe acceptant tous modèles XGBoost (regression, classification) avec calibration des probabilitées:**
   ![image](https://github.com/SebastianSosa/OCR6/assets/22368172/9e0fa1f8-37db-4885-8ef2-97947bba936b)

   - **Création d'une fonction pour validation croisé, optimization bayesienne des hyperparamètres, calibration des probabilitées acceptant n'importe quel fonction de perte et score:**
     ![image](https://github.com/SebastianSosa/OCR6/assets/22368172/96b22d18-fce7-4be4-ae35-b8c1a1f263a6)

  - **Approche MLOPS avec fonction acceptant la classe et la fonction crée:**
    ![image](https://github.com/SebastianSosa/OCR6/assets/22368172/3d26f700-15e6-485f-9f7e-63af9f403381)
    ![image](https://github.com/SebastianSosa/OCR6/assets/22368172/4ad6dd05-99ca-414b-b069-d87fdf22131f)

  - **Fonction de perte et score personalisé**:
    ![image](https://github.com/SebastianSosa/OCR6/assets/22368172/84215064-ac92-4c33-8cb2-4d7194fb5d81)
    ![image](https://github.com/SebastianSosa/OCR6/assets/22368172/b15439ba-a8e5-455a-b3de-f59a0cfb4697)



3. Construire un dashboard interactif à destination des gestionnaires de la relation client permettant d'interpréter les prédictions faites par le modèle, et d’améliorer la connaissance client des chargés de relation client.
![image](https://github.com/SebastianSosa/OCR6/assets/22368172/4abcd88e-2897-47fc-9cad-92b60110b2ca)

5. Mettre en production le modèle de scoring de prédiction à l’aide d’une API, ainsi que le dashboard interactif qui appelle l’API pour les prédictions.
![image](https://github.com/SebastianSosa/OCR6/assets/22368172/41054e73-e5ca-4eee-8bd0-08083e261fea)

### Compétences évaluées
1. Définir et mettre en œuvre une stratégie de suivi de la performance d’un modèle
2. Évaluer les performances des modèles d’apprentissage supervisé
3. Utiliser un logiciel de version de code pour assurer l’intégration du modèle
4. Définir la stratégie d’élaboration d’un modèle d’apprentissage supervisé
5. Réaliser un dashboard pour présenter son travail de modélisation
6. Rédiger une note méthodologique afin de communiquer sa démarche de modélisation
7. Présenter son travail de modélisation à l'oral
8. Déployer un modèle via une API dans le Web
9. Définir et mettre en œuvre un pipeline d’entraînement des modèles

### Livrables 
1. L’application de dashboard interactif répondant aux spécifications ci-dessus et l’API de prédiction du score, déployées chacunes sur le cloud.
2. Une note méthodologique décrivant la méthodologie d'entraînement du modèle, le traitement du déséquilibre des classes, la fonction coût métier, l'algorithme d'optimisation et la métrique d'évaluation, un tableau de synthèse des résultats, l’interprétabilité globale et locale du modèle, les limites et les améliorations possibles, l’analyse du Data Drift.
3. Un support de présentation
