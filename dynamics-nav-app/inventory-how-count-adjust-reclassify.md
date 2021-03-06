---
title: Inventaire, ajustement et reclassement du stock
description: "Décrit la manière d'effectuer un inventaire physique, faire des ajustements négatifs ou positifs, et comment modifier des informations, telles que le magasin ou le numéro de lot, sur des écritures comptables article ou des écritures entrepôt."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: adjustment, negative, positive, increase, decrease
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 4d53e6e9b64e0f5c790abb0f62f66a2b28c12c50
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-count-adjust-and-reclassify-inventory"></a>Procédure : Inventaire, ajustement et reclassement du stock
Vous devez effectuer un inventaire (c'est-à-dire compter tous les articles disponibles) au moins une fois par exercice pour vérifier si la quantité enregistrée dans la base de données est identique à la quantité réelle en stock dans les entrepôts. Lorsque vous connaissez la quantité physique réelle, vous devez la valider dans la comptabilité dans le cadre de l' évaluation du stock de fin d'exercice.

Bien que vous comptiez tous les articles du stock au moins une fois par an, vous pouvez avoir décidé de compter certains articles plus souvent, parce qu'ils ont plus de valeur ou parce qu'ils sont très demandés et représentent une partie importante de votre activité. Pour cela, vous pouvez affecter des périodes d'inventaire spéciales à ces articles. Pour plus d'informations, reportez-vous à la section « Effectuer un inventaire tournant ».

Pour ajuster les quantités en stock enregistrées, pour inventaire ou à d'autres fins, vous pouvez utiliser une feuille article pour modifier les écritures comptables inventaire directement sans valider les transactions commerciales. Sinon, vous pouvez ajuster pour un article distinct de la fiche article.

Pour modifier les attributs d'écritures comptables article et les quantités, vous pouvez utiliser la feuille reclassement article. Les attributs courants pour les reclassements incluent les numéros de série et/ou de lot, les dates d'expiration et les dimensions.

> [!NOTE]
> Dans les configurations d'entrepôt avancées, les articles sont enregistrés dans des emplacements en tant qu'écritures entrepôt, pas en tant qu'écritures comptables article. Par conséquent, vous effectuez l'inventaire, l'ajustement et le reclassement dans des feuilles entrepôt spéciales qui prennent en charge les emplacements. Ensuite, vous utilisez des fonctions spéciales pour synchroniser les écritures entrepôt nouvelles ou modifiées avec leurs écritures comptables article correspondantes pour refléter les modifications des quantités et valeurs en stock. Ceci est décrit dans des procédures spécifiques ci-dessous lorsque cela est approprié.

## <a name="to-perform-a-physical-inventory"></a>Pour effectuer un inventaire physique
A la fin de l'exercice comptable, ou plus souvent, vous devez effectuer un inventaire, c'est-à-dire compter les articles réellement disponibles, pour vérifier si la quantité enregistrée correspond à la quantité réelle du stock. S'il existe des différences, vous devez les valider dans les comptes article avant de procéder à l'évaluation du stock.

Outre la tâche de comptage réelle, le processus complet implique les trois tâches suivantes :

- Calculer le stock prévu.
- Imprimer l'état à utiliser lors du comptage.
- Saisir et valider le stock réel compté.

Vous pouvez effectuer l'inventaire physique de l'une des manières suivantes en fonction de votre configuration entrepôt. Pour plus d'informations, voir [Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md).  

-   Si votre magasin n'utilise pas le prélèvement et rangement suggérés (configuration d'entrepôt de base), vous pouvez utiliser la fenêtre **Feuille inventaire** du menu **Stock** ; la procédure est similaire à celle d'un inventaire sans inventaire tournant.  
-   Si votre magasin utilise le prélèvement et rangement suggérés (configuration d'entrepôt avancée), vous utilisez d'abord la fenêtre **Feuille inventaire entrepôt**, puis vous utilisez la fenêtre **Feuille article** pour exécuter la fonction **Calculer ajustement entrepôt**.

### <a name="to-calculate-the-expected-inventory-in-basic-warehouse-configurations"></a>Pour calculer le stock prévu dans les configurations d'entrepôt de base
1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuilles inventaire**, puis sélectionnez le lien connexe.
2. Choisissez l'action **Calculer stock**.
3. Dans la fenêtre **Calculer stock**, indiquez les conditions à utiliser pour créer les lignes feuille, par exemple si vous souhaitez inclure les articles pour lesquels aucun stock n'est enregistré.
4. Définissez des filtres si vous souhaitez uniquement calculer le stock pour certains articles, emplacements, magasins ou axes.
5. Cliquez sur le bouton **OK**.

> [!NOTE]  
>   Les écritures article sont traitées en fonction des informations que vous avez indiquées, et les lignes sont créées dans la feuille inventaire. Notez que le champ **Qté (constatée)** est renseigné automatiquement avec la même quantité que le champ **Qté (calculée)**. Avec cette fonction, vous n'avez pas besoin d'entrer le stock disponible pour les articles dont le nombre correspond à la quantité calculée. Toutefois, si la quantité comptée diffère de ce qui est saisi dans le champ **Qté (calculée)**, vous devez la remplacer par la quantité réellement comptée.

### <a name="to-calculate-the-expected-inventory-in-advanced-warehouse-configurations"></a>Pour calculer le stock prévu dans les configurations d'entrepôt avancées
1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Feuille article**, puis sélectionnez le lien connexe.  
2.  Sélectionnez l'action **Calculer ajustement entrepôt**.  
3.  Renseignez le formulaire de sélection du traitement par lots en y indiquant votre magasin et les numéros des articles que vous souhaitez compter.
4. Cliquez sur le bouton **OK**, puis validez les éventuels ajustements.

    Si vous n'effectuez pas cette opération avant d'exécuter l'inventaire entrepôt, les résultats que vous validez dans la feuille inventaire et dans l'écriture article dans la deuxième partie de la procédure seront les résultats de l'inventaire combinés avec d'autres ajustements entrepôt pour les articles comptés.  
5.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Feuille inventaire entrepôt**, puis sélectionnez le lien connexe.  
6. Choisissez l'action **Calculer stock**. Le formulaire de sélection du traitement par lots **Calculer stock entrepôt** s'ouvre.  
7.  Positionnez les filtres permettant de limiter les articles comptés dans la feuille, puis sélectionnez le bouton **OK**.

    Le programme crée une ligne pour chaque emplacement répondant aux exigences des filtres. A ce stade, vous pouvez encore supprimer certaines lignes, mais si vous souhaitez valider les résultats en tant qu'inventaire, vous devez compter l'article dans tous les emplacements le contenant.  

     Si le temps dont vous disposez vous permet uniquement de compter l'article dans certains emplacements, vous pouvez noter les différences, les enregistrer, puis les valider dans la feuille article à l'aide de la fonction **Calculer ajustement entrepôt**.  
8.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Liste d'inventaire entrepôt**, puis sélectionnez le lien connexe.  
9.  Ouvrez la page de sélection de l'état, puis imprimez les listes sur lesquelles vous souhaitez que les employés enregistrent la quantité des articles qu'ils comptent dans chaque emplacement.  
10. Une fois le décompte effectué, saisissez les quantités comptées dans le champ **Qté (constatée)** de la feuille inventaire entrepôt.  

    > [!NOTE]  
    >  Dans la feuille d'inventaire physique de l'entrepôt, le champ **Qté (calculée)** est renseigné automatiquement sur la base des enregistrements d'emplacement entrepôt et des copies de ces quantités sont effectuées sur chaque ligne du champ **Qté (physique)**. Dans la feuille inventaire, le programme renseigne automatiquement le champ Qté (calculée) en fonction des enregistrements emplacement entrepôt et copie ces quantités dans le champ Qté (constatée) de chaque ligne.Si la quantité comptée par le magasinier est différente de celle saisie par le programme dans le champ Qté (constatée), vous devez saisir la quantité réellement comptée.  

11. Lorsque vous avez entré toutes les quantités comptées, sélectionnez l'action **Enregistrer**.  

    Lorsque vous enregistrez la feuille, le programme crée dans l'historique entrepôt deux écritures entrepôt pour chaque ligne comptée et enregistrée.  

    -   Si les quantités calculées et les quantités réelles sont différentes, une quantité négative ou positive est enregistrée pour l'emplacement, et la quantité équilibre est validée dans l'emplacement ajustement du magasin.  
    -   Si la quantité calculée est égale à la quantité réelle, le programme enregistre une écriture de 0 pour l'emplacement et l'emplacement ajustement. Les écritures indiquent qu'à la date d'enregistrement, un inventaire entrepôt a été effectué et qu'il n'y avait aucune différence pour l'article au niveau de l'inventaire.  

Lorsque vous enregistrez l'inventaire entrepôt, vous ne validez ni dans l'écriture article ni dans l'écriture inventaire ni dans l'écriture valeur, mais les enregistrements peuvent être utilisés lorsqu'un rapprochement immédiat est nécessaire. Cependant, si vous souhaitez conserver des enregistrements précis des événements entrepôt et que vous avez compté tous les emplacements où les articles étaient enregistrés, validez immédiatement les résultats entrepôt en tant qu'inventaire physique. Pour plus d'informations, voir la section « Pour saisir et valider le stock réel compté dans les configurations d'entrepôt avancées ».

### <a name="to-print-the-report-to-be-used-when-counting"></a>Pour imprimer l'état à utiliser lors de l'inventaire
1. Dans la fenêtre **Feuille inventaire** contenant le stock prévu calculé, choisissez l'action **Imprimer**.
2. Dans la fenêtre **Liste d'inventaire**, indiquez si l'état doit indiquer la quantité calculée et si l'état doit répertorier les articles en stock par numéros de série/lot.
3. Définissez des filtres si vous souhaitez uniquement imprimer l'état pour certains articles, emplacements, magasins ou axes.
4. Cliquez sur le bouton **Imprimer**.

Les employés peuvent maintenant poursuivre le comptage du stock et noter les éventuelles différences sur l'état imprimé.

### <a name="to-enter-and-post-the-actual-counted-inventory-in-basic-warehouse-configurations"></a>Pour saisir et valider le stock réel compté dans les configurations d'entrepôt de base
1. Sur chaque ligne de la fenêtre **Feuilles inventaire** sur laquelle le stock réellement disponible, comme déterminé par le comptage, diffère de la quantité calculée, saisissez la quantité réellement disponible dans le champ **Qté (constatée)**.

    Les champs associés sont mis à jour en conséquence.

    > [!NOTE]  
>   Si le décompte fait apparaître des différences dues à des articles validés avec des codes magasin incorrects, n'indiquez pas les différences dans la feuille inventaire. Au lieu de cela, utilisez la feuille reclassement ou un ordre de transfert pour rediriger les articles vers les magasins appropriés. Pour plus d'informations, voir Feuille reclassement article ou Procédure : créer des ordres de transfert.

2. Pour ajuster les quantités calculées avec les quantités comptées réelles, choisissez **Valider**.

    Les écritures comptables article et les écritures comptables inventaire sont créées. Ouvrez la fiche article pour visualiser les écritures comptables inventaire ainsi obtenues.

3. Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Articles**, puis sélectionnez le lien connexe.
4. Pour vérifier l'inventaire de stock, ouvrez la fiche article en question, puis choisissez **Écritures comptables inventaire**.

### <a name="to-enter-and-post-the-actual-counted-inventory-in-advanced-warehouse-configurations"></a>Pour saisir et valider le stock réel compté dans les configurations d'entrepôt avancées

1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Feuille article**, puis sélectionnez le lien connexe.  
2.  Sélectionnez l'action **Calculer ajustement entrepôt**.  
3.  Sélectionnez les articles que vous avez compté au cours de l'inventaire que vous venez de réaliser, et tous les autres articles nécessitant un ajustement, puis choisissez le bouton **OK**.  

     La fenêtre **Feuille inventaire** s'ouvre et des lignes sont créées pour ces articles. Remarquez que les quantités nettes que vous venez de compter et d'enregistrer emplacement par emplacement sont à présent prêtes à être consolidées et synchronisées comme écritures comptables article.  

4.  Validez la feuille sans modifier les quantités.  

Les quantités de l'écriture article (écritures article) et les quantités de l'entrepôt (écritures entrepôt) sont une nouvelle fois identiques pour ces articles ; en outre, le programme a mis à jour la dernière date inventaire de l'article ou du point de stock.  

## <a name="to-perform-cycle-counting"></a>Pour effectuer l'inventaire périodique
Bien que vous comptiez tous les articles du stock au moins une fois par an, vous pouvez avoir décidé de compter certains articles plus souvent, parce qu'ils ont plus de valeur ou parce qu'ils sont très demandés et représentent une partie importante de votre activité. Pour cela, vous pouvez affecter des périodes d'inventaire spéciales à ces articles.

Vous pouvez effectuer un inventaire tournant de l'une des manières suivantes en fonction de votre configuration entrepôt. Pour plus d'informations, voir [Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md).  

-   Si votre magasin n'utilise pas le prélèvement et rangement suggérés (configuration d'entrepôt de base), vous pouvez utiliser la fenêtre **Feuille inventaire** du menu **Stock** ; la procédure est similaire à celle d'un inventaire sans inventaire tournant.  
-   Si votre magasin utilise le prélèvement et rangement suggérés (configuration d'entrepôt avancée), vous utilisez d'abord la fenêtre **Feuille inventaire entrepôt**, puis vous utilisez la fenêtre **Feuille article** pour exécuter la fonction **Calculer ajustement entrepôt**.  

### <a name="to-set-up-counting-periods"></a>Pour configurer des périodes d'inventaire
Un inventaire est généralement effectué en fonction d'intervalles réguliers (par exemple, tous les mois, tous les trimestres ou toutes les années). Vous pouvez configurer les périodes d'inventaire nécessaires.

Configurez les périodes d'inventaire que vous souhaitez utiliser, puis affectez-en une à chaque article. Lorsque vous effectuez un inventaire et que vous utilisez **Calculer période d'inventaire** de la feuille inventaire, les lignes des articles sont créées automatiquement.

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Périodes inventaire**, puis sélectionnez le lien connexe.  
2. Renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

### <a name="to-assign-a-counting-period-to-an-item"></a>Pour affecter une période d'inventaire à un article  
1. Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Articles**, puis sélectionnez le lien connexe.  
2. Sélectionnez l'article auquel vous souhaitez affecter une période d'inventaire.  
3. Dans le champ **Code période inventaire stock**, sélectionnez la période d'inventaire appropriée.  
4. Cliquez sur le bouton **Oui** pour modifier le code et la calculer la première période d'inventaire de l'article. La prochaine fois que vous choisissez de calculer une période d'inventaire dans la feuille inventaire, l'article s'affichera en tant que ligne dans la fenêtre **Sélection article inventaire**. Vous pouvez ensuite commencer à compter l'article sur une base périodique.

### <a name="to-initiate-a-count-based-on-counting-periods-in-basic-warehouse-configurations"></a>Pour lancer un décompte selon des périodes d'inventaire dans les configurations d'entrepôt de base
1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuille inventaire**, puis sélectionnez le lien connexe.
2. Choisissez l'action **Calculer la période d'inventaire**.

    La fenêtre **Sélection article inventaire** qui s'ouvre affiche les articles auxquels des périodes d'inventaire ont été affectés et qui doivent être comptés en fonction de leurs périodes d'inventaire.
3. Effectuer l'inventaire physique. Pour plus d'informations, voir la section « Pour effectuer un inventaire physique ».

### <a name="to-initiate-a-count-based-on-counting-periods-in-advanced-warehouse-configurations"></a>Pour lancer un décompte selon des périodes d'inventaire dans les configurations d'entrepôt avancées
1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Feuille inventaire entrepôt**, puis sélectionnez le lien connexe.  
2. Choisissez l'action **Calculer la période d'inventaire**.

    La fenêtre **Sélection article inventaire** qui s'ouvre affiche les articles auxquels des périodes d'inventaire ont été affectés et qui doivent être comptés en fonction de leurs périodes d'inventaire.
3. Effectuer l'inventaire physique. Pour plus d'informations, voir la section « Pour effectuer un inventaire physique ».  

    > [!NOTE]  
    >  Vous devez compter l'article dans tous les emplacements contenant cet article. Si vous supprimez certaines des lignes emplacement que le programme a récupérées dans la fenêtre **Inventaire entrepôt** , vous ne compterez pas tous les articles dans l'entrepôt. Si vous validez ultérieurement de tels résultats incomplets sur la feuille inventaire, les montants validés sont incorrects.  

## <a name="to-adjust-the-inventory-of-one-item"></a>Pour ajuster le stock d'un article
Après avoir effectué un inventaire d'un article dans votre module Distribution - Stocks, vous pouvez utiliser la fonction **Ajuster stock** pour enregistrer la quantité réelle en stock.

1. Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Articles**, puis sélectionnez le lien connexe.
2. Sélectionnez l'article pour lequel vous souhaitez ajuster le stock, puis sélectionnez l'action **Ajuster stock**.
3. Dans le champ **Nouveau stock**, entrez la quantité en stock que vous souhaitez enregistrer pour l'article.
4. Cliquez sur le bouton **OK**.

Le stock de l'article est désormais ajusté. La nouvelle quantité s'affiche dans le champ **Stock actuel** de la fenêtre **Ajuster stock** et dans le champ **Stock** de la fenêtre **Fiche article**.

Vous pouvez également utiliser la fonction **Ajuster stock** comme un moyen simple de placer les articles achetés dans le stock si vous n'utilisez pas des factures achat ou des commandes pour enregistrer vos achats. Pour plus d'informations, reportez-vous à [Procédure : enregistrer des achats](purchasing-how-record-purchases.md).

> [!NOTE]  
>   Après avoir ajusté le stock, vous devez le mettre à jour avec la valeur actuelle calculée. Pour plus d'informations, voir [Procédure : réévaluer le stock](inventory-how-revalue-inventory.md).

### <a name="to-adjust-the-inventory-quantity-of-multiple-items-in-basic-warehouse-configurations"></a>Pour ajuster la quantité en stock de plusieurs articles dans les configurations d'entrepôt de base
Dans la fenêtre **feuille article**, vous pouvez valider la transaction article directement pour ajuster le stock en fonction des achats, ventes et d'ajustements positifs et négatifs sans utiliser de documents.

Si vous utilisez fréquemment la feuille article pour comptabiliser des lignes feuille identiques ou analogues (par exemple, des lignes en rapport avec la consommation de matériel), vous pouvez utiliser la fenêtre **Feuille article standard** pour simplifier cette tâche récurrente. Pour plus d'informations, reportez-vous à la section « Feuilles standard » de [Utilisation de feuilles comptabilité](ui-work-general-journals.md).

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuilles article**, puis sélectionnez le lien connexe.
2. Renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Choisissez l'action **Valider** pour créer des ajustements de stock.

> [!NOTE]  
>   Après avoir ajusté le stock, vous devez le mettre à jour avec la valeur actuelle calculée. Pour plus d'informations, voir [Procédure : réévaluer le stock](inventory-how-revalue-inventory.md).

### <a name="to-adjust-bin-quantities-in-advanced-warehouse-configurations"></a>Pour ajuster les quantités de l'emplacement dans les configurations d'entrepôt avancées  
Si votre magasin utilise directement le prélèvement et rangement, vous pouvez utiliser la **feuille article entrepôt** pour valider, hors inventaire, tous les ajustements positifs et négatifs au niveau de la quantité article qui sont des gains réels, tels que les articles déjà validés comme étant manquants et qui réapparaissent subitement, ou des pertes réelles, telles que les bris d'articles fragiles.  

A la différence de la validation des ajustements dans la feuille article stock, l'utilisation de la feuille article entrepôt permet d'obtenir un autre niveau d'ajustement des enregistrements de quantité encore plus précis, à tout moment. Par conséquent, l'entrepôt dispose toujours d'un enregistrement complet indiquant le nombre d'articles disponibles et leur lieu de stockage, mais les enregistrements ajustement ne sont pas immédiatement validés dans l'écriture article. Au cours de l'enregistrement, le programme crédite ou débite l'emplacement de l'ajustement quantité, et crée une écriture de compensation dans l'emplacement ajustement entrepôt (emplacement virtuel sans articles réels). Cet emplacement a été défini dans le **Code emplacement ajustement stock** sur la fiche magasin.

1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Feuille article entrepôt**, puis sélectionnez le lien connexe.  
2.  Renseignez les informations d'ent-ête.  
3.  Renseignez le champ **N° article** de la ligne.  
4.  Saisissez l'emplacement dans lequel vous placez les articles supplémentaires ou dans lequel des articles sont manquants.  
5.  Saisissez la différence de quantité dans le champ **Quantité**. Si vous avez trouvé des articles supplémentaires, saisissez une quantité positive. Si des articles sont manquants, saisissez une quantité négative.  
6.  Sélectionnez l'action **Enregistrer**.

## <a name="to-synchronize-the-adjusted-warehouse-entries-with-the-related-item-ledger-entries"></a>Pour synchroniser les écritures entrepôt ajustées avec les écritures comptables article associées
Suivant des intervalles définis par la politique de la société, vous devez valider les enregistrements des emplacements ajustement entrepôt dans l'écriture article. Certaines sociétés choisissent de valider quotidiennement les ajustements dans l'écriture article, alors que d'autres préfèrent effectuer une simulation de manière moins fréquente.

1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Feuille article**, puis sélectionnez le lien connexe.  
2.  Renseignez les champs de chaque ligne feuille.  
3.  Sélectionnez l'action **Calculer ajustement entrepôt** et renseignez les filtres selon vos besoins dans la fenêtre de demande de traitement par lots. Les ajustements sont calculés uniquement pour les écritures de l'emplacement ajustement qui répondent aux exigences des filtres.  
4.  Sur le raccourci **Options**, entrez manuellement un numéro dans le champ **N° document**. Étant donné qu'aucune souche de numéros n'a été configurée pour ce traitement par lots, utilisez le modèle de numéros configuré par l'entrepôt ou saisissez la date suivie de vos initiales.  
5.  Cliquez sur le bouton **OK**. Les ajustements positifs et négatifs sont totalisés pour chaque article et les lignes sont créées dans la feuille article pour les articles pour lesquels la somme est une quantité positive ou négative.  
6.  Validez des lignes feuille pour entrer les différences de quantité dans la feuille article. Le stock des emplacements entrepôt correspond maintenant précisément à celui de l'écriture article.  

## <a name="to-reclassify-an-items-lot-number"></a>Pour reclasser le numéro de lot d'un article
1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuilles reclassement article**, puis sélectionnez le lien connexe.
2. Dans la fenêtre **Feuilles reclassement article**, renseignez les champs selon vos besoins.
3. Dans le champ **N° lot**, saisissez le numéro de lot actuel de l'article.
4. Dans le champ **Nouveau N° lot**, saisissez le nouveau numéro de lot de l'article.
5. Sélectionnez l'action **Valider**.

Des étapes spéciales s'appliquent lorsque vous souhaitez reclasser les numéros de série ou de lot. Pour plus d'informations, voir [Procédure : utiliser les numéros de lot et de série](inventory-how-work-item-tracking.md).

## <a name="see-also"></a>Voir aussi
[Stock](inventory-manage-inventory.md)
[Gestion d'entrepôt](warehouse-manage-warehouse.md)    
[Ventes](sales-manage-sales.md)  
[Achats](purchasing-manage-purchasing.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

