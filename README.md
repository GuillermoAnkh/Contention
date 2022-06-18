# Contention
Projet interne


L'idée est de pouvoir dans le fichier HTML saisir des valeurs si besoin et lors du clique rechercher utiliser le fichier PHP pour retourner dans un tableau les caractéristiques suivantes : 

EAN | Laboratoire | Marque | Classe | Type | Genre | Gamme | Couleur | Pied ouvert
1234567891234 | SigVaris | 2 | Chaussette | Femme | Voilisim | Beige | Oui

Pour des chaussettes par exemple on ne remplira pas tous les champs dans la DB puisque le produit s'appuie sur une mesure cheville / mollet / hauteur.
Et donc la recherche SQL serait du type si X valeurs soumises dans le formulaire. Cheville_min < X < Cheville_max.
Et ceci pour tous les champs qui sont remplis. Si on ne choisit pas une marque en particulier et qu'on rempli que cheville alors la requête retourne toutes les chevilles qui sont compatibles avec la mesure.

Je ne sais pas si par contre il y a possibilité d'inclure un bouton pour dire "Tolérance de +/- 1cm ?
