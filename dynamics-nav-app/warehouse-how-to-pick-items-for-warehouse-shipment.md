---
title: "Comment prélever des articles pour l'expédition entrepôt"
description: "Lorsque le magasin est configuré pour appeler un traitement de prélèvement entrepôt et un traitement d'expédition entrepôt, vous pouvez utiliser les documents prélèvement entrepôt pour créer et traiter les informations préalables à la validation de l'expédition entrepôt."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 256f7cfc0348b121a1302db49e57fa030b76f55c
ms.contentlocale: fr-be
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-pick-items-for-warehouse-shipment"></a>Comment prélever des articles pour l'expédition entrepôt
Lorsque le magasin est configuré pour appeler un traitement de prélèvement entrepôt et un traitement d'expédition entrepôt, vous pouvez utiliser les documents prélèvement entrepôt pour créer et traiter les informations préalables à la validation de l'expédition entrepôt.  

Vous ne pouvez pas créer de toutes pièces un document prélèvement entrepôt car une activité de prélèvement fait toujours partie d'un flux de travail, soit dans un scénario d'extraction, soit dans un scénario de déplacement.  

Vous pouvez créer des documents prélèvement entrepôt en mode extraction en ouvrant un document expédition entrepôt vide, détecter les documents origine qui sont lancés à l'expédition, puis créer des lignes prélèvement entrepôt pour ces expéditions. Vous pouvez utiliser les fonctions **Obtenir documents origine** ou **Utiliser filtre pour obtenir documents origine** pour détecter les documents origine qui sont prêts à l'expédition.

Sinon, vous pouvez utiliser la fenêtre **Feuille prélèvement** pour extraire et créer les lignes prélèvement en mode lots. Pour plus d'informations, voir [Procédure : planifier des prélèvements dans des feuilles](warehouse-how-to-plan-picks-in-worksheets.md).  

Vous pouvez également créer des documents prélèvement entrepôt en mode pousser à partir de la fenêtre **Expédition entrepôt** en sélectionnant **Créer prélèvement**.  

> [!NOTE]  
>  Le prélèvement pour l'expédition entrepôt des articles assemblés à la commande vente en cours d'expédition suit les mêmes étapes que les prélèvements entrepôt ordinaires pour l'expédition, comme décrit dans cette rubrique. Cependant, le nombre de lignes prélèvement par quantité à livrer peut grandement varier car le prélèvement entrepôt concerne les composants et non l'élément d'assemblage.  
>   
>  Les lignes prélèvement entrepôt sont créées suivant la valeur du champ **Quantité restante** sur les lignes de l'ordre d'assemblage associé à la ligne commande vente en cours d'expédition. Ceci garantit le prélèvement de tous les composants en une seule action.  
>   
>  Pour plus d’informations, reportez-vous à la section « Traitement des articles à assembler pour commande dans les expéditions entrepôt ».  
>   
>  Pour plus d'informations sur le prélèvement de composants pour les ordres d'assemblage en général, notamment les situations où l'élément d'assemblage n'est pas dû dans une expédition vente, voir [Procédure : prélever pour la fabrication ou l'assemblage](warehouse-how-to-pick-for-production.md).  

## <a name="to-pick-items-for-warehouse-shipment"></a>Pour prélever des articles pour l'expédition entrepôt  
1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Prélèvements**, puis sélectionnez le lien connexe.  

    Si vous souhaitez travailler à un prélèvement particulier, sélectionnez-le dans la liste ou filtrez cette dernière afin de trouver les prélèvements qui vous ont été spécifiquement affectés. Ouvrez la fiche prélèvement.  
2.  Si le champ **ID utilisateur affecté** est vide, entrez votre ID pour vous identifier si nécessaire.  
3.  Exécutez le prélèvement réel des articles.  

    Si le magasin est configuré pour utiliser des emplacements, les emplacements par défaut des articles sont utilisés pour suggérer où prendre les articles. Les instructions apparaissent sur deux lignes distinctes, une ligne au moins pour chaque type d'action, prélèvement et placement.  

    Si l'entrepôt est configuré pour utiliser un prélèvement et rangement dirigé, le classement d'emplacement est utilisé pour calculer les meilleurs emplacements d'où prélever, et ces emplacements sont ensuite suggérés sur les lignes prélèvement. Les instructions apparaissent sur deux lignes distinctes, une ligne au moins pour chaque type d'action, prélèvement et placement.  

4.  Lorsque vous avez effectué le prélèvement et placé les articles dans la zone ou l'emplacement d'expédition, choisissez l'action **Enregistrer prélèvement**.  

La personne responsable de l'expédition peut alors apporter les articles au quai de chargement et valider l'expédition, dont le document origine lié, dans la fenêtre **Expédition entrepôt** . Pour plus d'informations, voir [Procédure : Expédier des articles](warehouse-how-ship-items.md).   

En plus de prélever les documents origine, comme indiqué dans cette rubrique, vous pouvez prendre et placer les articles entre les emplacements sans faire référence aux documents origine. Pour plus d'informations, voir [Procédure : Prélever et ranger sans document origine](warehouse-how-to-create-put-aways-from-internal-put-aways.md).  

## <a name="handling-assemble-to-order-items-in-warehouse-shipments"></a>Traitement des articles à assembler pour commande dans les expéditions entrepôt
Dans des scénarios d'assemblage pour commande, le champ **Qté à expédier** sur les lignes expédition entrepôt est utilisé pour enregistrer le nombre d'unités assemblées. La quantité spécifiée est ensuite validée comme résultats d'assemblage lorsque l'expédition entrepôt est validée.

Pour d'autres lignes expédition entrepôt, la valeur du champ **Qté à expédier** est zéro dès le début.

Lorsque les travailleurs chargés de l’assemblage finissent d’assembler les pièces ou l’ensemble de la quantité à assembler pour commande, ils l’enregistrent dans le champ **Qté à expédier** de la ligne expédition entrepôt dans les configurations avancées et sélectionnent ensuite l'action **Valider expédition**. Le résultat est que les résultats d'assemblage correspondants sont validés, y compris la consommation de composants. Une expédition vente pour la quantité est validée pour la commande vente.

À partir de l'ordre d'assemblage, vous pouvez choisir **Ligne expédition entrepôt Assembler pour commande** pour accéder à la ligne expédition entrepôt. Ceci peut être utile pour les travailleurs qui n'utilisent pas généralement la fenêtre **Expédition entrepôt**.

Une fois l'expédition entrepôt validée, divers champs de la ligne commande vente sont mis à jour pour afficher la progression dans l'entrepôt. Les champs suivants sont également mis à jour pour afficher le nombre de quantités à assembler pour commande qui restent à être assemblées et expédiées :

- **Qté restante entrepôt ATO**
- **Qté restante entrepôt ATO (base)**

> [!NOTE]
> Dans les scénarios de combinaison, où une partie de la quantité doit d'abord être assemblée et l'autre doit être expédiée à partir des stocks, deux lignes expédition entrepôt sont créées. L'une est pour la quantité à assembler pour commande et l'autre est destinée à la quantité en stock.

> Dans ce cas, la quantité à assembler pour commande est traitée comme décrite dans cette rubrique, et la quantité en stock est traitée comme toute autre ligne expédition entrepôt normale. Pour plus d'informations sur les scénarios de combinaison, consultez [Description des processus Assembler pour commande et Assembler pour stock](assembly-assemble-to-order-or-assemble-to-stock.md).

## <a name="see-also"></a>Voir aussi  
[Gestion d'entrepôt](warehouse-manage-warehouse.md)  
[STOCKS ET EN-COURS](inventory-manage-inventory.md)  
[Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md)     
[Gestion des assemblages](assembly-assemble-items.md)    
[Détails de conception : gestion d'entrepôt](design-details-warehouse-management.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

