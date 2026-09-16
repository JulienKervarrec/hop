# 2. Le bridge entre L1 et L2

Le SDK construit un parcours selon trois directions : L1 vers L2, L2 vers L2 et L2 vers L1. Les watchers correspondants vivent dans packages/sdk/src/watchers et adaptent les étapes à la chaîne source et à la chaîne de destination.

Un dépôt L1 ou L2 verrouille l’actif dans le bridge de la chaîne source. Pour un transfert L2 vers L2, le protocole combine le retrait vers L1 et le dépôt vers l’autre L2 dans une expérience unifiée. Les contrats et adresses déployées sont sélectionnés à partir de la configuration de chaîne.

Le SDK sépare la préparation de la transaction, l’envoi, l’observation des événements et la récupération de la preuve. Cette séparation réduit le risque de confondre transaction soumise et transfert effectivement disponible.

Suite : [le rôle du bonder](03-bonder-liquidite.md).
