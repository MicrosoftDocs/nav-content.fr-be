---
title: Gestion des comptes client
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 3f2be627dfda9720e9f31fd227164d1c27116d2c
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="manage-receivables"></a>Gestion des comptes client#
Une tâche centrale de la gestion des comptes client consiste à lettrer les paiements entrants à leurs écritures comptables client ou fournisseur associées et de ce fait clôturer les factures vente ou les avoirs achat associés comme payés. Lorsque tous les paiements sont lettrés, vous pouvez rapprocher le compte bancaire.  

Vous pouvez effectuer cette tâche dans la fenêtre **Feuille rapprochement bancaire** en important un fichier ou un flux de relevé bancaire pour enregistrer rapidement les paiements dans Dynamics NAV. Une fonction de lettrage automatique lettre les paiements à leurs écritures comptables client ou fournisseur ouvertes associées en fonction des correspondances de données entre le texte de paiement et les informations d'écriture. Vous pouvez réviser et modifier les lettrages automatiques avant de valider la feuille. Vous pouvez choisir de clôturer les écritures comptables compte bancaire ouvertes associées aux écritures comptables lettrées lorsque vous validez la feuille. Cela signifie que le compte bancaire est automatiquement rapproché lorsque tous les paiements sont lettrés.

**Remarque** : vous pouvez rapprocher des comptes bancaires en tant que tâche distincte dans la fenêtre **Rapprochement bancaire**, qui prend également en charge les écritures comptables chèque. Pour plus d'informations, reportez vous à [Procédure : rapprocher des comptes bancaires séparément](bank-how-reconcile-bank-accounts-separately.md).

Sinon, vous pouvez lettrer les paiements dans la fenêtre **Enregistrement de paiement** en vérifiant manuellement les paiements reçus en liquide, par chèque ou par transaction bancaire par rapport à une liste générée de documents vente échus. Notez que cette fonctionnalité est uniquement disponible pour les documents vente.

Autre méthode de rapprochement manuel des paiements : vous pouvez valider chaque réception à un compte général, client ou autre en saisissant une ligne règlement dans la fenêtre **Feuille règlement**. Dans ce cas, vous pouvez soit lettrer la réception ou le remboursement à une ou plusieurs écritures ouvertes avant de valider la feuille règlement, ou vous pouvez lettrer les écritures comptables client créées.

Une autre tâche de gestion des comptes client consiste à collecter des soldes restants, notamment pour gérer les intérêts de retard et l'émission de relances.

Le tableau suivant décrit une série de tâches et inclut des liens vers les rubriques qui les décrivent.

|Pour |Voir |
|---|----|
|Lettrer des paiements aux écritures comptables client ou fournisseur ouvertes sur la base d'un fichier ou flux de relevé bancaire importé, et rapprocher le compte bancaire lorsque tous les paiements sont lettrés.|[Procédure : lettrage automatique des paiements et rapprochement des comptes bancaires](receivables-apply-payments-auto-reconcile-bank-accounts.md)|
|Lettrer les paiements aux écritures comptables client ouvertes selon la saisie manuelle dans la liste des documents vente échus. | [Procédure : rapprocher les paiements client manuellement à partir de la liste des documents vente échus](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md)|
|Valider les règlements ou les remboursements pour les clients dans la feuille règlement et lettrer aux écritures comptables client, à partir de la feuille ou des écritures comptables validées. | [Procédure : rapprocher les paiements client manuellement](receivables-how-apply-sales-transactions-manually.md) |
|Rappeler aux clients les soldes échus, calculer les intérêts et les intérêts de retard, et gérer les comptes clients. | [Procédure : collecter des soldes restants](receivables-collect-outstanding-balances.md) |

## <a name="see-also"></a>Voir aussi
[Gestion des ventes](sales-manage-sales.md)  
[Gestion des comptes fournisseur](payables-manage-payables.md)  
[Utiliser Dynamics NAV](ui-work-product.md)  
[Fonctionnalités communes aux différents secteurs d'activité](ui-across-business-areas.md)

