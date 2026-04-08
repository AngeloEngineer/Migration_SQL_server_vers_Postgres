# Préface
L'objectif de cette mission est de faire migrer des données d'entreprise de sql_server vers Postgresql tout en évitant la perte d'information

Pour ce faire nous utiliserons:
- SQL
- Python
- Jupyter Notebook


# Pseudocode


## Haut niveau

1- Auditer la donnée en dans SQL server  
2- Extraire la donnée depuis SQL server  
3- Transformer la donnée  
4-Charger la donnée dans PostgreSQL  
5-Valider la donnée (Après Migration)  
6- Generer un rapport de validation

## Bas niveau

- Creer un fichier .env  
- Charger les variables de env  
- Connection à SQL server (pyodbc)  
- Connection à Postgres (psycopg2)  
- Auditer la donnée  
- Pour chaque table:  
   - Compter le nombre de lignes  
   - Extraire toutes les lignes  
   - Transformer les nom de colonnes en miniscules  
   - Convertir les types de données   
   - Créer des tables dans Postgres  
- Lancer les vérifications post-migration  
- Generer des rapports de validation

