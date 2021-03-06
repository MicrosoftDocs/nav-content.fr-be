---
title: "Procédure : déplacer des articles dans les configurations de stockage avancées"
description: "Dans des configurations d'entrepôt avancées, c'est-à-dire des magasins avec prélèvement et rangement dirigé, des mouvements entrepôt entre emplacements sont exécutés par un cadre qui prépare des mouvements entrepôt dans la feuille mouvement, puis crée les mouvements entrepôt que les magasiniers doivent exécuter."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/232017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: a7e26a8910b0cf7d8a78b7f86291d9cfd5d18bec
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-move-items-in-advanced-warehouse-configurations"></a>Procédure : déplacer des articles dans les configurations de stockage avancées
Dans des configurations d'entrepôt avancées, c'est-à-dire des magasins avec prélèvement et rangement dirigé, des mouvements entrepôt entre emplacements sont exécutés par un cadre qui prépare des mouvements entrepôt dans la feuille mouvement, puis crée les mouvements entrepôt que les magasiniers doivent exécuter.  

## <a name="to-move-items-with-the-warehouse-movement-worksheet"></a>Pour déplacer des articles avec la feuille mouvement entrepôt
La fenêtre **Feuille mouvement** a deux fonctions qui peuvent vous aider à renseigner automatiquement les lignes. La première est la fonction **Calculer réappro. emplacement**. Cette fonction utilise les priorités emplacement pour suggérer le réapprovisionnement des emplacements les mieux classés à partir de ceux moins bien classés. La seconde est la fonction de **Extraire contenu emplacement**, qui renseigne les lignes feuille avec tout le contenu des emplacements que vous spécifiez.

1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuille mouvement**, puis sélectionnez le lien connexe.  
2.  Renseignez comme il convient les informations de mouvement d'entrepôt dans les lignes de la feuille.  
3. Choisissez l'action **Créer mouvement** pour créer un document mouvement entrepôt qui pourra être ensuite enregistré lorsque le mouvement sera terminé.  

### <a name="to-register-the-warehouse-movement"></a>Pour enregistrer le mouvement d'entrepôt  
1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Mouvements**, puis sélectionnez le lien connexe.  
2.  Ouvrez le mouvement entrepôt que vous souhaitez traiter.  
3.  Sur les lignes dont le type d'action est **Emplacement**, spécifiez où, quoi et quand déplacer l'article concerné en modifiant les champs **Code zone**, **Code emplacement** ou **Qté à traiter**, ou **Date d'échéance** .  

    Si votre entrepôt a été configuré de façon à ce que les codes emplacement suivent la structure physique de l'entrepôt, vous pouvez prendre des quantités de plusieurs articles dans des emplacements consécutifs, puis les placer dans des emplacements de prélèvement se trouvant en aval et pouvant être proches les uns des autres.  
4.  Sur les lignes dont le type d'action est **Prélever**, indiquez dans le champ **Qté à traiter** une quantité du contenu emplacement que vous souhaitez déplacer. Tous les autres champs sur les lignes dont le type d'action est **Prélever** sont en lecture seule.  
5.  Pour déplacer toutes les quantités proposées comme spécifiées dans le champ **Quantité**, choisissez l'action **Renseigner automatiquement la quantité à traiter**.  
6. Sélectionnez l'action **Enregistrer**.  

> [!NOTE]  
>  Si le magasin utilise des prélèvement et rangement suggérés, vous ne pouvez pas déplacer manuellement des articles vers ou depuis un emplacement de type RÉCEPTIONNER, car les articles dans ce type d'emplacement doivent être enregistrés comme étant rangés avant de faire partie du stock disponible.

## <a name="to-register-the-movement-of-an-item-that-has-already-occurred"></a>Pour enregistrer un mouvement d'un article déjà terminé  
Si, en cas d'utilisation d'un prélèvement et d'un rangement suggérés dans le magasin, vous devez déplacer des articles vers d'autres emplacements sans rangement, prélèvement ou mouvement entrepôt préexistant, vous pouvez alors enregistrer l'emplacement exact des articles dans l'entrepôt à l'aide de la fonction **Feuille reclassement entrepôt**.

1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuille reclassement entrepôt**, puis sélectionnez le lien connexe.  
2.  Renseignez les champs **N° article**, **Du code zone**, **Du code emplacement**, **Vers code zone** et **Du code emplacement**.  
3.  Sélectionnez l'action **Enregistrer**.  

## <a name="see-also"></a>Voir aussi  
[Gestion d'entrepôt](warehouse-manage-warehouse.md)  
[STOCKS ET EN-COURS](inventory-manage-inventory.md)  
[Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md)     
[Gestion des assemblages](assembly-assemble-items.md)    
[Détails de conception : gestion d'entrepôt](design-details-warehouse-management.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

