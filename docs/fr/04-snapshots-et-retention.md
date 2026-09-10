# 04 — Snapshots, journaux et retention

Le noeud ecrit commandes repliquees et snapshots periodiques dans `~/hl/data`.
La documentation estime que les journaux peuvent atteindre environ 100 Go par jour avec les reglages par defaut.
Une retention sure se base sur hauteur, age, verification d archive et possibilite de restauration, pas seulement sur l espace libre.
Les snapshots doivent etre copies atomiquement avec hash, chaine, hauteur et version du binaire.
Avant suppression, verifier qu une source de rattrapage et un snapshot precedent restent disponibles.
Les exports JSON servent a l inspection ; ils ne remplacent pas necessairement le format de restauration natif.
Source : section donnees L1 de [`README.md`](https://github.com/hyperliquid-dex/node/blob/main/README.md).

[Suite : exploitation](05-checklist-operateur.md)
