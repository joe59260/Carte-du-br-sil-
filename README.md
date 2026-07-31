# Carte-du-bresil-
Étude exploratoire de 27 États brésiliens sur 14 variables (urbanisation, mortalité infantile, âge, fécondité, espérance de vie, résultats électoraux…) dans le cadre d'un travail universitaire
statistiques descriptives, matrice de corrélations et cartes thématiques.

1. analyse_bresil.py produit :
> un tableau de statistiques descriptives (min, quartiles, médiane, moyenne, max) 
> un indicateur d'asymétrie `D = moyenne − médiane` par variable 
> des boîtes à moustaches 
> la matrice de corrélations (nuages de points croisés + heatmap Pearson) et la listedes corrélations les plus fortes.

2. Cartographie
Les cartes thématiques finales (variable par État, cercles proportionnels) ont été réalisées avec Magrit puis retouchées sous Inkscape, avec une réflexion sur la discrétisation (comparaison Jenks / progression géométrique / quantiles) et la sémiologie graphique.
Voir le rapport joint `exercice_bresil.pdf`.
Technologies
Python (pandas, numpy, matplotlib) · Magrit · Inkscape
Lancer le script
```
pip install pandas numpy matplotlib
python analyse_bresil.py
```
Les figures sont enregistrées dans le dossier `figures/`.
Données
`donnees_bresil.csv` — 27 États × 14 variables.

---
Réalisé dans le cadre du CSGA (ENSG). — Joe-Ann Ball.
