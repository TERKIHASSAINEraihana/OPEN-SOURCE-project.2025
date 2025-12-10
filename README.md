#TERKI-HASSAINE raihanna biochimie appliquée 13/12/2025 
#MIMOUNI Aouicha chaimaa 
#Kaid Chaimaa Nouha 
#LASGAA manel
#Boudia Anefel 

#import pandas
import pandas as pd

#1)creation du tableau des données d'ADN

#insertion des donées du tableau

data={
     "séquences": [ "ATGCGTACGTA", "GCTAGCTAGGCC" , "ATGCGGTAAAGT" , "TACGATCGTA" , "ATGAAAGGCTT" , "CGTAGCTAGC" , "TTAACCGGAT" ],
     "Longueur" : [11, 12, 12, 10, 11, 10, 10],
     "Pourcentage GC": [50, 66.67, 58.33, 40, 45.45, 60, 55] 
}
#creation DataFrame
df = pd.DataFrame(data)

#affichage du tableau données d'ADN

print("===== Tableau données d'ADN =====") 
print(df,"\n\n") 


















