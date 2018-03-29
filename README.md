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

## 5. Identifier les tendances
Créer une nouvelle feuille dans votre classeur. Afficher de nouveau une table avec les années (Year) en colonne, et les États (States) en ligne.

Regarder dans les données quelle colonne peut donner une indications sur la force de la victoire (en bas à gauche de Tableau cliquer sur Source de données (Data Source)). 

Utiliser une marque textuelle (ou changer celle utilisée par défaut) pour indiquer le vainqueur (State Winner), et la couleur (ici la taille) pour indiquer l'intensité de la victoire (avec la variable que vous avez identifié dans les données). 

![](https://github.com/ctith/Tableau/blob/master/Tableau-screenshot/2018-03-29%2013_59_09-Tableau_2018-03-29%2012_19_40-Tableau%20Public%20Sign%20In.png%20at%20master%20%C2%B7%20ctith_Tableau.png)

Ajuster la couleur pour qu'elles représentent les partis (clic droit sur la légende > modifier les couleurs), et utiliser les paramètres avancés pour que l'échelle soit uniforme. Sauvegarder.

**Questions :**

•	Identifier les périodes temporelles (intervalles) plutôt démocrates et plutôt républicains.

![](https://github.com/ctith/Tableau/blob/master/Tableau-screenshot/2018-03-29%2013_58_08-Editing%20Tableau_README.md%20at%20master%20%C2%B7%20ctith_Tableau.png)

## 6. Cartographier
Créer une nouvelle feuille, ajouter Latitude et Longitude en ligne et colonne.

Via le menu Montre-moi (Show me) en haut à droite, basculer sur une visualisation sous forme de carte. 

Rajouter la dimension State comme Repère (Mark) détail, et la variable RD Difference (bin) utilisée précédemment toujours en couleur. 

Via Montre-moi, constater la différence entre Carte de symbole (Symbol Map) et Carte pleine (Filled Maps). Laquelle semble plus appropriée?

[Documentation Map](http://onlinehelp.tableau.com/current/pro/desktop/en-us/help.html#maps_build.html%3FTocPath%3DDesign%2520Views%2520and%2520Analyze%2520Data%7CBuild%2520Map%2520Views%7CMapping%2520in%2520Tableau%7C_____0)

> Proportional **symbol maps** are great for showing quantitative data for individual locations. For example, you can plot earthquakes around the world and size them by magnitude.

![](https://github.com/ctith/Tableau/blob/master/Tableau-screenshot/2018-03-29%2014_18_43-Editing%20Tableau_README.md%20at%20master%20%C2%B7%20ctith_Tableau.png)

> Also known as **filled maps** in Tableau, Choropleth maps are great for showing ratio data. For example, if you want to see obesity rates for every county across the United States, you might consider creating a choropleth map to see if you can spot any spatial trends.

![](https://github.com/ctith/Tableau/blob/master/Tableau-screenshot/2018-03-29%2014_18_08-Editing%20Tableau_README.md%20at%20master%20%C2%B7%20ctith_Tableau.png)

Rajouter les années en ligne (Row). Pour ne plus voir toutes années d'un coup, déplacer le bloc année de Ligne (Row) à Pages. Il est maintenant possible de naviguer entre les années.

Rajouter des informations par État qui enrichissent la visualisation.

L'exercice peut être que comme c'est une valeur quantitative cette fois identifier les différents mappings.

