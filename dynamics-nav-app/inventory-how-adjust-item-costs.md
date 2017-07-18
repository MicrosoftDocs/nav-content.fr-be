---
title: "Procédure : ajustement des coûts article"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 59db38c159dd2810656edc668ee431c6414b9d90
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-adjust-item-costs"></a>Procédure : ajustement des coûts article   
Le coût d'un article (valeur du stock) que vous achetez et vendez ultérieurement peut changer au cours de sa durée de vie, par exemple parce que des frais de transport sont ajoutés à son coût d'achat après que vous ayez vendu l'article. Pour toujours connaître la valeur du stock correcte, les coûts article doivent donc être ajustés régulièrement.
Cela garantit que les statistiques vente et profit sont à jour et que les indicateurs clés financiers sont corrects.

**Remarque** : Le coût des articles est ajusté uniquement selon la méthode d'évaluation du stock FIFO. Cela signifie que le coût unitaire d'un article est la valeur réelle de toute réception de l'article, et que le stock est évalué en supposant que les premiers articles stockés sont ceux vendus en premier.

La fonction d'ajustement des coûts traite uniquement les écritures valeur non encore ajustées. Si la fonction est confrontée à une situation où des coûts entrants modifiés doivent être transférés à des écritures sortantes associées, de nouvelles écritures valeur ajustées sont créées, sur la base des informations des écritures valeur d'origine, mais contenant le montant de l'ajustement. La fonction d'ajustement des coûts utilise la date comptabilisation de l'écriture valeur d'origine dans l'écriture ajustée, sauf si la date est comprise dans une période inventaire clôturée. Dans ce cas, le programme utilise la date début de la période d'inventaire ouverte suivante. Si aucune période inventaire n'est utilisée, la date du champ **Début période validation** de la fenêtre **Paramètres comptabilité** définira la date de comptabilisation de l'écriture ajustée.

**Remarque** : une fois les coûts article ajustés, les coûts ajustés doivent être validés dans la comptabilité, manuellement ou automatiquement. Pour plus d'informations, reportez-vous à [Procédure : valider les coûts ajustés dans la comptabilité](inventory-how-post-inventory-cost-gl.md).

Vous pouvez ajuster les coûts article de deux manières :
 - Automatiquement, en faisant en sorte que le système ajuste toute modification des coûts chaque fois que des mouvements de stock se produisent.
 - Manuellement, en exécutant le traitement par lots **Ajuster coûts : Écr. article** pour un ou plusieurs articles lorsque vous savez que leurs coûts ont changé.  

## <a name="to-adjust-item-costs-automatically"></a>Pour ajuster les coûts article automatiquement
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Paramètres stock**, puis sélectionnez le lien connexe.
2. Dans la fenêtre **Paramètres stock**, dans le champ **Ajustement automatique des coûts**, sélectionnez l'une des valeurs suivantes.

|Option |Comportement |
|-------|---------|
|Jamais|Les coûts ne sont jamais ajustés lors de la validation|
|Jour|Les coûts sont ajustés si la validation a lieu dans la journée commençant à la date de travail|
|Semaine|Les coûts sont ajustés si la validation a lieu dans la semaine commençant à la date de travail|
|Mois|Les coûts sont ajustés si la validation a lieu dans le mois commençant à la date de travail|
|Trimestre|Les coûts sont ajustés si la validation a lieu dans le trimestre commençant à la date de travail|
|Année|Les coûts sont ajustés si la validation a lieu dans l'année commençant à la date de travail|
|Toujours|Les coûts sont systématiquement ajustés en cas de validation, quelle que soit la date de comptabilisation|

## <a name="to-adjust-item-costs-manually"></a>Pour ajuster les coûts article manuellement
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Ajuster coûts : Écr. article**, puis sélectionnez le lien connexe.
2. Dans **Ajuster coûts : Écr. article** fenêtre, spécifiez les articles pour lesquels ajuster les coûts ajustement et si les coûts ajustés doivent être validés dans la comptabilité en même temps.

## <a name="see-also"></a>Voir aussi
[Gestion du stock](inventory-manage-inventory.md)  
[Procédure : valider les coûts ajustés dans la comptabilité](inventory-how-post-inventory-cost-gl.md)  
[Gestion des ventes](sales-manage-sales.md)  
[Gestion des achats](purchasing-manage-purchasing.md)

