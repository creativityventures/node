# 08 — Rattrapage et réconciliation

Un indexeur ne doit pas supposer que le flux en direct a toujours été continu.
Au redémarrage, il repart du dernier bloc durablement confirmé puis rejoue la suite.
Les écritures idempotentes rendent ce recouvrement volontairement répétable.
Le rattrapage compare hauteur attendue, hauteur reçue et fraîcheur de l’API locale.
Une divergence est signalée avant de remplacer des données considérées comme correctes.
La rétention des fichiers doit couvrir la fenêtre maximale de reprise envisagée.
Les snapshots accélèrent le retour en service sans remplacer la validation de continuité.
Ce chapitre décrit le dépôt sans affirmer qu’une configuration particulière a été vérifiée.
Aucune nouvelle installation, compilation ou exécution n’a été réalisée.

Sources : [README](../../README.md), [pruner](../../pruner).
