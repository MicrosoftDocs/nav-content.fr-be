---
title: "Procédure : gérer les budgets pour les immobilisations"
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
ms.openlocfilehash: 47b5e0abcae4fab92da5dd9c1bda350a37ec0358
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-manage-budgets-for-fixed-assets"></a>Procédure : gérer les budgets pour les immobilisations
Vous pouvez paramétrer des immobilisations budgétées. Cela permet d'inclure dans des états des acquisitions et des ventes anticipées.  

 Pour préparer le compte de gestion budgété, le compte de bilan budgété et le budget de trésorerie, vous avez besoin d'informations sur les investissements, les cessions et les amortissements futurs des immobilisations. Vous pouvez obtenir ces informations dans l'état **Immo. - Valeur projetée**. Avant d'imprimer cet état, vous devez préparer le budget.  

## <a name="to-budget-the-acquisition-cost-of-a-fixed-asset"></a>Pour budgéter le coût d'acquisition d'une immobilisation
Pour préparer un budget, vous devez définir des fiches immobilisation pour les immobilisations que vous souhaitez acheter. Les immobilisations du budget sont configurées comme immobilisations ordinaires, mais elles doivent être configurées pour ne pas être validées en comptabilité.

Lorsque vous validez le coût d'acquisition, vous saisissez le numéro de l'immobilisation budgétée dans le champ **N° immo. budgétée** . Cela permet de valider un coût d'acquisition avec un signe opposé pour l'immobilisation budgétée. Le coût d'acquisition total de l'immobilisation budgétée est donc la différence entre le coût d'acquisition budgété et le coût réel.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Immobilisations**, puis sélectionnez le lien connexe.
2. Sélectionnez l'action **Nouveau** pour créer une fiche immobilisation pour l'immobilisation budgétée.
3. Cochez la case **Actif budgété** pour empêcher la validation en comptabilité.
4. Complétez les champs restants, attribuez une loi d'amortissement, puis validez le premier coût d'acquisition avec l'immobilisation budgétée saisie dans le champ **N° immo. budgétée** de la ligne feuille. Pour en savoir plus, voir [Procédure : acquérir les immobilisations](fa-how-acquire.md).

## <a name="to-budget-the-disposal-of-a-fixed-asset"></a>Pour budgéter la cession d'une immobilisation
Si vous prévoyez de vendre des immobilisations dans la période correspondant au budget, vous pouvez indiquer des informations concernant le prix et la date de vente.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Immobilisations**, puis sélectionnez le lien connexe.
2. Sélectionnez l'immobilisation à céder, puis sélectionnez l'action **Lois d'amortissement**.
3. Dans la fenêtre **Lois d'amortissement immo.**, complétez les champs **Date cession prévue** et **Produit de cession prévu**. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.

## <a name="to-view-projected-disposal-values"></a>Pour visualiser des valeurs de cession prévues
Pour visualiser les valeurs de cession prévues et effectuer le calcul des gains et des pertes, vous pouvez utiliser l'état **Immo. - Valeur projetée**.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Immo. - Valeur projetée**, puis sélectionnez le lien connexe.
2. Renseignez les champs selon vos besoins.
3. Cliquez sur le bouton **Imprimer** ou **Aperçu**.

## <a name="to-budget-depreciation"></a>Pour budgéter des amortissements
Vous pouvez utiliser l'état **Immo. - Valeur projetée** pour calculer l'amortissement à venir. L'état affiche la valeur comptable et l'amortissement cumulé au début et à la fin de la période sélectionnée, ainsi que les modifications apportées durant cette période.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Immo. - Valeur projetée**, puis sélectionnez le lien connexe.
2. Renseignez les champs selon vos besoins.
3. Pour voir les valeurs totales de tous les actifs, décochez la case **Imprimer par immobilisation**.
4. Ne renseignez pas le raccourci **Immobilisation** pour inclure toutes les immobilisations. Dans le champ **Immo. budgétée**, vous pouvez saisir **Non** afin d'exclure les immobilisations budgétées ou sur **Oui** pour les visualiser.
5. Cliquez sur le bouton **Imprimer** ou **Aperçu**.

## <a name="see-also"></a>Voir aussi
[Gérer des immobilisations](fa-manage.md)  
[Configurer des immobilisations](fa-setup.md)  
[Finance](finance-setup.md)  
[Bienvenue dans Dynamics NAV](across-get-started.md)

