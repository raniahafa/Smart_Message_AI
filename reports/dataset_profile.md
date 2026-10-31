# Profil et audit du dataset – SMS Spam Collection

## 1. Présentation du dataset

Le projet utilise le dataset **SMS Spam Collection**, provenant de l'Université de Californie à Irvine (UCI).

Il contient des messages SMS en anglais répartis en deux catégories :

- **Ham** : messages normaux et légitimes.
- **Spam** : messages indésirables ou publicitaires.

**Source :** [UCI Machine Learning Repository – SMS Spam Collection](https://archive.ics.uci.edu/dataset/228/sms+spam+collection)

## 2. Structure du dataset

Le dataset chargé contient deux colonnes :

- `label` : catégorie du message (ham ou spam).
- `message` : contenu textuel du SMS.

**Dimensions :**
- Nombre de lignes : 5 574.
- Nombre de colonnes : 2.

Une troisième colonne, `longueur_caracteres`, a été ajoutée pour calculer le nombre de caractères de chaque message.

## 3. Répartition des classes

L'analyse de la colonne `label` donne les résultats suivants :

- **Ham** : 4 827 messages (86,59 %).
- **Spam** : 747 messages (13,41 %).
- **Total** : 5 574 messages.

**Observation :**

Les messages Ham sont largement majoritaires par rapport aux messages Spam. Le dataset présente donc un déséquilibre des classes.

## 4. Vérification de la qualité des données

### 4.1 Valeurs manquantes

La vérification avec `isna()` ne révèle aucune valeur manquante dans les colonnes `label` et `message`.

### 4.2 Doublons

La fonction `duplicated()` a permis de détecter :

- 403 lignes répétées après leur première apparition.
- 684 lignes appartenant à des groupes de doublons, en comptant toutes leurs occurrences.

**Observation :**

Les doublons ont été identifiés, mais aucune suppression automatique n'a été effectuée. Leur traitement nécessitera une décision justifiée.

## 5. Préparation des données

Une nouvelle colonne appelée `longueur_caracteres` a été créée à partir de la colonne `message`.

Elle permet de connaître le nombre de caractères de chaque SMS.

Le dataset préparé a ensuite été enregistré dans le dossier `data/processed/` sous le nom `sms_spam_collection.csv`, en conservant le fichier original dans `data/raw/`.

## 6. Conclusion

L'audit a permis de comprendre la structure du dataset et d'effectuer les premières vérifications de qualité.

Les principales observations sont :

- Le dataset chargé contient 5 572 messages.
- Les messages sont répartis en deux catégories : Ham et Spam.
- Aucune valeur manquante n'a été détectée.
- Des doublons sont présents.
- Les classes présentent un déséquilibre important.
 =>Ces vérifications constituent une première étape dans la préparation des données avant l'application des algorithmes de Machine Learning.
