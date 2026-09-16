# 3. Le bonder et la liquidité avancée

Le bonder est un opérateur qui avance des fonds sur la chaîne de destination. Il reçoit une rémunération et immobilise du capital jusqu’à ce que le retrait canonique puisse être réclamé sur la chaîne source.

Dans hop-node, les classes L1Bridge et L2Bridge suivent les événements du bridge. Les watchers AvailableLiquidity, CommitTransfers, ConfirmRoots et BondWithdrawalWatcher organisent la chaîne opérationnelle : connaître la liquidité, regrouper les transferts, publier ou confirmer les racines, puis réclamer le remboursement.

Cette architecture crée une frontière importante : la vitesse de l’utilisateur dépend du bonder, mais la solvabilité finale dépend du bridge canonique et de la disponibilité de sa preuve. Une panne de nœud ralentit le service ; elle ne doit pas transformer une avance non remboursable en privilège permanent.

Suite : [l’AMM et le prix de sortie](04-amm-et-slippage.md).
