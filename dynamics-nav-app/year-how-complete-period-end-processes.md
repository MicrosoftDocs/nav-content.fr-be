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
# <a name="close-periods"></a><span data-ttu-id="bf42e-102">Clôturer les périodes</span><span class="sxs-lookup"><span data-stu-id="bf42e-102">Close Periods</span></span>
<span data-ttu-id="bf42e-103">L'application ne vous oblige pas à clôturer les périodes. Toutefois, il existe de nombreuses activités de clôture de période (fin de mois) que vous pouvez effectuer dans le cadre de l'application si vous le souhaitez.</span><span class="sxs-lookup"><span data-stu-id="bf42e-103">The application does not force you to close periods, however, there are many period-end (month-end) activities that can be performed in the application if you want.</span></span> <span data-ttu-id="bf42e-104">Cette rubrique présente un aperçu de ces processus et activités, qui peuvent ou non être nécessaires pour votre société.</span><span class="sxs-lookup"><span data-stu-id="bf42e-104">This topic provides an overview of these processes and activities, which may or may not be necessary for your company.</span></span>

## <a name="general-ledger"></a><span data-ttu-id="bf42e-105">Écritures comptables</span><span class="sxs-lookup"><span data-stu-id="bf42e-105">General Ledger</span></span>
* <span data-ttu-id="bf42e-106">Spécifiez des plages de date de validation à l'échelle du système et spécifiques à l'utilisateur.</span><span class="sxs-lookup"><span data-stu-id="bf42e-106">Specify system-wide and user-specific posting period.</span></span>

    <span data-ttu-id="bf42e-107">Cela spécifie les dates entre lesquelles les validation sont autorisées.</span><span class="sxs-lookup"><span data-stu-id="bf42e-107">This specifies the dates between which postings are allowed.</span></span> <span data-ttu-id="bf42e-108">En fonction des besoins de votre activité, vous pouvez restreindre les plages de date validation utilisateur au début du processus de clôture d'exercice ou à une date ultérieure vers la fin de l'exercice.</span><span class="sxs-lookup"><span data-stu-id="bf42e-108">Depending on your business needs, you may want to restrict user posting date ranges at the start of the period-end process or at later time towards the end of the period.</span></span> <span data-ttu-id="bf42e-109">Pour plus d'informations, reportez vous à [Procédure: spécifier des périodes de validation](finance-setup-how-specify-posting-periods.md).</span><span class="sxs-lookup"><span data-stu-id="bf42e-109">For more information, see [How to: Specify Posting Periods](finance-setup-how-specify-posting-periods.md).</span></span>
* <span data-ttu-id="bf42e-110">Effectuez tous les ajustements comptables nécessaires.</span><span class="sxs-lookup"><span data-stu-id="bf42e-110">Make all necessary G/L adjustments.</span></span>
* <span data-ttu-id="bf42e-111">Mettez à jour et validez les feuilles abonnement.</span><span class="sxs-lookup"><span data-stu-id="bf42e-111">Update and post Recurring Journals.</span></span>
<!--* Process Consolidations-->
* <span data-ttu-id="bf42e-112">Exécutez les tableaux d'analyse comme suit :</span><span class="sxs-lookup"><span data-stu-id="bf42e-112">Run account schedules as follows:</span></span>
  1. <span data-ttu-id="bf42e-113">Ouvrez la fenêtre **Tableau d'analyse**, puis sélectionnez l'action **Imprimer**.</span><span class="sxs-lookup"><span data-stu-id="bf42e-113">Open the **Account Schedule** window, and choose the **Print** action.</span></span>
  2. <span data-ttu-id="bf42e-114">Renseignez le formulaire de sélection **Tableau d'analyse**, puis sélectionnez l'action **Imprimer**.</span><span class="sxs-lookup"><span data-stu-id="bf42e-114">Fill the **Account Schedule** request window and choose the **Print** action.</span></span>

## <a name="sales--receivables"></a><span data-ttu-id="bf42e-115">Ventes</span><span class="sxs-lookup"><span data-stu-id="bf42e-115">Sales & Receivables</span></span>
* <span data-ttu-id="bf42e-116">Validez l'ensemble des commandes, factures, avoirs et retours vente.</span><span class="sxs-lookup"><span data-stu-id="bf42e-116">Post all sales orders, invoices, credit memos, and return orders.</span></span>
* <span data-ttu-id="bf42e-117">Validez l'ensemble des feuilles règlement.</span><span class="sxs-lookup"><span data-stu-id="bf42e-117">Post all cash receipt journals.</span></span>
* <span data-ttu-id="bf42e-118">Mettez à jour et validez les feuilles abonnement associées aux ventes.</span><span class="sxs-lookup"><span data-stu-id="bf42e-118">Update and post recurring journals that are related to Sales & Receivables.</span></span>
* <span data-ttu-id="bf42e-119">Rapprochez la comptabilité client de la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="bf42e-119">Reconcile accounts receivable to the general ledger.</span></span>
* <span data-ttu-id="bf42e-120">Exécutez le traitement par lots **Supprimer cdes vente facturées**.</span><span class="sxs-lookup"><span data-stu-id="bf42e-120">Run the **Delete Invoiced Sales Orders** batch job.</span></span>

## <a name="purchases--payables"></a><span data-ttu-id="bf42e-121">Achats</span><span class="sxs-lookup"><span data-stu-id="bf42e-121">Purchases & Payables</span></span>
* <span data-ttu-id="bf42e-122">Validez l'ensemble des commandes, factures, avoirs et retours achat.</span><span class="sxs-lookup"><span data-stu-id="bf42e-122">Post all purchase orders, invoices, credit memos, and return orders.</span></span>
* <span data-ttu-id="bf42e-123">Validez l'ensemble des feuilles paiement.</span><span class="sxs-lookup"><span data-stu-id="bf42e-123">Post all payment journals.</span></span>
* <span data-ttu-id="bf42e-124">Mettez à jour et validez les feuilles abonnement associées aux achats.</span><span class="sxs-lookup"><span data-stu-id="bf42e-124">Update and post recurring journals that are related to purchases & payables.</span></span>
* <span data-ttu-id="bf42e-125">Générez l'état **Comptabilité fournisseur âgée** et rapprochez la comptabilité fournisseur de la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="bf42e-125">Run the **Aged Accounts Payable** report and reconcile accounts payable to the general ledger.</span></span>
* <span data-ttu-id="bf42e-126">Exécutez le traitement par lots **Supprimer cdes achat facturées**.</span><span class="sxs-lookup"><span data-stu-id="bf42e-126">Run the **Delete Invoiced Purchase Orders** batch job.</span></span>

<!-- ### Fixed Assets
* Post all maintenance costs have been posted through the fixed asset journals or invoices.
* Post adjustments.
* Post appreciation.
* Post depreciation.
* Update and post the recurring fixed asset journal.-->

<!--### Intercompany
* Process Intercompany Postings.-->

## <a name="calculate-and-process-sales-tax"></a><span data-ttu-id="bf42e-127">Calculez et traitez la Sales Tax.</span><span class="sxs-lookup"><span data-stu-id="bf42e-127">Calculate and Process Sales Tax</span></span>
*  <span data-ttu-id="bf42e-128">Renseignez les déclarations de TVA.</span><span class="sxs-lookup"><span data-stu-id="bf42e-128">Complete Tax Statements.</span></span>

## <a name="see-also"></a><span data-ttu-id="bf42e-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bf42e-129">See Also</span></span>
[<span data-ttu-id="bf42e-130">Clôture des exercices et des périodes</span><span class="sxs-lookup"><span data-stu-id="bf42e-130">Closing Years and Periods</span></span>](year-close-years-periods.md)  
[<span data-ttu-id="bf42e-131">Clôture des livres</span><span class="sxs-lookup"><span data-stu-id="bf42e-131">Close Books</span></span>](year-close-books.md)

