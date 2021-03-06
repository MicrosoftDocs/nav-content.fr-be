---
title: Comment transborder des articles
description: "La fonctionnalité de transbordement est disponible si le magasin est configuré pour appeler un traitement à la fois de réception entrepôt et de rangement magasin."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 2103f5f284e29bb81f24dec668a9d03f741327c9
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-cross-dock-items"></a>Comment transborder des articles
La fonctionnalité de transbordement est disponible si le magasin est configuré pour appeler un traitement à la fois de réception entrepôt et de rangement magasin.  

Lorsque vous transbordez des articles, vous les manipulez en effectuant des réceptions et des expéditions, sans jamais les ranger. Vous évitez ainsi les processus de rangement et de prélèvement, et limitez la manipulation physique des articles. Vous pouvez transborder des articles pour des expéditions comme pour des ordres de fabrication. Lorsque vous préparez une expédition ou prélevez des articles pour la production, et que vous utilisez des emplacements, le programme tente d'abord automatiquement de prélever l'article dans un emplacement de transbordement avant d'envisager d'autres emplacements. Vous devez vérifier si les articles dont vous avez besoin sont disponibles dans la zone de transbordement avant de pouvoir accéder à ces articles dans leur zone de stockage habituel.  

Lorsque vous avez calculé les quantités à transborder, des lignes rangement désignant l'emplacement de transbordement sont créées pour effectuer les calculs de transbordement lors de la validation de la réception. Les autres lignes rangement sont créées normalement.  

Pour valider immédiatement les articles à transborder afin qu'ils soient disponibles pour le prélèvement, vous devez aussi enregistrer un rangement pour les autres articles issus de la ligne réception, c'est-à-dire les articles à ranger. Si une partie seulement des articles d'une ligne réception doit être transbordée, efforcezvous de ranger le reste des articles le plus vite possible. Sinon, vous pouvez aussi instaurer dans votre entrepôt une politique encourageant les employés à effectuer le transbordement de lignes réception entières chaque fois que cela est possible.  

Dans l'instruction de rangement, vous avez tout intérêt à effacer les lignes d'instructions, les lignes prélèvement et placement de chaque ligne réception, concernant des réceptions qui doivent être entièrement rangées. Ces lignes pourront être créées ultérieurement en tant que lignes rangement à partir de la feuille rangement ou de la réception enregistrée. Une fois ces lignes effacées, vous pouvez ranger les articles à transborder et enregistrer les lignes concernant ces articles.  

Si vous avez sélectionné le champ **Utiliser feuille rangement** de la fiche magasin et validé votre réception en calculant les transbordements, toutes les lignes réception sont disponibles dans la feuille. Les informations de transbordement sont perdues et ne peuvent plus être créées. Par conséquent, pour utiliser la fonctionnalité de transbordement, il vaut mieux que vous transfériez les lignes vers la feuille rangement en effaçant les instructions de rangement plutôt que d'utiliser la fonction de transfert automatique prévue dans le champ **Utiliser feuille rangement**.  

Lorsque vous validez la réception entrepôt, et que le champ **Utiliser feuille rangement** n'est pas activé, les articles à transborder figurent dans des lignes distinctes dans l'instruction de rangement. Le champ **Informations transbordement** de chaque ligne rangement indique si la ligne contient des articles à transborder, des articles provenant d'une même réception et devant tous être rangés ou des articles à ranger provenant d'une ligne réception dans laquelle certains des articles sont à transborder. Grâce à ce champ, les employés peuvent voir aisément pourquoi toute la quantité réceptionnée n'est pas rangée.  

Le programme ne crée pas d'enregistrement distinct concernant les articles transbordés, mais les enregistre plutôt en tant qu'instructions de rangement ordinaires.  

## <a name="to-set-up-the-warehouse-for-cross-docking"></a>Pour configurer l'entrepôt en vue du transbordement  
1.  En cas d'utilisation d'emplacements, configurez au moins un emplacement de transbordement. En cas d'utilisation d'un prélèvement et d'un rangement suggérés, configurez une zone de transbordement.  

    Le champ **Emplacement transbordement** d'un emplacement de transbordement est activé. Son type d'emplacement doit correspondre à celui activé dans les champs **Réception** et **Prélèvement**. Pour plus d'informations, voir [Procédure : créer des emplacements](warehouse-how-to-create-individual-bins.md) et [Procédure : configurer des types d'emplacement](warehouse-how-to-set-up-bin-types.md).  

    Si vous utilisez des zones, créez une zone pour vos emplacements de transbordement, puis sélectionnez le champ **Transborder zone emplacement**. Pour plus d'informations, reportez-vous à [Comment configurer des magasins de sorte qu'ils utilisent des emplacements](warehouse-how-to-set-up-locations-to-use-bins.md).  

2.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Magasin**, puis sélectionnez le lien connexe.  
3.  Dans la fenêtre **Magasin**, sélectionnez le magasin que vous souhaitez configurer pour le transbordement, puis choisissez l'action **Modifier**.  
4.  Sur le raccourci **Entrepôt**, cochez la case **Utiliser transbordement**, puis renseignez le champ **Délai transbordement** en y indiquant la période pendant laquelle le programme doit rechercher des opportunités de transbordement.

    L'option **Utiliser transbordement** n'est disponible que si vous avez activé les champs **Réception requise**, **Expédition requise**, **Prélèvement requis** et **Rangement requis**.  

5.  Sur le raccourci **Emplacements**, renseignez le champ **Code emplacement transbord.** en y insérant le code de l'emplacement à utiliser comme emplacement de transbordement par défaut.  
6.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Point de stock**, puis choisissez le lien connexe.  
7.  Pour chaque article ou point de stock que vous souhaitez pouvoir transborder, sélectionnez l'article, puis cliquez sur l'action **Modifier**.
8. Dans la fenêtre **Fiche point de stock**, cochez la case **Utiliser transbordement**.  

> [!NOTE]  
>  Le transbordement n'est possible que si le magasin est configuré pour appeler un traitement à la fois de réception entrepôt et de rangement magasin.  

## <a name="to-cross-dock-items-without-viewing-the-opportunities"></a>Pour transborder des articles sans afficher les opportunités  
1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Réceptions entrepôt**, puis sélectionnez le lien connexe.  
2.  Créer des réceptions entrepôt pour un article qui est arrivé et qui pourrait nécessiter un transbordement. Pour plus d'informations, voir [Procédure : réceptionner des articles](warehouse-how-receive-items.md).  
3.  Renseignez le champ **Qté à recevoir**, puis choisissez l'action **Calculer transbordement**.  

    Les documents origine sortants demandant les articles qui doivent quitter l'entrepôt durant la période indiquée par la formule date sont identifiés.  [!INCLUDE[d365fin](includes/d365fin_md.md)] calcule les quantités pour que vous puissiez effectuer un maximum de transbordements pour éviter de ranger des articles, sans entasser trop d'articles dans la zone de transbordement. La valeur du champ **Qté à transborder** est ainsi la plus petite de ces deux valeurs : la somme de toutes les lignes sortantes demandant l'article avant la fin de la période de prévision des transbordements, moins la quantité d'articles déjà placés dans la zone de transbordement ou la valeur du champ **Qté à recevoir** de la ligne réception. (Vous ne pouvez pas transborder plus d'articles que vous en avez reçus.  

4.  Pour transborder la quantité en suivant la procédure indiquée, validez la réception. Vous pouvez aussi décider de modifier la quantité à transborder pour augmenter ou réduire sa valeur, puis valider la réception.  

    Les quantités à transborder apparaissent maintenant en tant que lignes dans l'instruction de rangement, en supposant que vous n'ayez pas activé le champ **Utiliser feuille rangement**. Les quantités non destinées au transbordement apparaissent aussi en tant que lignes dans l'instruction de rangement.  

    Si vous possédez des emplacements, les articles transbordés ont été affectés à l'emplacement de transbordement par défaut défini dans la fiche magasin.  

5.  Supprimez les lignes **prélèvement** et **placement** pour les articles qui ne font l'objet d'aucun transbordement.  
6.  Imprimez l'instruction de rangement pour les lignes restantes, puis placez les quantités de la réception à ranger dans les emplacements appropriés ou dans la zone appropriée de l'entrepôt. Placez les articles à transborder dans la zone ou l'emplacement qui leur est attribué par la politique de l'entrepôt. Parfois, la politique de l'entrepôt peut nécessiter simplement de les laisser dans la zone de réception.  
7.  Pour enregistrer les articles transbordés comme étant rangés et disponibles pour le prélèvement, choisissez l'action **Enregistrer**.  

## <a name="to-cross-dock-items-after-viewing-the-opportunities"></a>Pour transborder des articles après avoir affiché les opportunités  
1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Réceptions entrepôt**, puis sélectionnez le lien connexe.  
2.  Créer des réceptions entrepôt pour un article qui est arrivé et qui pourrait nécessiter un transbordement. Pour plus d'informations, voir [Procédure : réceptionner des articles](warehouse-how-receive-items.md).  

    Vous souhaitez afficher les lignes document origine demandant l'article avant de valider la réception.  
3.  Choisissez l'action **Calculer transbordement**.  

    Dans la fenêtre **Opportunités transbordement**, vous pouvez voir les informations les plus importantes concernant les lignes demandant l'article, comme le type du document, la quantité demandée et la date d'échéance. Ces informations peuvent vous aider à décider de la quantité d'articles à transborder, de l'endroit où placer ces articles dans la zone de transbordement ou de la manière de les regrouper.  

4.  Choisissez l'action **Remplir quantité à transborder** pour savoir comment les quantités figurant dans les lignes réception sont calculées. Lorsque vous modifiez le nombre d'articles dans le champ **Qté à transborder** de chaque ligne, le calcul est mis à jour lorsque vous effectuez des modifications. Cela ne signifie pas que l'expédition ou l'ordre de fabrication concerné reçoit réellement les articles dont le transbordement est proposé, car ces opérations ne sont qu'un simple test. Toutefois, ce processus peut être intéressant à titre d'information si plusieurs unités de mesure sont utilisées.  
5.  Pour réserver une quantité de l'article pour une ligne commande donnée, placez le curseur sur cette ligne, puis choisissez l'action **Réserver**. Dans la fenêtre **Réservation**, vous pouvez maintenant réserver n'importe quelle quantité disponible de l'article pour cette commande. Cette réservation ne diffère pas des autres réservations, et le fait qu'elle ait été créée au cours d'un transbordement ne lui confère aucune priorité. Pour plus d'informations, voir [Procédure : réserver des articles](inventory-how-to-reserve-items.md).   
6.  Lorsque vous avez fini de refaire les calculs et que la réservation est terminée, sélectionnez le bouton **OK** pour insérer le calcul que vous venez de réviser dans le champ **Qté à transborder** de la ligne réception ou choisissez le bouton **Annuler** pour revenir à la réception entrepôt et y recalculer le transbordement.  
7.  Validez à présent la réception. Vous pouvez ensuite passer à l'instruction de rangement, comme l'indiquent les étapes 3 à 7 de la section « Pour transborder des articles sans afficher les opportunités ».  

> [!NOTE]  
>  Dans le rangement entrepôt, vous pouvez continuer de modifier les quantités en cours de transbordement ou de rangement dans le stock, selon vos besoins. Par exemple, vous pouvez décider de transborder une quantité supplémentaire afin d'expédier l'enregistrement du transbordement.  

## <a name="to-view-cross-docked-items-in-a-shipment-or-pick-worksheet"></a>Affichage d'articles transbordés dans une expédition ou une feuille prélèvement  
Si vous possédez des emplacements, chaque fois que vous ouvrez une expédition ou la feuille prélèvement, vous pouvez voir le calcul mis à jour de la quantité de chaque article dans les emplacements de transbordement. Cette information est précieuse si vous attendez l'arrivée d'un article. Dès que vous voyez qu'un article est disponible dans l'emplacement de transbordement, vous pouvez rapidement créer un prélèvement pour tous les articles de l'expédition. Dans la feuille prélèvement, vous pouvez modifier les lignes, puis créer un prélèvement.  

Pour prélever des articles à expédier, vous devez commencer par rechercher les articles concernés dans la zone de transbordement. Si, au cours du processus de réception, vous avez noté les documents origine à la base du transbordement, vous saurez plus précisément si l'article que vous recherchez se trouve ou non dans la zone de transbordement.  

Après le lancement d'un ordre de production, les lignes sont disponibles dans la feuille prélèvement et vous pouvez consulter le champ **Qté empl. transbordement** pour voir si les articles que vous attendez sont arrivés et ont été placés dans les emplacements de transbordement. Lorsque vous créez une instruction de prélèvement, le programme vous propose de prélever d'abord les articles transbordés, après quoi il recherche les articles dans les emplacements de stockage.  

Si vous n'utilisez pas d'emplacements, n'oubliez pas de vérifier, de temps en temps, la zone de transbordement ou consultez les notifications de réception pour connaître l'arrivée des articles destinés à la production.  

## <a name="see-also"></a>Voir aussi  
[Gestion d'entrepôt](warehouse-manage-warehouse.md)  
[STOCKS ET EN-COURS](inventory-manage-inventory.md)  
[Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md)     
[Gestion des assemblages](assembly-assemble-items.md)    
[Détails de conception : gestion d'entrepôt](design-details-warehouse-management.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

