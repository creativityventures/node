# 02 — RPC HyperEVM et semantique des lectures

Le drapeau `--serve-eth-rpc` expose un endpoint EVM local, utile pour reduire la confiance dans un fournisseur distant.
La compatibilite JSON-RPC ne signifie pas que toutes les methodes ou hauteurs historiques sont prises en charge.
Le client doit connaitre la semantique de chaque methode, notamment `latest` contre une hauteur explicite.
Une reponse bien formee ne garantit pas que le backend a honore un parametre non supporte.
Pour les decisions critiques, verifier chain ID, hauteur retournee et fraicheur avant utilisation.
Les applications doivent refuser une substitution silencieuse de l etat courant a un etat historique demande.
Source : section EVM de [`README.md`](https://github.com/hyperliquid-dex/node/blob/main/README.md).

[Suite : Info local](03-info-local-et-fraicheur.md)
