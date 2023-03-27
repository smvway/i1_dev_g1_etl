# TP - Maintenance informatique automatisée - Correction

## Partie 1

- 1\) Fonction de concaténation
  - `=CONCAT("ÉLÉMENT";B2)`
  - Mettre le format cellule en standard
- 2\) Fonction `RECHERCHEV`
  - `=RECHERCHEV(B7;'date délivrance'!$B$2:$C$29;2;FAUX)`
  - Prendre en entrée la matrice avec l'ID modifié (et pas l'ID original)
  - Format de celulle en mode date courte
- 3\) Fonction `SI.NON.DISP`
  - `=SI.NON.DISP(E3;"")`
  - Format de celulle en mode date courte

## Partie 2

- 1\) Fonction de différence entre deux dates
  - `=FRACTION.ANNEE(AUJOURDHUI();F3)`
  - Réduire à un chiffre après la virgule (format personnalisé → ``0,0``)
- 2\) Fonction de gestion d'erreur dans les formules
  - `=SIERREUR(G3;"")`
- 3\) Fonction de condition + test logique
  - `=SI(H3>=1;"Oui";"Non")`
  - Modifier les dates dans l'onglet "Tableau" pour rajouter + de "Non"

## Partie 3

- 1\) Fonction ``UNIQUE``
  - Disponible uniquement dans Office365
  - Faire à la main
  - `=UNIQUE(matrice;FAUX;FAUX)`
- 2\) Fonction `SI.MULTIPLE`
  - `=SI.MULTIPLE(C3;"imprimante laser";"Maintenance externe";"scanner";"Maintenance externe";"photocopieuse";"Maintenance externe";"écran supplémentaire";"Maintenance externe";"ordinateur portable";"Maintenance externe";"maintenance interne")`
- 3\) "Compliqué" : Combiner les fonctions ``SI`` & ``ET``
  - `=SI(ET(I3="Oui";J3="Maintenance externe");"Oui";"Non")`
  - Rajouter une mise en forme conditionnelle