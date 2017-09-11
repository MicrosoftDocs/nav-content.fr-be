---
title: "Gérer les comptes bancaires"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: d97c3afba0e899768bda1b637c4f288db210d38c
ms.contentlocale: fr-be
ms.lasthandoff: 07/19/2017

---

# <a name="manage-bank-accounts"></a><span data-ttu-id="dbf8c-102">Gérer les comptes bancaires</span><span class="sxs-lookup"><span data-stu-id="dbf8c-102">Manage Bank Accounts</span></span>
<span data-ttu-id="dbf8c-103">Vous devez rapprocher régulièrement vos écritures comptables bancaires dans Dynamics NAV avec les transactions bancaires associées dans les comptes bancaires de votre banque, puis valider le solde sur votre compte bancaire.</span><span class="sxs-lookup"><span data-stu-id="dbf8c-103">At regular intervals, you must reconcile your bank ledger entries in Dynamics NAV with the related bank transactions in bank accounts at your bank, and then post the balance to your bank account.</span></span> <span data-ttu-id="dbf8c-104">Vous pouvez effectuer cette tâche soit dans le cadre du traitement des paiements représentés sur un relevé bancaire dans la **Feuille rapprochement bancaire**.</span><span class="sxs-lookup"><span data-stu-id="dbf8c-104">You can perform this task either as part of processing the payments represented on a bank statement in the **Payment Reconciliation Journal**.</span></span> <span data-ttu-id="dbf8c-105">Sinon, vous pouvez effectuer la tâche séparément du traitement des paiements, dans la fenêtre **Rapprochement bancaire**, qui prend en charge des écritures comptables chèque.</span><span class="sxs-lookup"><span data-stu-id="dbf8c-105">Alternatively, you can perform the task separately from payment processing, in the **Bank Acc. Reconciliation** window, which supports check ledger entries.</span></span> <span data-ttu-id="dbf8c-106">Dans les deux cas, vous renseignez les fenêtres en important le relevé bancaire dans Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="dbf8c-106">In both cases, you fill the windows by importing the bank statement into Dynamics NAV.</span></span>

<span data-ttu-id="dbf8c-107">Parfois, vous devez transférer les montants entre comptes bancaires dans Dynamics NAV pour refléter les transferts effectués au niveau de votre banque.</span><span class="sxs-lookup"><span data-stu-id="dbf8c-107">Sometimes, you need to transfer amounts between bank account in Dynamics NAV to reflect transfers at your bank.</span></span> <span data-ttu-id="dbf8c-108">Vous effectuez cette tâche dans la fenêtre **Feuille comptabilité**, de différentes manières en fonction de la devise des fonds.</span><span class="sxs-lookup"><span data-stu-id="dbf8c-108">You perform this task in the **General Journal** window, in different ways depending on the currency of the funds.</span></span>

<span data-ttu-id="dbf8c-109">Avant de pouvoir gérer des comptes bancaires, vous devez configurer chaque compte bancaire en tant que fiche compte bancaire.</span><span class="sxs-lookup"><span data-stu-id="dbf8c-109">Before you can manage bank accounts, you must set each bank account up as a bank account card.</span></span> <span data-ttu-id="dbf8c-110">En outre, vous devez configurer les services électroniques que vous pouvez utiliser pour l'importation de relevés bancaires et l'exportation de fichiers de paiement.</span><span class="sxs-lookup"><span data-stu-id="dbf8c-110">In addition, you must set up electronic services that you may use for bank statement import and payment file export.</span></span> <span data-ttu-id="dbf8c-111">Pour plus d'informations, reportez vous à [Configuration de comptes bancaires](bank-setup-banking.md).</span><span class="sxs-lookup"><span data-stu-id="dbf8c-111">For more information, see [Set Up Bank Accounts](bank-setup-banking.md).</span></span>

<span data-ttu-id="dbf8c-112">Le tableau suivant décrit une série de tâches et inclut des liens vers les rubriques qui les décrivent.</span><span class="sxs-lookup"><span data-stu-id="dbf8c-112">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="dbf8c-113">Pour</span><span class="sxs-lookup"><span data-stu-id="dbf8c-113">To</span></span> |<span data-ttu-id="dbf8c-114">Voir</span><span class="sxs-lookup"><span data-stu-id="dbf8c-114">See</span></span> |
|---|----|
|<span data-ttu-id="dbf8c-115">Rapprocher des comptes bancaires en relation avec le traitement des paiements dans la fenêtre **Feuille rapprochement bancaire**.</span><span class="sxs-lookup"><span data-stu-id="dbf8c-115">Reconcile bank accounts in connection with payment processing in the **Payment Reconciliation Journal** window.</span></span>|[<span data-ttu-id="dbf8c-116">Procédure : lettrage automatique des paiements et rapprochement des comptes bancaires</span><span class="sxs-lookup"><span data-stu-id="dbf8c-116">Apply Payments Automatically and Reconcile Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md)|
|<span data-ttu-id="dbf8c-117">Rapprocher des comptes bancaires, y compris les écritures comptables chèque, en tant que tâche distincte dans la fenêtre **Rapprochement bancaire**.</span><span class="sxs-lookup"><span data-stu-id="dbf8c-117">Reconcile bank accounts, including check ledger entries, as a separate task in the **Bank Acc. Reconciliation** window.</span></span>|[<span data-ttu-id="dbf8c-118">Procédure : rapprocher des comptes bancaires séparément</span><span class="sxs-lookup"><span data-stu-id="dbf8c-118">How to: Reconcile Bank Accounts Separately</span></span>](bank-how-reconcile-bank-accounts-separately.md)|
|<span data-ttu-id="dbf8c-119">Valider des transferts entre comptes bancaires dans la même devise ou dans des devises différentes.</span><span class="sxs-lookup"><span data-stu-id="dbf8c-119">Post transfers between bank accounts in the same currency or in different currencies.</span></span>|[<span data-ttu-id="dbf8c-120">Procédure : Transfert de fonds à la banque</span><span class="sxs-lookup"><span data-stu-id="dbf8c-120">How to: Transfer Bank Funds</span></span>](bank-how-transfer-bank-funds.md)
## <a name="see-also"></a><span data-ttu-id="dbf8c-121">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="dbf8c-121">See Also</span></span>  
[<span data-ttu-id="dbf8c-122">Configuration des opérations bancaires</span><span class="sxs-lookup"><span data-stu-id="dbf8c-122">Set Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="dbf8c-123">Gestion des comptes client</span><span class="sxs-lookup"><span data-stu-id="dbf8c-123">Manage Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="dbf8c-124">[Gestion des comptes fournisseur](payables-manage-payables.md)  </span><span class="sxs-lookup"><span data-stu-id="dbf8c-124">[Manage Payables](payables-manage-payables.md)  </span></span>  
[<span data-ttu-id="dbf8c-125">Utiliser Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="dbf8c-125">Work With Dynamics NAV</span></span>](ui-work-product.md)  
[<span data-ttu-id="dbf8c-126">Fonctionnalités communes aux différents secteurs d'activité</span><span class="sxs-lookup"><span data-stu-id="dbf8c-126">Across Business Areas</span></span>](ui-across-business-areas.md)

