# 06 — Flux d’événements et ordre des blocs

Le nœud peut produire des flux destinés à des consommateurs externes.
Un traitement fiable conserve le numéro de bloc avec chaque lot d’événements.
L’ordre d’arrivée réseau ne remplace pas l’ordre canonique porté par la chaîne.
Un consommateur persiste un curseur seulement après avoir stocké le lot complet.
Les doublons doivent être tolérés afin de permettre une reprise idempotente.
Une rupture de séquence déclenche un rattrapage plutôt qu’une estimation silencieuse.
Le flux temps réel optimise la latence ; l’historique assure la correction.
Cette séparation évite qu’une reconnexion crée un trou invisible dans l’indexation.

Source : [documentation du nœud](../../README.md).

→ [Chapitre 07 — Provenance](07-provenance-des-actions.md)
