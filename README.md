# Jeu de Données sur les prêts de Prosper
## by Ousseynou Diop


## Dataset
Les banques recueillent beaucoup de données concernant leur utilisateur avant de leur délivrer un prêt.
Dans ce contexte on va étudier un [dataset](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv%26amp;sa%3DD%26amp;ust%3D1581581520570000&sa=D&source=editors&ust=1659905511742826&usg=AOvVaw3ThKJ5Dc5EHpAfo4vO9yGa) contenant des informations sur les prets banquaires de 113937 personnes avec 81 variables dont:
1. LoanStatus : Status actuel du prêt
2. BorrowerRate : Taux d'intérêt de l'emprunteur pour ce prêt 
3. StatedMonthlyIncome : Revenu mensuel déclaré par l'emprunteur
4. Term: La durée du prêt exprimée en mois 
5. ProsperRating(Alpha) : La note Prosper attribuée au moment de la création de la liste entre AA et HR
6. EmploymentStatus : Le statut d'emploi de l'emprunteur au moment ou il a créé la liste
7. LoanOriginalAmount : Montant initial du prêt

8. ProsperScore : Un score de risque personnalisé construit à partir des données historiques de Prosper . Le score va de 1 à 10 ,10  étant le meilleur ou le plus faible score de risque
9. BorrowerAPR : le taux annuel effectif global(TAEG) de l'emprunteur pour le prêt. 
10. ListingCategory : La catégorie de l'annonce que l'emprunteur a sélectionnée lors de la publication de son annonce 
11. EmploymentStatusDuration : La durée en mois du statut d'emploi au moment de la création de la fiche  
12. IsBorrowerHomeowner Un emprunteur sera classé comme propriétaire s'il a un pret hypothecaire dans son profil de crédit ou s'il fournit des documents confirmant qu'il est propriétaire
13. Occupation : La profession choisie par l'emprunteur au moment ou il a créé la liste
14. CurrentCreditLines : Nombre de lignes de crédit en cours au moment ou le profil de crédit a été établi

etc..... 

Pour notre étude on va se focaliser sur ses variables listé ici pour les besoin de notre analyse



## Résumé des conclusions

Au cours de l'exploration j'ai constaté que la distribution de la variable le taux annuel effectif global(TAEG) présenté beaucoup de pic et qu'il existait une relation entre le taux annuel effectif global(TAEG) et le montant du prêt avec la durée du prêt .
Le taux les plus élevé correspond en générale au montant les plus faible ce qui s'explique par la corrélation négative entre les deux variables.
La variable Prosper Rating(Alpha) qui correspond à la note Prosper attribuée au moment de la création de la liste entre AA et HR on constate que pour les personnes
avec la valeur AA ont des TAUX plus faibles .
Et le statut de l'emprunteur aussi joue sur le taux .
On constate aussi que la statue du demandeur joue sur le taux des personnes avec une statue other et not employed ont des taux (TAEG) sont plus élevés.
On peut voir que la durée du prêt est importante plus le montant du prêt initial est élevé.
Et le Prosper Rating (Alpha) la durée la plus représentée dans les classes est de 36 mois.

J'ai aussi regardé les variables qui influencent le score personnalisé que la banque donne au demandeur sont la durée du prêt et le nombre de lignes de crédit .
En dehors des variables d'intérêt j'ai vérifié que les montants les plus élevés correspondent aux durées les plus longues.

### Principaux éléments de la présentation

Pour la présentation je vais  commencer  par la distribution des variables taux  , le montant initial du prêt et la durée du prêt.
Ensuite j'introduis le Prosper Rating (Alpha) et le score personnalisé de la personne et la relation entre le temps et le montant initial du prêt. Je vais utiliser un boxplot pour visualiser cette relation car c'est plus facile de comparer le temps avec un boxplot.
Après, à l'aide d'un diagramme en point je visualise la relation entre le taux le Prosper Rating (Alpha) et la durée du prêt.
Enfin je vais présenter la corrélation négative entre le taux et le montant du prêt a l'aide d'un nuage de point je vais utiliser le paramètre alpha pour voir la ou les point sont plus centré.


