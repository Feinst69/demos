# DEMOS

## Auteurs
Alexander  
Arthur  
Mahmoud  
Tanjona  

## Contexte

La démocratie, considérée comme un pilier fondamental des sociétés modernes, trouve ses origines dans la Grèce antique. Clisthène, réformateur athénien du VIe siècle avant J.-C., a jeté les bases de la démocratie, introduisant des concepts tels que l'égalité et la participation des citoyens. Dans les démocraties contemporaines, le vote est l'un des principaux moyens par lesquels les citoyens exercent leur pouvoir.

Cependant, une part significative de la population choisit de ne pas voter lors des élections, un phénomène connu sous le nom d'abstention. Cette question est devenue un sujet d'étude majeur en sciences politiques et sociales. Comprendre pourquoi certaines personnes ne participent pas au processus électoral est essentiel pour renforcer la démocratie.

## Origines des données

Les données utilisées dans ce projet proviennent de l’enquête sur la participation électorale (2017). Elles comprennent:  

**Code** : Code des départements français, incluant la Corse-du-Sud (2A) et la Haute-Corse (2B).  
**HLM** : Part des locataires HLM dans les résidences principales en France en 2014.  
**Salairemoy** : Salaire net horaire moyen en France pour l'année 2015.  
**Ouvrier** : Part des ouvriers dans le nombre d’emplois sur le lieu de travail en France.  
**Employé** : Part des employés dans le nombre d’emplois sur le lieu de travail en France.  
**PI** : Part des professions intermédiaires dans le nombre d’emplois sur le lieu de travail en France.  
**Cadre** : Part des cadres et professions intellectuelles supérieures dans le nombre d’emplois sur le lieu de travail en France.  
**Artisan** : Part des artisans, commerçants et chefs d’entreprise dans le nombre d’emplois sur le lieu de travail en France.  
**Agri** : Part des agriculteurs exploitants dans le nombre d’emplois sur le lieu de travail en France.  
**TxPauv** : Taux de pauvreté en France en 2014, défini par le seuil de 60% du revenu médian.  
**NonDiplome** : Part des personnes non diplômées ou faiblement diplômées dans la population non scolarisée de 15 ans ou plus.  
**Txcho** : Taux de chômage en France au deuxième trimestre de 2017.  
**TxAbs** : Taux d’abstention aux élections présidentielles de 2017 en France.  


## Outils utilisés
Pour mener à bien cette analyse, R a été exclusivement utilisé avec ses différentes librairies :  

**readxl** : pour l'importation des données.  
**tidyverse** : pour manipuler et visualiser les données. Il inclut des composantes essentielles comme `dplyr` pour la manipulation des données, `ggplot2` pour la visualisation, et `tidyr` pour le nettoyage des jeux de données.  
**ggcorrplot** : utilisé pour visualiser les matrices de corrélation de manière intuitive.  
**reshape2** : utile pour manipuler les données en les mettant en forme longue ou large, facilitant ainsi l'analyse et la visualisation.  

## ANALYSE
### Exploration des données
L'exploration des données a été réalisée pour comprendre la structure, la distribution et les caractéristiques des variables dans l'ensemble de données.

- **Chargement des Données :**  
  Les données ont été importées à partir d'un fichier CSV.
- **Inspection des données**  
- **VIsialisation Initiale**  

### Analyse des variables
L'analyse des variables a permis d'identifier les relations significatives et d'évaluer l'importance de chaque variable par rapport au taux d'abstention.  
-**Gestions des variables compositionnels**  
-**Coorélations**  

### Reduction des données
La réduction des dimensions a été effectuée pour simplifier les données tout en conservant l'information pertinente.  
-**Analyse en Composantes Principles (ACP)**  
-**Sélection des Composantes Principales**  

### Modélisation des régressions par rapport au taux d'abstention  
Deux modèles de régression ont été appliqués pour prédire le taux d'abstention.  
-**Régression en Lasso**  
-**Modèle Random Forest**  

### Création de cluster  
La création de clusters a été réalisée pour identifier des groupes similaires au sein des données.  
-**Méthode du Coude**  
-**Clustering K-means**  
-**Visualisation du Cluster**  
