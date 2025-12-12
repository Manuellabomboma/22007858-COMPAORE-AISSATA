# RAPPORT GLOBAL SUR LES FACTEURS DE RISQUE CARDIAQUE
Fais par COMPAORE AISSATA
---

## 1. CADRE DE L'ÉTUDE ET PRÉPARATION DES DONNÉES

Cette analyse approfondie repose sur l'exploitation de la base de données UCI Heart Disease afin d'identifier les déterminants majeurs de la présence d'une pathologie cardiaque. L'étude a débuté par une phase rigoureuse de nettoyage des données où les valeurs manquantes, initialement marquées par des symboles d'interrogation, ont été traitées pour garantir l'intégrité des résultats statistiques.

Après la suppression des dossiers incomplets et l'élimination des variables jugées non significatives pour ce modèle particulier comme l'identifiant du patient ou le niveau de glycémie à jeun, l'échantillon final s'est stabilisé à 297 patients. La variable de sortie a été transformée en indicateur binaire pour permettre l'application d'une régression logistique, séparant distinctement les patients sains des patients présentant une maladie confirmée.

---

## 2. ÉVALUATION ET FIABILITÉ DU MODÈLE STATISTIQUE

Le modèle de régression logistique mis en place a été soumis à une phase de test rigoureuse pour mesurer sa capacité de généralisation. Les indicateurs de performance révèlent une précision globale de 85,56 %, ce qui témoigne d'une grande fiabilité dans les prédictions effectuées. 

L'analyse de la matrice de confusion montre que le système est particulièrement performant pour détecter les cas de maladie réels, avec un rappel s'élevant à 88,46 %. Cette sensibilité élevée est un atout majeur car elle minimise le risque de faux négatifs dans un diagnostic médical critique. Parallèlement, la spécificité reste robuste à 83,72 %, assurant que les patients sains sont également identifiés avec une marge d'erreur très faible.



---

## 3. ANALYSE DÉTAILLÉE DES IMPACTS PAR LES ODDS RATIOS

L'interprétation statistique via les Odds Ratios permet de quantifier précisément l'influence de chaque variable sur la probabilité de développer une maladie cardiaque. Les résultats de cette analyse permettent de classer les facteurs selon la force de leur impact.

Le facteur de risque le plus massif identifié concerne le nombre de vaisseaux colorés par fluoroscopie, particulièrement lorsque ce nombre atteint deux ou trois vaisseaux, multipliant de manière exponentielle les chances de maladie. Le sexe du patient apparaît également comme un prédicteur crucial, les hommes présentant des chances de maladie environ 480 % plus élevées que les femmes dans cet échantillon, toutes choses égales par ailleurs.

D'autres variables cliniques comme le type de douleur thoracique ont montré des résultats intéressants. Paradoxalement, dans ce modèle spécifique, l'angine de poitrine typique a été associée à une probabilité plus faible par rapport aux autres formes de douleurs complexes. En revanche, les indicateurs liés à l'effort physique comme la fréquence cardiaque maximale atteinte montrent un rôle protecteur constant. Pour chaque battement supplémentaire par minute atteint lors de l'effort, le risque global diminue de 3 %, soulignant l'importance de la capacité cardiovasculaire.



---

## 4. CONCLUSIONS GÉNÉRALES ET PRÉCONISATIONS

L'étude conclut que la maladie cardiaque est prédite par une combinaison de facteurs physiologiques immuables et de signes cliniques mesurables lors de tests d'effort. La prédominance des résultats liés à la fluoroscopie et au sexe indique que le dépistage doit être particulièrement vigilant chez les profils masculins présentant des anomalies vasculaires visibles.

Il est recommandé d'intégrer ces poids statistiques dans les outils d'aide au diagnostic pour prioriser les patients les plus à risque. Les résultats suggèrent également que le maintien d'une bonne condition physique permettant d'atteindre des fréquences cardiaques élevées sans douleur reste l'un des meilleurs indicateurs de protection. Cette analyse fournit une base solide pour orienter les examens cliniques vers les variables ayant le plus fort pouvoir prédictif identifié par le modèle.

