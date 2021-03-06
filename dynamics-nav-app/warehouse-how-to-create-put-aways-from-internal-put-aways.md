---
title: "Procédure : créer un rangement à partir du rangement interne"
description: "Lorsque les articles ont été rangés et avant d'être prélevés pour répondre aux besoins d'un ordre de fabrication ou d'une expédition, ils sont stockés dans l'entrepôt comme faisant partie du stock disponible."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 970b9b9046018b0dcea5b9996d10e19e444a7639
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-pick-and-put-away-without-a-source-document"></a>Procédure : Prélever et ranger sans document origine
Lorsque les articles ont été rangés et avant d'être prélevés pour répondre aux besoins d'un ordre de fabrication ou d'une expédition, ils sont stockés dans l'entrepôt comme faisant partie du stock disponible.  

Vous pouvez être amené à sortir temporairement des articles des emplacements prélèvement entrepôt, par exemple pour les présenter au cours d'une argumentation. Ces articles appartiennent toujours à la société et font partie du stock ; par contre, ils ne peuvent pas être prélevés. Ils sont enregistrés dans un emplacement spécial que vous créez à cet effet ; techniquement, les articles se trouvent dans l'entrepôt, mais physiquement, ils peuvent se trouver dans une salle de conférences ou d'exposition.  

Il peut également arriver que l'unité de fabrication ait inopinément besoin de quelques pièces pour un processus. Vous pouvez prélever des articles pour les emplacements fabrication à l'aide du prélèvement interne. Une fois le processus terminé et la fabrication réalisée, vous validez la consommation des articles et videz l'emplacement fabrication, ce qui a pour effet de réduire la quantité de l'article dans votre magasin.  

De même, des articles peuvent être retournés à l'entrepôt pour être rangés. Les articles ont pu être prélevés dans le stock disponible pour un ordre de fabrication, puis non utilisés. Pour qu'ils fassent de nouveau partie du stock disponible, ils doivent faire l'objet d'un rangement dans l'emplacement.  

Les **rangements internes** vous permettent d'effectuer des rangements sans avoir à vous référer à un document origine spécifique. Vous pouvez facilement configurer toutes les informations nécessaires pour créer une instruction entrepôt de rangement.  

> [!NOTE]  
>  Lorsque vous n'utilisez pas de prélèvements internes ni de rangements internes, vous pouvez effectuer ces ajustements en déplaçant les articles d'un emplacement à un autre ou en validant les ajustements des quantités d'un emplacement.  
>   
>  Lorsque le magasin utilise les prélèvement et rangement suggérés et, par conséquent, utilise des types emplacement, vous ne pouvez pas déplacer manuellement des articles vers ou depuis un emplacement de type RECEPTIONNER, car les articles dans ce type d'emplacement doivent être enregistrés comme étant rangés avant de faire partie du stock disponible.  

## <a name="to-create-an-internal-pick"></a>Pour créer un prélèvement interne  
1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Prélèvement interne entrepôt**, puis sélectionnez le lien connexe.  
2.  Renseignez le champ **N°** et **Vers code emplacement** du raccourci **Général**. Le champ **Du code emplacement** indique l'emplacement où se trouvent les articles que vous souhaitez. Pour des raisons de fabrication, cet emplacement représente l'emplacement enlogement ou l'emplacement atelier ouvert. Pour d'autres raisons, vous devez choisir un code emplacement de destination d'un type emplacement qui n'est pas utilisé pour le prélèvement (par exemple, un emplacement affectation, expédition ou un emplacement spécial).  
3.  Sélectionnez un article dans le champ **N° article**, puis renseignez les quantités à prélever.  
4. Choisissez l'action **Créer prélèvement**. Une instruction prélèvement entrepôt est maintenant créée pour un magasinier.  

## <a name="to-create-an-internal-put-away"></a>Pour créer un rangement interne  
1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Prélèvement interne entrepôt**, puis sélectionnez le lien connexe.  
2.  Renseignez le champ **N°** et **Du code emplacement** du raccourci **Général**. Le champ **Du code emplacement** indique l'emplacement où se trouvent les articles retournés à l'entrepôt (par l'unité de production, par exemple).  
3.  Renseignez les numéros article et les quantités sur les lignes.  
4.  Choisissez l'action **Créer rangement**. Une instruction rangement entrepôt est maintenant créée pour un magasinier.  

## <a name="see-also"></a>Voir aussi  
[Gestion d'entrepôt](warehouse-manage-warehouse.md)  
[STOCKS ET EN-COURS](inventory-manage-inventory.md)  
[Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md)     
[Gestion des assemblages](assembly-assemble-items.md)    
[Détails de conception : gestion d'entrepôt](design-details-warehouse-management.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

