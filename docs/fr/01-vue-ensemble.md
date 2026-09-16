# 1. Vue d’ensemble de Hop

Hop est un protocole de transfert d’actifs entre Ethereum et des réseaux de couche 2. Son monorepo regroupe le SDK TypeScript, le nœud de bonder, les interfaces et les outils d’exploration. Le parcours suit principalement les flux v1 décrits par les packages sdk et hop-node.

L’idée centrale est de ne pas attendre la finalité complète d’un retrait L2 : un bonder avance la liquidité sur la chaîne cible, puis se rembourse lorsque le retrait canonique est finalisé. Chaque étape possède un identifiant, des preuves et des garde-fous.

Le dépôt expose aussi une branche v2 en développement, mais sa documentation publique reste limitée. Nous distinguons donc clairement les mécanismes v1 lisibles et les éléments v2 seulement signalés par le code.

Suite : [identité des chaînes et bridge](02-bridge-l1-l2.md).
