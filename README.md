# Etude du prix de l'immobilier à Paris
### Projet de Python pour le Datascientist - 2A ENSAE
### Wakil LASSEL - Lilian MAREY
### Encadrante : Elvire ROBLIN

## Présentation

Dans ce projet, nous proposons une étude des différents facteurs influençant le prix de vente des appartements Parisiens en 2019. 
Notre travail se base sur la base de données DVF 2019 (Demande de valeurs foncières) fournies part data.gouv.fr.    


Dans un premier temps, l'enjeu est d'enrichir la base de données DVF grâce à d'autres bases, en associant à chaque appartement plusieurs nouvelles variables : 
- date de construction du bâtis. 
- Coordonnées géographiques (latitude et longitude). 
- Quartier administratif. 
- Différents scores de proximité :  
    - Score de proximité aux jardins et aux espace verts. 
    - Score de proximité aux monuments. 
    - Score de proximité aux stations de métro. 
    - Score de proximité aux commerces et aux commerces spécialisés (épiceries bio, chocolateries, torrefacteurs, etc.). 
    
  
Dans un deuxième temps, il s'agit de modéliser le prix au m<sup>2</sup> à partir de toutes ces variables, et d'analyser quelles variables influencent le plus le prix.  
Des variables natives de la base DVF sont naturellement aussi considérées (arrondissement, nombre de pièces, numéro).  
Les modèles utilisés sont :  
- Regression linéaire multiple. 
- Regressions polynomiales multiples. 
- Regression pénalisée (ElasticNet)
- Regression avec Random Forest
- Réseaux de neurones.   
  
  
+ ACP et clustering.   


## Structure du projet

PrixImmobilier  
    |      
    |  
    |---- enrichissement_BDD.ipynb      : Enrichissement de la base de données DVF en ajoutant des variables  
    |  
    |---- ML.ipynb                      : Modélisation de la base enrichie et analyse des résultats  
    |  
    |---- data                          : Bases de données utilisées au cours du projet  
    |  
    |____ README.md     
    
    
## Sources

DVF : https://www.data.gouv.fr/fr/datasets/r/3004168d-bec4-44d9-a781-ef16f41856a2 (info : https://www.data.gouv.fr/fr/datasets/demandes-de-valeurs-foncieres/)    
  
Date de construction du bâtis : https://opendata.apur.org/datasets/emprise-batie-paris/data?selectedAttribute=n_sq_pc  
  
Parcelle cadastrale : https://opendata.apur.org/datasets/c38cf1e31205484ca9014e35132789cc_0  
  
Coordonnées GPS : https://adresse.data.gouv.fr/data/ban/adresses/latest/csv/adresses-75.csv.gz  
  
Quartier administratif : https://opendata.apur.org/datasets/quartier-de-paris  
  
Espaces verts : https://opendata.paris.fr/explore/dataset/espaces_verts/information/  
  
Monuments : http://pro.visitparisregion.com/chiffres-tourisme-paris-ile-de-france/frequentation-touristique-paris/Bilans/Bilan-de-l-annee-touristique-2019-a-Paris-Ile-de-France (construite à la main)  









