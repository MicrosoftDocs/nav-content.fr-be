---
title: "Procédure : valider les coûts ajustés dans la comptabilité"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 34eec596392e9316e807d3c073c3b8e59dbc12e9
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-post-inventory-costs-to-the-general-ledger"></a>Procédure : valider les coûts ajustés dans la comptabilité   
Lorsque vous validez des mouvements de stock, tels que des expéditions vente, des factures achat ou des ajustements de stock, les quantités et les coûts modifiés sont enregistrés respectivement dans les écritures comptables article et les écritures valeur. Pour refléter ces modifications de la valeur stock dans vos livres financiers, vous devez valider les coûts ajustés sur les comptes stock associés dans les écritures comptables.

Vous pouvez valider les coûts ajustés dans les écritures comptables de deux manières :

- automatiquement, de sorte que les coûts ajustés soient validés dans les écritures comptables chaque fois que vous validez un mouvement de stock ;
- manuellement, de sorte que les coûts ajustés soient uniquement validés dans les écritures comptables lorsque vous exécutez un traitement par lots.


## <a name="to-post-inventory-costs-automatically"></a>Pour valider des coûts ajustés automatiquement
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Paramètres stock**, puis sélectionnez le lien connexe.
2. Dans la fenêtre **Paramètres stock**, cochez la case **Compta. coûts automatique**.

Pour chaque mouvement stock que vous validez, les valeurs appropriées sont validées dans le compte stocks, le compte ajustement et le compte validation stock dans la comptabilité.

Même si vous utilisez la validation coût automatique, vous devez continuer à exécuter périodiquement le traitement par lots Ajuster coûts : Écr. article pour vous assurer que les coûts des biens sont transmis aux transactions sortantes appropriées, telles que les ventes ou les transferts. Cela est particulièrement important dans les situations où vous vendez des biens avant de facturer leur achat.

Si une erreur se produit dans la configuration de dimension lors de la validation des coûts ajustés dans la comptabilité, la validation se termine par une erreur.

## <a name="to-post-inventory-costs-manually"></a>Pour valider des coûts ajustés manuellement
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Valider coûts ajustés**, puis sélectionnez le lien connexe.
2. Validez les coûts ajustés dans la comptabilité manuellement en exécutant le traitement par lots. Lorsque vous exécutez ce dernier, des écritures comptables sont créées, basées sur des écritures valeur. Vous pouvez valider les écritures de façon à ce qu'elles soient récapitulées par groupe comptabilisation.

**Remarque** : lorsque vous exécutez ce traitement par lots, il se peut que vous rencontriez des erreurs en relation avec une configuration manquante ou une configuration d'axe analytique incompatible. Si le traitement par lots détecte des erreurs dans la configuration de dimension, il les ignore et utilise les dimensions de l'écriture valeur. Pour toute autre erreur, le traitement par lots ignore la validation des écritures valeur et les répertorie à la fin de l'état dans la section intitulée « Écritures ignorées ». Pour valider ces écritures, vous devez corriger les erreurs.

Pour afficher la liste des erreurs avant d'exécuter le traitement par lot de validation, vous pouvez générer l'état **Valider coûts ajust. - Test**. L'impression test répertorie toutes les erreurs détectées durant le test de validation. Vous pouvez ensuite corriger les erreurs et exécuter le traitement par lots de validation des coûts ajustés sans ignorer aucune entrée.

Si vous voulez simplement afficher un aperçu des valeurs qui pourraient être validées dans la comptabilité sans réellement effectuer la validation, vous pouvez exécuter le traitement par lots Valider coûts ajustés sans réellement valider les valeurs dans la comptabilité. Pour ce faire, désactivez le champ Valider sur la page de sélection. De cette manière, lorsque vous exécutez le traitement par lots, l'état est produit, indiquant les valeurs prêtes pour imputation dans la comptabilité, mais elles ne sont pas validées.

## <a name="see-also"></a>Voir aussi
[Gestion du stock](inventory-manage-inventory.md)    
[Procédure : ajustement des coûts article](inventory-how-adjust-item-costs.md)  
[Gestion des ventes](sales-manage-sales.md)  
[Gestion des achats](purchasing-manage-purchasing.md)

