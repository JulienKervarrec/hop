# 5. Le cycle de vie d’un transfert

Le SDK suit un transfert par identifiants et événements plutôt que par une seule transaction. Les utilitaires calculent notamment les identifiants de transfert, les racines de transfert et les données nécessaires aux étapes suivantes.

Le parcours typique est : construire la transaction, attendre sa confirmation, détecter le transfert bondé, suivre la racine publiée, puis rendre le transfert réclamable. Les watchers L1ToL2Watcher, L2ToL2Watcher et L2ToL1Watcher encapsulent ces transitions.

Cette machine d’état est utile pour les interfaces : un statut « envoyé » ne signifie pas « liquidité disponible », et « bonder avancé » ne signifie pas encore « retrait canonique remboursé ». Les erreurs doivent conserver le transfert et son identifiant pour permettre une reprise idempotente.

Suite : [preuves et retraits](06-preuves-et-retraits.md).
