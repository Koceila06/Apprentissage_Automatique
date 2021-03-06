# Apprentissage Automatique

## Présentation du projet
Application des algorithmes d'apprentissage supervisé ( KNN, Percepteron, Arbre de décision ) et non supervisé ( K-Moyennes ) sur une base de données réelle "Agribalise" afin de mettre en évidence des résultats intéressants.
</br>
Les problématiques étant à définir par nous même, elles comprennent : 
<ul>
         
  <li>  un problème d'apprentissage supervisé </li>
  <li>  un problème d'apprentissage non supervisé </li>
  </ul>
  
## Traitement des données
<ul>
         <li> Numérisation des données catégorielles </li>
         <li> Normalisation des données pour le k-moyennes </li>
</ul>

## Apprentissage supervisé 

### Problématique de départ 
Etude de la pollution ou non des produits selon leurs moyen de transport 
( avion ou non avion) car cela a un impact direct sur les emissions de C02
#### Difficulté 
Deux transport par avion dans toutes la base de données, ce qui est insuffisant pour l'appliquation de la validation croisée et pour le teste de nos algorithmes d'apprentissage.

### Problématique choisie
Prédiction du goupe d'aliments d'un produit en fonction des autres attributs

### Algorithmes d’apprentissage appliqués
<ul>
         <li> KNN </li>
         <li> Perceptron </li>
         <li> Arbre de décision </li>
</ul>

### Conclusion 
les algorithmes d'apprentissage « KNN » et « Arbre de décision » ont des résultats similaires et plus 
performants que le « Perceptron »

## Apprentissage non supervisé 

### Problématique choisie

#### Hypothèse   
Aprés lecture de la documentation de la base de données, on a fait l'hypothése que la base de données est divisée en deux groupes :
<ul>
         <li> Produits polluants </li>
         <li> Produits non polluants </li> 
</ul>

### Algorithmes d’apprentissage appliqués
<ul>
         <li> K-Moyennes (k==2) </li>
</ul> 

### Vérification d'hypothèse  
Aprés avoir déroulé le K-moyennes : 

Pour une meilleure précision et une meilleure vision des différences entre les deux clusters et 
pour pouvoir en tirer une conclusion, un traitement supplémentaire sur les données est nécessaire  : 
<ul> 
         <li> Suppression des colonnes non discriminantes </li>
 </ul>
 
### Résultat obtenu 

#### Premier cluster 
<img width="247" alt="Capture3" src="https://user-images.githubusercontent.com/77555379/169168271-f9000551-cc84-497e-ad79-1f5619b9451a.PNG">

#### Deuxième cluster 
<img width="217" alt="Capture4" src="https://user-images.githubusercontent.com/77555379/169168398-dd5acb45-5ec9-46ea-8d59-f3e99415214f.PNG">

### Observations 
Les valeurs de tout les attributs du deuxième cluster sont supérieures à celles du premier

### Conclusion 
On peut se dire dans ce cas qu'on possède un cluster qui représente les 
produits "polluants" (deuxième cluster) et un autre cluster composé des produits peu 
"polluant" ( premier cluster ) <Strong> notre hypothèse de départ est donc pertinente </Strong>

A présent, on peut se servir de ces résultats pour faire de l'inférence ( supervisé ) en 
comparant chaque nouvelle entrée au centroïde de chacun des clusters et de l’affecter au plus proches

## Comment tester 

Pour tester il faut : 
<ol> 
         <li> Télécharger : 
<ul>
         <li> Le dossier "iads" </li>
         <li> Le fichier "Projet_kemiche.ipynb" </li> 
         <li> Le dossier "Donnees_Agribalyse" contenant la base de données </li>
 </ul> 
         </li>
         <li> Ouvrir un terminal </li>
         <li> Se placer sur la racine du projet </li> 
         <li> Lancer la commande " jupyter notebook & " </li>
         <li> Une nouvelle fenêtre sur un navigateur va apparaitre </li>
         <li> Ouvrir sur cette fenêtre le fichier "Projet_kemiche.ipynb" </li> 
         <li> Exécuter chaque cellule du notebook </li> 
  </ol>
  
## Auteur
Koceila Kemiche
