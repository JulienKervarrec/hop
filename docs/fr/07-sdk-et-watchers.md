# 7. SDK, watchers et exploitation

Le SDK fournit la couche d’intégration côté application. Hop-node fournit la couche d’exploitation : configuration des chaînes, contrats, comptes, files d’événements, métriques et reprises après incident.

Les watchers sont spécialisés : RelayWatcher, SyncWatcher, IncompleteSettlementsWatcher, HealthCheckWatcher et ChallengeWatcher couvrent respectivement l’envoi, la synchronisation, les opérations incomplètes, la santé et les contestations. Cette spécialisation rend les responsabilités observables, mais multiplie les états à corréler.

Un opérateur doit conserver les journaux et les métriques de chaque transfert, limiter les privilèges des clés, surveiller la liquidité et traiter les reverts comme des états à diagnostiquer. Les commandes d’installation et de test mentionnées par le dépôt restent hors du périmètre de ce parcours documentaire.

Suite : [limites et périmètre](08-limites-et-perimetre.md).
