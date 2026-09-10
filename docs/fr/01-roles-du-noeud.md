# 01 — Roles du noeud Hyperliquid

Le depot fournit l enveloppe de deploiement et la documentation pour executeur validateur ou non-validateur.
Un validateur doit prioriser consensus et gossip ; les services publics couteux gagnent a etre separes sur des sentries.
Le noeud non-validateur peut exposer RPC HyperEVM, API Info et flux de donnees locaux.
Ces roles n ont ni le meme risque ni le meme budget de ressources.
Une architecture professionnelle separe cle de validation, trafic public, indexation et stockage historique.
Le runbook doit indiquer quel processus fait autorite pour chaque donnee servie.
Source : [`README.md`](https://github.com/hyperliquid-dex/node/blob/main/README.md).

[Suite : RPC HyperEVM](02-rpc-hyperevm.md)
