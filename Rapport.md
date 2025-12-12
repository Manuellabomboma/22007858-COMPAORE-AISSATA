Rapport d'Analyse : Facteurs de Risque de Maladie Cardiaque
Fais par COMPAORE AISSATA
Ce rapport présente l'analyse de régression logistique effectuée sur le jeu de données des maladies cardiaques (UCI Heart Disease Data).

L'objectif de cette étude était de déterminer les facteurs qui influencent significativement la présence d'une maladie cardiaque (variable cible binaire : 0 = absence, 1 = présence) chez les patients, en quantifiant l'effet de ces facteurs via les Odds Ratios (OR).
1. Description des Données et Nettoyage

Le jeu de données initial a été nettoyé pour gérer les valeurs manquantes (notées ? et remplacées par NaN dans les colonnes thal et ca). Après suppression des lignes incomplètes, 297 observations ont été conservées pour la modélisation.

    Variable Cible (output) : Le jeu de données était relativement bien équilibré, avec 136 patients sans maladie cardiaque et 161 patients avec la maladie.

2. Évaluation de la Performance du Modèle

Le modèle de régression logistique a été entraîné et évalué sur un ensemble de test (30% des données) après encodage des variables catégorielles.

    Précision (Accuracy) : Le modèle a atteint une précision d'environ 85.56%, indiquant qu'il prédit correctement l'état de la maladie pour cette proportion de patients testés.

    Rappel (Recall) pour la Maladie (1) : Il a identifié correctement environ 88.46% des patients qui avaient réellement la maladie cardiaque.

    Spécificité (Specificity) pour l'Absence de Maladie (0) : Il a identifié correctement environ 83.72% des patients qui n'avaient pas la maladie cardiaque.

La performance globale du modèle est jugée solide, avec une bonne capacité à diagnostiquer les cas positifs (rappel élevé).
3. Analyse des Facteurs de Risque (Odds Ratios)

L'analyse des Odds Ratios (OR) et des P-values (seuil de signification de 0.05) a permis de séparer les facteurs en deux catégories : ceux qui augmentent et ceux qui diminuent les chances de maladie.
Facteurs Augmentant FORTEMENT les Chances (Risques)

Les facteurs suivants ont montré une corrélation positive et statistiquement significative avec la présence d'une maladie cardiaque (OR >1) :

    Type de Douleur Thoracique (cp_3 et cp_2) :

        La douleur thoracique de type cp_3 (typique d'angine) est l'un des prédicteurs les plus puissants, augmentant les chances de maladie d'environ 915% par rapport à la catégorie de référence (OR ≈10.15).

        La douleur de type cp_2 (atypique) augmente les chances d'environ 309% (OR ≈4.09).

    Angine Induite par l'Exercice (exang_1) :

        L'apparition de l'angine de poitrine lors d'un effort physique augmente les chances de maladie cardiaque d'environ 273% (OR ≈3.73).

    Défaut Réversible au Test de Stress (thal_3) :

        Ce résultat au test de thallium est un facteur de risque important, augmentant les chances d'environ 251% (OR ≈3.51).

    Sexe (Homme) (sex_1) :

        Le fait d'être un homme augmente les chances de maladie cardiaque d'environ 145% par rapport aux femmes (OR ≈2.45).

    Dépression du Segment ST (oldpeak) :

        Chaque unité d'augmentation de ce paramètre (mesuré à l'exercice) augmente les chances de maladie d'environ 57% (OR ≈1.57).

Facteurs Diminuant les Chances (Protection)

Un seul facteur a montré une corrélation négative statistiquement significative (OR <1) :

    Fréquence Cardiaque Maximale Atteinte (thalach) :

        Chaque battement supplémentaire de la fréquence cardiaque maximale atteinte diminue les chances de maladie cardiaque d'environ 3% (OR ≈0.97).

4. Conclusions et Recommandations
Conclusions Clés

    Priorité Clinique : Les symptômes et signes d'ischémie (douleur thoracique spécifique et angine à l'effort) sont les prédicteurs les plus fiables et les plus puissants de la maladie cardiaque dans ce jeu de données.

    Rôle Protecteur du Thalach : L'atteinte d'une fréquence cardiaque maximale plus élevée est associée à une probabilité plus faible de maladie, suggérant que l'amélioration de la capacité cardiovasculaire est un facteur de protection pertinent.

    Variables non Significatives : Des facteurs biométriques courants comme l'âge, la pression artérielle au repos (trestbps) et le cholestérol (chol) n'ont pas montré d'effet statistiquement indépendant et significatif dans ce modèle.Rapport d'Analyse : Facteurs de Risque de Maladie Cardiaque

Ce rapport présente l'analyse de régression logistique effectuée sur le jeu de données des maladies cardiaques (UCI Heart Disease Data).

L'objectif de cette étude était de déterminer les facteurs qui influencent significativement la présence d'une maladie cardiaque (variable cible binaire : 0 = absence, 1 = présence) chez les patients, en quantifiant l'effet de ces facteurs via les Odds Ratios (OR).
1. Description des Données et Nettoyage

Le jeu de données initial a été nettoyé pour gérer les valeurs manquantes (notées ? et remplacées par NaN dans les colonnes thal et ca). Après suppression des lignes incomplètes, 297 observations ont été conservées pour la modélisation.

    Variable Cible (output) : Le jeu de données était relativement bien équilibré, avec 136 patients sans maladie cardiaque et 161 patients avec la maladie.

2. Évaluation de la Performance du Modèle

Le modèle de régression logistique a été entraîné et évalué sur un ensemble de test (30% des données) après encodage des variables catégorielles.

    Précision (Accuracy) : Le modèle a atteint une précision d'environ 85.56%, indiquant qu'il prédit correctement l'état de la maladie pour cette proportion de patients testés.

    Rappel (Recall) pour la Maladie (1) : Il a identifié correctement environ 88.46% des patients qui avaient réellement la maladie cardiaque.

    Spécificité (Specificity) pour l'Absence de Maladie (0) : Il a identifié correctement environ 83.72% des patients qui n'avaient pas la maladie cardiaque.

La performance globale du modèle est jugée solide, avec une bonne capacité à diagnostiquer les cas positifs (rappel élevé).
3. Analyse des Facteurs de Risque (Odds Ratios)

L'analyse des Odds Ratios (OR) et des P-values (seuil de signification de 0.05) a permis de séparer les facteurs en deux catégories : ceux qui augmentent et ceux qui diminuent les chances de maladie.
Facteurs Augmentant FORTEMENT les Chances (Risques)

Les facteurs suivants ont montré une corrélation positive et statistiquement significative avec la présence d'une maladie cardiaque (OR >1) :

    Type de Douleur Thoracique (cp_3 et cp_2) :

        La douleur thoracique de type cp_3 (typique d'angine) est l'un des prédicteurs les plus puissants, augmentant les chances de maladie d'environ 915% par rapport à la catégorie de référence (OR ≈10.15).

        La douleur de type cp_2 (atypique) augmente les chances d'environ 309% (OR ≈4.09).

    Angine Induite par l'Exercice (exang_1) :

        L'apparition de l'angine de poitrine lors d'un effort physique augmente les chances de maladie cardiaque d'environ 273% (OR ≈3.73).

    Défaut Réversible au Test de Stress (thal_3) :

        Ce résultat au test de thallium est un facteur de risque important, augmentant les chances d'environ 251% (OR ≈3.51).

    Sexe (Homme) (sex_1) :

        Le fait d'être un homme augmente les chances de maladie cardiaque d'environ 145% par rapport aux femmes (OR ≈2.45).

    Dépression du Segment ST (oldpeak) :

        Chaque unité d'augmentation de ce paramètre (mesuré à l'exercice) augmente les chances de maladie d'environ 57% (OR ≈1.57).

Facteurs Diminuant les Chances (Protection)

Un seul facteur a montré une corrélation négative statistiquement significative (OR <1) :

    Fréquence Cardiaque Maximale Atteinte (thalach) :

        Chaque battement supplémentaire de la fréquence cardiaque maximale atteinte diminue les chances de maladie cardiaque d'environ 3% (OR ≈0.97).

4. Conclusions et Recommandations
Conclusions Clés

    Priorité Clinique : Les symptômes et signes d'ischémie (douleur thoracique spécifique et angine à l'effort) sont les prédicteurs les plus fiables et les plus puissants de la maladie cardiaque dans ce jeu de données.

    Rôle Protecteur du Thalach : L'atteinte d'une fréquence cardiaque maximale plus élevée est associée à une probabilité plus faible de maladie, suggérant que l'amélioration de la capacité cardiovasculaire est un facteur de protection pertinent.

    Variables non Significatives : Des facteurs biométriques courants comme l'âge, la pression artérielle au repos (trestbps) et le cholestérol (chol) n'ont pas montré d'effet statistiquement indépendant et significatif dans ce modèle.
