---
title: "Clôturer les périodes"
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: ac1ed2d1dcf8bf780bda91fbf0a04e5c5e8d106a
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---
# <a name="close-periods"></a>Clôturer les périodes
L'application ne vous oblige pas à clôturer les périodes. Toutefois, il existe de nombreuses activités de clôture de période (fin de mois) que vous pouvez effectuer dans le cadre de l'application si vous le souhaitez. Cette rubrique présente un aperçu de ces processus et activités, qui peuvent ou non être nécessaires pour votre société.

## <a name="general-ledger"></a>Écritures comptables
* Spécifiez des plages de date de validation à l'échelle du système et spécifiques à l'utilisateur.

    Cela spécifie les dates entre lesquelles les validation sont autorisées. En fonction des besoins de votre activité, vous pouvez restreindre les plages de date validation utilisateur au début du processus de clôture d'exercice ou à une date ultérieure vers la fin de l'exercice. Pour plus d'informations, reportez vous à [Procédure: spécifier des périodes de validation](finance-setup-how-specify-posting-periods.md).
* Effectuez tous les ajustements comptables nécessaires.
* Mettez à jour et validez les feuilles abonnement.
<!--* Process Consolidations-->
* Exécutez les tableaux d'analyse comme suit :
  1. Ouvrez la fenêtre **Tableau d'analyse**, puis sélectionnez l'action **Imprimer**.
  2. Renseignez le formulaire de sélection **Tableau d'analyse**, puis sélectionnez l'action **Imprimer**.

## <a name="sales--receivables"></a>Ventes
* Validez l'ensemble des commandes, factures, avoirs et retours vente.
* Validez l'ensemble des feuilles règlement.
* Mettez à jour et validez les feuilles abonnement associées aux ventes.
* Rapprochez la comptabilité client de la comptabilité.
* Exécutez le traitement par lots **Supprimer cdes vente facturées**.

## <a name="purchases--payables"></a>Achats
* Validez l'ensemble des commandes, factures, avoirs et retours achat.
* Validez l'ensemble des feuilles paiement.
* Mettez à jour et validez les feuilles abonnement associées aux achats.
* Générez l'état **Comptabilité fournisseur âgée** et rapprochez la comptabilité fournisseur de la comptabilité.
* Exécutez le traitement par lots **Supprimer cdes achat facturées**.

<!-- ### Fixed Assets
* Post all maintenance costs have been posted through the fixed asset journals or invoices.
* Post adjustments.
* Post appreciation.
* Post depreciation.
* Update and post the recurring fixed asset journal.-->

<!--### Intercompany
* Process Intercompany Postings.-->

## <a name="calculate-and-process-sales-tax"></a>Calculez et traitez la Sales Tax.
*  Renseignez les déclarations de TVA.

## <a name="see-also"></a>Voir aussi
[Clôture des exercices et des périodes](year-close-years-periods.md)  
[Clôture des livres](year-close-books.md)

