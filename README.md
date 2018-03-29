# TP Tableau

## Objectifs du TP
- Découvrir Tableau Public
- Comprendre le mapping de données sur des marques graphiques (ligne, carré, ..) et leurs propriétés (taille, couleur, ..)
- Faire la distinction entre données brutes et abstraites, ainsi qu'entre dimensions et mesures
- Explorer un espace de conception de visualisation

## 1. Charger les données dans Tableau
Lancer Tableau, sélectionner connexion à un fichier texte et charger le fichier csv :
> ElectionsPresidentielleUS_data_clean.csv. 

Basculer sur la vue des données (en bas à gauche de Tableau cliquer sur Source de données (Data Source)).
![](https://github.com/ctith/Tableau/blob/master/Tableau-screenshot/2018-03-29%2011_53_55-TP%20Tableau.docx%20-%20Word.png)

**Questions :**

•	Que signifient les icônes dans l'en-tête des colonnes ?
> Le type des données

•	Quelles sont les valeurs possibles ?
> Nombre décimal, Nombre entier, Date & Heure, Date, Chaîne de caractère, Booléen, Par défaut

•	Est-ce possible de changer ces valeurs et quel est l'effet sur la colonne en cours ?
> Oui, Tableau transforme les données de la colonne dans le type voulu (ex: Nombre entier 1 -> Nombre décimal 1,0000)

## 2. Voir les résultats sous forme de table
Basculer maintenant sur la 1ère Feuille (Sheet). 

Commencer par afficher une table avec les années (Year) en colonne, et les États (States) en ligne.

Afficher à l'intérieur de la table le gagnant de l'État en question pour l'année donnée (State Winner). 
Pour ce faire, associer le State Winner à une marque graphique, ou Repères (Mark). 
Essayer avec du texte (Label) ou de la couleur. 

Ajuster le format de la marque graphique (texte, carré, ...) 

Ajuster au besoin la couleur (via le menu de la légende, à droite) pour que le rouge représente les républicains, le bleu les démocrates et le orange les indépendants.

![](https://github.com/ctith/Tableau/blob/master/Tableau-screenshot/2018-03-29%2012_01_29-.png)

**Questions :**

•	Quelles sont les données manquantes ?
> Alaska, Dist of Col., Hawaii entre 1910 et 1960

•	Quel indicateur utiliser ?
> States

Ré-organiser la table (trier par ligne selon la mesure auto-générée Nombre d'enregistrement) pour mettre en avant les données qui manquent.

![](https://github.com/ctith/Tableau/blob/master/Tableau-screenshot/2018-03-29%2012_09_17-Trier%20%5BState%5D.png)
![](https://github.com/ctith/Tableau/blob/master/Tableau-screenshot/2018-03-29%2012_09_25-Editing%20Tableau_README.md%20at%20master%20%C2%B7%20ctith_Tableau.png)

## 3. Filtrer de manière basique
Pour chercher où un Indépendant (candidat non Républicain ou Démocrate) est arrivé en tête, il est possible de cliquer sur la légende (qui est interactive). 

Cependant créez votre propre mécanisme de filtrage, similaire à la légende, en rajoutant State Winner comme filtre. 

Faire en sorte que le filtre apparaisse à l'écran, et l'utiliser pour répondre à la question suivante.

![](https://github.com/ctith/Tableau/blob/master/Tableau-screenshot/2018-03-29%2012_12_40-Filtrer%20%5BState%20Winner%5D.png)

**Questions :**

•	Dans quel État et en quelle année un indépendant un indépendant est arrivé en tête ?
![](https://github.com/ctith/Tableau/blob/master/Tableau-screenshot/2018-03-29%2012_15_40-Tableau%20Public%20-%20Classeur1.png)

## 4. Sauvegarder et partager
Renommer votre feuille de calcul en double cliquant sur le titre de la visualisation, selon le numéro de l'exercice. Par exemple TPDataViz1.3. Sauvegarder, créer un compte Tableau Public au besoin.

![](https://github.com/ctith/Tableau/blob/master/Tableau-screenshot/2018-03-29%2012_19_40-Tableau%20Public%20Sign%20In.png)
