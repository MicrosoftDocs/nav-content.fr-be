---
title: Comment imprimer un avis de remise
description: "Vous pouvez aider vos fournisseurs à effectuer des rapprochements en imprimant des avis de remise avant d'afficher une feuille de paiement et après avoir validé un règlement."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/26/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 71c84b4a7bad83e6008c0fa34f908e133b014a59
ms.contentlocale: fr-be
ms.lasthandoff: 10/26/2017

---

#<a name="how-to-print-remittance-advice"></a>Procédure : imprimer un avis de remise
Vous pouvez imprimer l'avis de remise avant de valider une feuille paiements et après avoir validé un paiement. Cette option affiche les numéros de facture fournisseur, ce qui permet aux fournisseurs d'effectuer les rapprochements.

##<a name="to-print-remittance-advice"></a>Pour imprimer un avis de remise
1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuilles paiement**, puis sélectionnez le lien connexe.  
2. Dans la fenêtre **Feuille paiement**, sélectionnez le paiement pour lequel l'avis de remise doit être imprimé.  
3. Choisissez l'action **Imprimer l'avis de remise**.  
4. Dans le traitement par lots **Avis de remise - Feuille**, sous le raccourci **Ligne feuille comptabilité**, sélectionnez les filtres appropriés.  
  
    >[!Note]
    > Vous pouvez appliquer un filtre en utilisant le numéro de document externe provenant du fournisseur pour refléter les paiements avec les factures.

5. Sur le raccourci **Fournisseur**, choisissez les filtres appropriés.  
6. Choisissez **Imprimer** pour imprimer l'état, ou choisissez **Aperçu** pour l'afficher maintenant.  

## <a name="using-remittance-advice-reports"></a>Utilisation des états d'avis de remise
Le tableau suivant décrit les états que vous pouvez utiliser avec la notification de remise :

|État|Désignation|
|----|----|
|Avis de remise - État Journal|Cet état indique les documents qui sont inclus dans le paiement. Pour les lignes feuille comptabilité, vous pouvez spécifier le modèle et la feuille dont les avis de remise sont imprimés, la date de la première activité d'impression, et filtrer sur un numéro de document. Pour les fournisseurs, vous pouvez saisir les numéros de fournisseur à inclure dans l'état. |
|Avis de remise - État Écritures| Cet état indique les documents qui sont inclus dans le paiement. Définissez le contenu de l'état en paramétrant des filtres. Vous pouvez définir des champs supplémentaires sous l'onglet en cliquant sur le champ **Champ**. Pour les écritures fournisseur, vous pouvez spécifier les fournisseurs à inclure dans l'état, la date de la première activité d'impression, la devise et le numéro d'écriture à inclure. |

> [!Note]
> Avis de remise - État Journal ne prend pas en charge les scénarios d'application de devises croisées ou les écarts de règlement. Pour en savoir plus, voir [Procédure : activer le lettrage d'écritures comptables client en devises différentes](finance-how-enable-application-ledger-entries-different-currencies.md).

> [!Tip]
> Pour plus d'informations sur l'utilisation des états, consultez [Affichage d'états de test avant la validation](ui-how-view-test-reports-posting.md), [Utiliser des états dans](ui-work-report.md) et [Recherche, filtrage et tri de données](ui-enter-criteria-filters.md).

##<a name="see-also"></a>Voir aussi  
[Bienvenue dans Dynamics NAV](across-get-started.md)
