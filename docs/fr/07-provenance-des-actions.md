# 07 — Provenance des actions système

Les sorties CoreWriter relient l’exécution HyperEVM aux actions du cœur Hyperliquid.
Une trace exploitable conserve bloc, transaction, index de log et identifiant système.
Le hash de transaction seul ne suffit pas lorsqu’une transaction émet plusieurs événements.
L’identifiant métier ne doit pas être reconstruit à partir d’un texte d’affichage.
Les événements inconnus sont archivés avant d’être décodés par une version plus récente.
La provenance permet d’expliquer quelle entrée a produit quel changement observé.
Elle facilite aussi la réconciliation entre l’état local et les réponses de l’API Info.
Le modèle de données doit donc préserver les identifiants bruts et leur contexte.

Source : [documentation du nœud](../../README.md).

→ [Chapitre 08 — Rattrapage](08-rattrapage-et-reconciliation.md)
