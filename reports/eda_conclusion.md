# Conclusions de l'analyse exploratoire (EDA)
## 1. Objectif

L'objectif de cette analyse exploratoire est de mieux comprendre le dataset SMS Spam Collection avant de commencer la construction des modèles de classification.

Nous avons étudié la répartition des classes, la longueur des messages et les mots les plus fréquents.

## 2. Répartition des classes

Le dataset contient 5 574 messages :

- Ham : 4 827 messages (environ 86,6 %).
- Spam : 747 messages (environ 13,4 %).

Les messages Ham sont largement majoritaires. Le dataset présente donc un déséquilibre entre les deux classes.

## 3. Longueur des messages

La longueur moyenne des messages est différente selon leur catégorie :

- Ham : environ 71 caractères.
- Spam : environ 139 caractères.

Les messages Spam sont donc presque deux fois plus longs en moyenne que les messages Ham.

L'histogramme montre également que la majorité des messages sont relativement courts. Quelques messages présentent des longueurs particulièrement élevées.

## 4. Analyse des mots fréquents

L'analyse des mots les plus fréquents montre certaines différences entre les deux catégories.

Dans les messages Ham, on retrouve notamment des mots comme `i`, `you`, `to` et `me`.

Dans les messages Spam, on retrouve notamment `to`, `call`, `your`, `free` et `now`.

Ces résultats permettent d'identifier des mots intéressants à étudier. Cependant, un mot isolé ne suffit pas pour déterminer si un message est indésirable.

## 5. Principales observations

À partir de cette analyse, nous avons retenu les observations suivantes :

1. Les messages Ham représentent environ 86,6 % du dataset.
2. Les messages Spam représentent environ 13,4 % du dataset.
3. La longueur moyenne des messages Spam est supérieure à celle des messages Ham.
4. Les longueurs des messages sont variables, avec une majorité de messages relativement courts.
5. Certains mots, comme `free` et `call`, apparaissent parmi les mots les plus fréquents dans les messages Spam.

## 6. Hypothèses à tester ultérieurement

À partir de nos observations, nous formulons trois hypothèses :

1. Les messages plus longs pourraient avoir davantage tendance à être des Spam.
2. La présence de certains mots, comme `free`, `call` et `win`, pourrait être associée aux messages Spam.
3. La combinaison de plusieurs mots pourrait permettre de mieux distinguer les messages Ham des messages Spam qu'un seul mot pris isolément.

Ces hypothèses devront être vérifiées lors des prochaines étapes du projet.

## 7. Conclusion générale

Cette analyse exploratoire nous a permis de mieux comprendre la structure et les caractéristiques du dataset.

Nous avons identifié un déséquilibre entre les classes, des différences de longueur entre les messages Ham et Spam ainsi que des différences dans les mots fréquemment utilisés.

Ces observations constituent une première base pour la préparation des données et la construction des futurs modèles de classification.

Aucune conclusion définitive sur la capacité de ces caractéristiques à détecter les Spam ne peut être tirée à ce stade.