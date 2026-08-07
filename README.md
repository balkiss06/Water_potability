## **I/OBJECTIF:** <br>

De nos jours, face aux défis qu’on confronte fréquemment qui sont liés à la qualité de l’eau potable (les risques de contamination et les limites des méthodes traditionnelles de l’analyse), il est devenu indispensable de concevoir un système prédictif qui est capable de déterminer la qualité de l’eau et sa potabilité à partir de sa composition chimique.

---
---
            
## **II/DATASET UTILISE:**
 https://www.kaggle.com/datasets/adityakadiwal/water-potability
 
---  
---
   FEATURES:
1/ ph (pH): paramètre qui est compris entre 0 et 14 qui mesure l’acidité et la basicité de l’eau.
*Acidité : pH < 7
*Neutralité : pH = 7
*Basicité  : pH > 7
Pour que l’eau soit potable, son pH doit etre compris entre 6,5 et 8,5. 
2/ Hardness (dureté de l’eau): paramètre qui représente la concentration en ions calcium (Ca²⁺) et magnésium (Mg²⁺) dissous dans l'eau. La dureté seule ne détermine pas si l’eau est potable ou non mais elle nous informe seulement sur sa qualité.
3/ Solids (Solides dissous): paramètre qui nous renseigne sur les solides dissous (les sels minéraux, les ions, les métaux...)
4/ Chloramines: Des composés chimiques formés par le chlore et l'ammoniac. Ce sont des désinfectants utilisés pour restreindre la croissance des bactéries.
Si leur concentration est faible, l’eau n’est pas proprement désinfectée, alors que si leur concentration est très élevée, l’eau peut avoir une odeur et un gout étranges.
5/ Sulfate(SO₄²⁻): Ce sont des sels minéraux naturellement présents dans l'eau. Leur concentration élevée peut indique une contamination  de l’eau.
6/ Conductivity (Conductivité électrique): paramètre qui mesure  la capacité de l’eau à conduire le courant électrique. Une conductivité élevée n’affirme pas seule que l’eau est potable ou non.
7/ Organic_carbon (Carbone organique): paramètre qui représente la quantité de matière organique dissoute dans l’eau. Une faible concentration indique une eau propre tandis que une concentration élevée indique sa pollution.
8/ Trihalomethanes (THM): Ce sont des composés chimiques qui nous renseignent sur la qualité de l’eau par leur concentration (Une concentration faible est conforme aux normes de la qualité alors qu’une élevée présente des dangers sur notre santé).
9/ Turbidity(Turbidité): C’est une mesure de la clarté de l’eau: Une faible turbidité indique une eau claire alors qu’une forte réduit la qualité visuelle de l’eau. 

---   
 Target (CIBLE):
10/Potability (Potabilité): indique si l’eau peut etre consommée sans danger.
*Potability=1: Eau potable.
*Potability=0: Eau non potable.

---
---
## **III/EDA:**
   On essaie de comprendre le dataset, visualiser ses variables et identifier les relations entre elles avant de choisir le modèle convenable:
*Visualisation des valeurs manquantes
*Visualisation des doublons
*Visualisation des valeurs aberrantes (outliers)
*Relation entre les variables
*Analyse de la variable cible

---
---
## **IV/PRETRAITEMENT:**
 On traite les valeurs manquantes, les doublons et les valeurs aberrantes afin qu’ils n’influencent pas la performance du système.
*Remplacement des valeurs manquantes par la médiane
*Suppression des doublons

---
---
## **V/SEPARATION DES DONNEES:**
Dans cette étape, on sépare la variable cible des features. Puis, on effectue une standardisation puisque les variables n’ont pas la meme unité. On sépare ensuite les données d’entrainement de celles du test et on fait l’équilibrage nécessaire pour les données d’entrainement.

---
---
## **VI/MODELE DU MACHINE LEARNING:**
 Pour un projet de classification (Potable/Non potable), trois algorithmes peuvent etre implémentés:
1/DecisionTree: C’est le modèle le plus simple à implémenter et à interpréter, le plus rapide à entrainer mais ayant une précision plus faible par rapport aux autres modèles.
2/RandomForest: Il est plus compliqué puisqu’il rassemble plusieurs arbres de décision. Il est plus précis mais relativement plus lent. → C’est le modèle qu’on a utilisé dans ce projet.
3/XgBoost: C‘est le modèle le plus compliqué entre eux. Il est à base d’arbres de décision ou chaque nouvel arbre corrige les erreurs des précédents, plus performant, mais nécessite de réglages.

---
---
## **VII/ENTRAINEMENT DU MODELE:**
   On traine le modèle sur les données d’entrainement puis il utilise les données de test pour prédire la valeur cible.

---
---
## **VIII/EVALUATION:**
La précision du système est: 0.6646341463414634= 66,46% avec une précision de 73% pour la classe 0 et de 55% pour la classe 1.

---
---
## **IX/TEST:**
 Finalement, La partie la plus amusante consiste à essayer d’entrer un nouvel échantillon avec des nouvelles valeurs qu’on choisit et voir le résultat prédit par le système. 

---
---
## **X/Autre modèle:**
On essaie d'utiliser un autre modèle et comparer les deux performances.

---
---
## **XI/CONCLUSION:**
   Au cours de ce projet, on a développé un modèle de Machine Learning qui permet de prédire la potabilité de l’eau à partir de sa composition (son pH, sa dureté...) en suivant un démarche qui commence par l’exploration des données (EDA), le prétraitement, l’entraînement du et se termine par évaluation de sa performance. Pour savoir quel est l’algorithme optimal, on implémente des  modèles et on compare leur performance afin d'identifier le modèle offrant les meilleurs résultats.
Le Machine Learning constitue ainsi un outil efficace pour assister la surveillance de la qualité de l'eau et aider à détectter les échantillons susceptibles d'être non potables.
Ce système peut contribuer à une gestion plus efficace des ressources d’eau et à la protection de la santé publique.

## Author
**Balkis Joudi**
-LinkedIn: https://www.linkedin.com/in/balkis-joudi-332076328/
