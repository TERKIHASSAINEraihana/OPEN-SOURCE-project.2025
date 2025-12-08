#TERKI-HASSAINE raihanna biochimie appliquée 13/12/2025 
#MIMOUNI Aouicha chaimaa 
#Kaid Chaimaa Nouha 
#LASGAA manel
#Boudia Anefel 

#import pandas
import pandas as pd

#1)Création du tableau des données d'ADN

#inerstion les données du tableau

data = {
    "séquences": [ "ATGCGTACGTA", "GCTAGCTAGGCC", "ATGCGGTAAAGT","TACGATCGTA", "ATGAAAGGCTT", "CGTAGCTAGC", "TTAACCGGAT"],
    "Longueur": [11, 12, 12, 10, 11, 10, 10],
    "Pourcentage GC": [50, 66.67, 58.33, 40, 45.45, 60, 50]
}
#creation DataFrame
df = pd.DataFrame(data)
