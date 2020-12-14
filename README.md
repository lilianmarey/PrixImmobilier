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
