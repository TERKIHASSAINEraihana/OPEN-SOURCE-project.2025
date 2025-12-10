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
     "Pourcentage GC": [50, 66.67, 58.33, 40, 45.45, 60, 50] 
}
#creation DataFrame
df = pd.DataFrame(data)

#affichage du tableau données d'ADN

print("===== Tableau données d'ADN =====") 
print(df,"\n\n") 

#2) operation sur le tableau 
print("===== operation =====\n\n")

# Sélection et affichage de la colonne Longueur 

print("*** Colonne Longueur ***")
Longueur = df["Longueur"]
print(Longueur,"\n\n")

#3)Filtrer les séquences dont la Longueur > 10
print("*****séquence avec Longueur > 10 *****")
Filtred_df = df[df["Longueur"]> 10]
print(Filtred_df,"\n\n")

#4)Calcul du Pourcentage GC moyen avec 3 chiffres aprés la virgule 
print("*****calcul du Pourccentage GC moyen*****")
average_gc = df["Pourcentage GC"].mean() 
print(f"Pourcentage GC moyen : {average_gc:.3f}%""\n\n") 

#5)Ajouter une nouvelle colonne avec calcule 
#ajout d'une colonne 'Catégorie GC' 
print("***** ajout d'une colonne Catégorie GC *****") 
average_gc = df["Pourcentage GC"].apply(lambda GC: "Riche" if GC > 55 else ("Moyen" if 45 <= GC <= 55 else "Faible" )) 
print(df,"\n\n") 

#6)Ajouter une colonne donnant le nombre de 'G' dans chaque séquence 
print("*****une colonne donnant le nombre de 'G' dans chaque séquence ******") 
df["nombre de G"] = df["séquences"].str.count("G")
print(df,"\n\n")

#7)Calculer l'écart-type
#Calculer l'écart- type du pourcentage GC
print("*****calcul de l'ecart-type du pourcentage GC *****")
ecart_type_gc = df["Pourcentage GC"].std()
print(f"Pourcentage GC: {ecart_type_gc}","\n\n")



















