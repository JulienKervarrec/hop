# 4. L’AMM et le prix de sortie

Hop utilise des wrappers AMM sur certaines chaînes pour convertir entre l’actif canonique et la représentation locale. Le package hop-node distingue L2Amm et L2AmmWrapper, tandis que le SDK expose les informations nécessaires au calcul d’un transfert.

L’AMM permet à l’utilisateur de recevoir un actif immédiatement utilisable, mais le prix dépend de la réserve et de la courbe d’échange. Il faut donc séparer le montant nominal du transfert, les frais du bonder, le prix AMM et la tolérance de glissement.

Une intégration sérieuse affiche ces composantes avant signature et vérifie que la sortie minimale reste acceptable. Une estimation globale qui masque la conversion peut donner l’impression d’un bridge sans coût alors que le coût est porté par la liquidité.

Suite : [le cycle de vie d’un transfert](05-cycle-transfert.md).
