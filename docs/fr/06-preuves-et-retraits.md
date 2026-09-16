# 6. Preuves, racines et retraits

Après la fenêtre de finalité, un retrait L2 peut être prouvé sur la chaîne canonique. Le SDK contient WithdrawalProof et les tests associés documentent la construction des données de preuve sans réduire la preuve à un simple reçu de transaction.

Le nœud surveille la publication et la confirmation des racines. BondTransferRootWatcher et ConfirmRootsWatcher relient les événements observés aux opérations de remboursement du bonder.

Le modèle de sécurité repose sur plusieurs vérifications : bon réseau, bon transfert, bonne racine, bon destinataire et absence de réclamation déjà effectuée. Une preuve valide atteste un état précis ; elle ne garantit pas à elle seule la disponibilité d’une transaction RPC ni la bonne configuration de l’opérateur.

Suite : [SDK, watchers et exploitation](07-sdk-et-watchers.md).
