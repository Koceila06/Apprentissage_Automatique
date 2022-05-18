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
performants que le Perceptron 

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
Pour une meilleure précision et une meilleure vision des différences entre les deux clusters et 
pour pouvoir en tirer une conclusion, un traitement supplémentaire sur les données était nécessaire  : 
<ul> 
         <li> suppression des colonnes non discriminantes </li>
 </ul>
 
### Résultat obtenu 

#### Premier cluster 

![Résultat1](https://user-images.githubusercontent.com/77555379/169166920-52c6312b-2e50-49e1-9800-957c276fd459.png)
#### Deuxième cluster 
![Résultat2](https://user-images.githubusercontent.com/77555379/169166948-58cd73c4-5478-4cac-93a2-13e48e343a48.png)
