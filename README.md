# Projet-Velib---Bicycle-sharing-analysis

Ce projet porte sur l'analyse des flux d'utilisation de vélos dans le cadre du système de partage public : Vélib. Les données ont été récoltées via l'API sur la page Open Data du site Vélib-métropole.fr en licence ouverte.

Language : Python

Bibliothèques : Pandas, numpy
Data visualisation : matplotlib, seaborn

##### Période étudiée : 4 mois - à partir de mai jusqu'à août 2021.

<img width="649" alt="image" src="https://user-images.githubusercontent.com/119977140/207740449-16a79a39-ba4b-42ce-8eab-f41487d31392.png">

## La problématique data : optimiser la circulation et les flux d'utilisation de vélo dans les stations Vélib parisiennes pour les trajets 'domicile-travail'.

Explication des colonnes du jeu de données : 

<img width="461" alt="image" src="https://user-images.githubusercontent.com/119977140/207625151-60d26e79-9b56-48fa-a56f-28f1b26b0b2c.png">

### Les étapes de l'analyse :
#### 1) Data preparation/cleaning (suppression des duplicates, des colonnes non utilisables,...)
#### 2) Data prep & analysis : (création de colonnes plus pertinentes à l'aide de l'extraction de l'heure et du jour de la colonne 'due_date' et de l'extraction de la latitude et longitude de la colonne 'coordonnees_geo', création des colonnes weekend et vacances scolaires (booléen indiquant si la ligne concerne un jour de weekend ou de vacances scolaires)
#### 3) Enrichissement des données : code postaux obtenus grâce au reverse geocoding et import de données de population/arrondissement


<img width="676" alt="image" src="https://user-images.githubusercontent.com/119977140/207742169-6c500bae-4cd1-482a-8e23-531c235194a2.png">


# Principales visualisations :

<img width="563" alt="image" src="https://user-images.githubusercontent.com/119977140/207741015-ec4eb8b5-8fa9-4104-95e3-5dcc785241fc.png">

Dans un premier temps, ces graphiques (fig 6 & 7) indiquent un déséquilibre entre le choix d'implantation des stations et la concentration de population dans les arrondissements parisiens

<img width="704" alt="image" src="https://user-images.githubusercontent.com/119977140/207741968-4146c39a-3783-4528-ba2e-b4f68b8f2727.png">
figure 6 : capacité de vélos/habitant et par arrondissement // figure 7 : distribution du pourcentage de population/arrondissement

# Observations : 

<img width="559" alt="image" src="https://user-images.githubusercontent.com/119977140/207742257-b747910b-634b-48c0-875e-df47b544ce68.png">

<img width="696" alt="image" src="https://user-images.githubusercontent.com/119977140/207742302-4c1293a7-986a-4fe1-9173-92daf9755b6b.png">


<img width="641" alt="image" src="https://user-images.githubusercontent.com/119977140/207744219-71ac7b7b-0e97-4167-b224-ac06060e8122.png">

Focus sur les arrondissements avec les courbes de tendance similaires ( 11, 14, 17, 18, 19 & 20ème) ==> Présence de forte utilisation des vélos pour les trajets domicile-travail (indiqué par un taux de disponibilité bas pendant les horaires de travail)

<img width="646" alt="image" src="https://user-images.githubusercontent.com/119977140/207744317-8dcd99dc-d050-4d67-bab2-473aef8aeebb.png">

Focus sur les arrondissements avec les courbes de tendance similaires : (du 1er au 9ème) ==> zones dites 'de destination', où les utilisateurs se rendent le matin aux horaires de travail. Le taux de disponibilité dans ceux-ci augmente fortement entre 7h et 9h du matin pour ensuite baisser en fin de journée travaillée quand les salariés quittent ces zones.

<img width="630" alt="image" src="https://user-images.githubusercontent.com/119977140/207746706-9a10bdc6-182b-45d2-88b7-5ce6134e7a87.png">


En croisant ces données avec des données externes sur le taux de concentration de l'emploi par arrondissement, nous constatons que l'implantation des stations Vélib doit être revue afin de répondre au besoin des arrondissements à faible taux de concentration. La population de ces arrondissement a tendance à se déplacer en vélo vers les arrondissements à taux de concentration d'emploi élevé causant des taux de disponibilités mal équilibrés et par la suite, un taux d'embouteillage élevé du fait d'utilisation d'autres moyens de transport :

<img width="706" alt="image" src="https://user-images.githubusercontent.com/119977140/207746181-45a42911-5528-456c-a056-2da86475216f.png">


Travail réalisé par :
Elsa T. ;
Marie-Claudine B. et
Aline E.

