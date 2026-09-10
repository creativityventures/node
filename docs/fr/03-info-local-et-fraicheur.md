# 03 — Serveur Info local et fraicheur

Le drapeau `--serve-info` expose un sous-ensemble des requetes Info derivables de l etat local.
Cette surface reduit les limites de taux externes, mais ne fournit ni toutes les series historiques ni les websockets.
Le depot recommande de comparer periodiquement les timestamps via `exchangeStatus`.
Un consommateur doit ignorer ou degrader une source locale lorsque son horodatage L1 devient trop ancien.
La disponibilite HTTP et la fraicheur de l etat sont deux indicateurs distincts.
Exporter metriques de hauteur, retard temporel et dernier bloc applique rend cette frontiere observable.
Source : section Info de [`README.md`](https://github.com/hyperliquid-dex/node/blob/main/README.md).

[Suite : snapshots](04-snapshots-et-retention.md)
