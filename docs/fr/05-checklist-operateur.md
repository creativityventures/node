# 05 — Checklist operateur Hyperliquid

1. Separer validateur, sentry, RPC public et indexation selon leurs budgets.
2. Surveiller consensus, peers, hauteur locale, retard temporel, disque et redemarrages du visor.
3. Ne servir RPC HyperEVM ou Info qu apres un seuil de synchronisation explicite.
4. Tester fraicheur et semantique des methodes, pas seulement le statut HTTP.
5. Versionner snapshots et configurations, puis exercer la restauration.
6. Proteger cle de validation et secrets d alerte hors des journaux et sauvegardes ordinaires.
Ce parcours est documentaire, pas un guide de production garanti. Aucune installation, execution de noeud ou de tests n a ete effectuee.
Sources : [`README.md`](https://github.com/hyperliquid-dex/node/blob/main/README.md) et [`README_misc.md`](https://github.com/hyperliquid-dex/node/blob/main/README_misc.md).

[Retour au sommaire](README.md)
