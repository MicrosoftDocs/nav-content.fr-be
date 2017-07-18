---
title: Gestion des comptes fournisseur
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
ms.openlocfilehash: 50a68e1eaf0d6057420635f85b473639e39caa5a
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="manage-payables"></a>Gestion des comptes fournisseur
Une tâche centrale de la gestion des comptes fournisseurs est de payer de vos fournisseurs. Vous pouvez utiliser les fonctions permettant de renseigner automatiquement la fenêtre **Feuille paiement** avec des lignes de paiement pour les factures achat échues. Pour effectuer rapidement les transactions bancaires nécessaires, vous pouvez exporter plusieurs lignes feuille paiement vers un fichier, que vous téléchargez ensuite vers votre banque pour traitement. Vous pouvez également effectuer des paiements par chèque, notamment pour transmettre des chèques en tant que paiements électroniques.

Une autre tâche courante consiste à lettrer les paiements sortants à leurs écritures comptables fournisseur associées et de ce fait clôturer les factures achat ou les avoirs achat associés comme payés. Vous pouvez effectuer cette tâche dans la fenêtre **Feuille rapprochement bancaire** en important un fichier de relevé bancaire pour enregistrer rapidement les paiements dans Dynamics NAV. Une fonction automatique de l'application lettre les paiements à leurs écritures comptables fournisseur ouvertes ou à leurs écritures comptables client associées en fonction des correspondances de données entre le texte de paiement et les informations d'écriture. Vous pouvez utiliser plusieurs fonctionnalités pour réviser et modifier les lettrages automatiques avant de valider la feuille. Vous pouvez choisir de clôturer les écritures comptables compte bancaire ouvertes associées aux écritures comptables lettrées lorsque vous validez la feuille. Cela signifie que le compte bancaire est automatiquement rapproché lorsque tous les paiements sont lettrés.

Sinon, vous pouvez lettrer les paiements sortants manuellement dans la fenêtre **Feuille paiement** ou à partir des écritures comptables fournisseur associées.

Le tableau suivant décrit une série de tâches associées aux comptes fournisseur et inclut des liens vers les rubriques qui les décrivent.

|Pour |Voir |
|---|----|
|Générer des paiements fournisseur échus classés par ordre de priorité en fonction des escomptes et des pénalités de retard. Éventuellement, exporter les paiements vers un fichier bancaire lors de la validation.|[Exécuter des paiements](payables-make-payments.md)|
|Lettrer les paiements fournisseur automatiquement aux factures achat impayées en important un fichier de relevé bancaire.|[Procédure : lettrage automatique des paiements et rapprochement des comptes bancaires](receivables-apply-payments-auto-reconcile-bank-accounts.md)|
|Lettrer les paiements fournisseur aux factures achat impayées manuellement.|[Procédure : lettrer les paiements fournisseur manuellement](payables-how-apply-purchase-transactions-manually.md)|

## <a name="see-also"></a>Voir aussi
[Gestion des achats](purchasing-manage-purchasing.md)  
[Gestion des comptes client](receivables-manage-receivables.md)  
[Utiliser Dynamics NAV](ui-work-product.md)  
[Fonctionnalités communes aux différents secteurs d'activité](ui-across-business-areas.md)

