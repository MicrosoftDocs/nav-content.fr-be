---
title: "Procédure : regrouper des réceptions"
description: "Si vous voulez facturer plusieurs réceptions achat en une fois, vous pouvez utiliser la fonction Regroupement des réceptions."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/14/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 10749dc8d8d692d94c5405fbb0a4a965d482f013
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-combine-receipts-on-a-single-invoice"></a>Procédure : Regroupement de bons de réception sur une seule facture
Si vous voulez facturer plusieurs réceptions achat en une fois, vous pouvez utiliser la fonction **Regroupement des réceptions**.  

Avant de pouvoir regrouper des réceptions achat, plusieurs réceptions achat du même fournisseur doivent être validées dans la même devise. En d'autres termes, vous devez avoir renseigné au moins deux commandes achat et les avoir validées comme reçues, mais non facturées.  

Lorsque des réceptions achat sont regroupées sur une facture et validées, une facture achat enregistrée est créée pour les lignes facturées. Le champ **Quantité facturée** de la commande achat d'origine, ou de la commande ouverte achat, est mis à jour en fonction de la quantité facturée. Comme ce document d'achat d'origine n'est toutefois pas supprimé, même s'il a été entièrement reçu et facturé, vous devez supprimer le document d'achat.  

## <a name="to-combine-receipts"></a>Pour regrouper des réceptions  
1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Factures achat**, puis sélectionnez le lien connexe.  
2. Sélectionnez l'action **Nouveau**. Pour plus d'informations, reportez-vous à [Procédure : enregistrer des achats](purchasing-how-record-purchases.md).  
3. Dans le raccourci **Lignes**, sélectionnez l'action **Extraire lignes réception**.  
4. Sélectionnez plusieurs lignes réception à inclure dans la facture.  

    Si une ligne réception incorrecte a été sélectionnée ou que vous souhaitez recommencer, il vous suffit de supprimer les lignes de la facture achat et d'utiliser à nouveau la fonction **Extraire lignes réception**.  
5. Pour valider la facture, sélectionnez l'action **Valider**.  

## <a name="to-remove-open-purchase-orders-after-combined-receipt-posting"></a>Pour supprimer des commandes achat ouvertes après la validation de reçus regroupés  
1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Supprimer les commandes achat facturées**, puis sélectionnez le lien connexe.  
2. Renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)].
3. Cliquez sur le bouton **OK**.  

Vous pouvez également supprimer chacune des commandes manuellement.

Répétez les étapes 1 à 3 pour tous les autres documents affectés, comme des commandes ouvertes achat.

## <a name="see-also"></a>Voir aussi  
[Achats](purchasing-manage-purchasing.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

