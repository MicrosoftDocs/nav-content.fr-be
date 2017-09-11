---
title: Enregistrer automatiquement les interactions avec les contacts
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 1be15b94abf24da46dd0c46ce217aeb74378f400
ms.contentlocale: fr-be
ms.lasthandoff: 07/19/2017

---
# <a name="prepare-pre-closing-reports"></a><span data-ttu-id="023f3-102">Préparation d'états préalables à la clôture</span><span class="sxs-lookup"><span data-stu-id="023f3-102">Prepare Pre-Closing Reports</span></span>
<span data-ttu-id="023f3-103">Il existe de nombreux états standard qui vous permettent de vérifier la précision des comptes avant de clôturer les livres à la fin d'un exercice ou d'une période.</span><span class="sxs-lookup"><span data-stu-id="023f3-103">There are many standard reports that you can use to verify the accuracy of the accounts before closing the books at the end of a year or period.</span></span> <span data-ttu-id="023f3-104">Par exemple, vous pouvez utiliser l'état **Clients : Balance** pour vérifier que le solde d'un groupe comptabilisation client est égal au solde du compte général correspondant à une date donnée.</span><span class="sxs-lookup"><span data-stu-id="023f3-104">For example, you can use the **Customer - Trial Balance** report to verify that the balance for a customer posting group is equal to the balance on the corresponding general ledger account on a certain date.</span></span>

<span data-ttu-id="023f3-105">Le tableau suivant décrit un certain nombre d'états qui peuvent être utiles dans ce processus, ainsi que le nom du rapport.</span><span class="sxs-lookup"><span data-stu-id="023f3-105">The following table describes a number of reports that may be useful in this process along with the report name.</span></span>

|<span data-ttu-id="023f3-106">Pour</span><span class="sxs-lookup"><span data-stu-id="023f3-106">To</span></span>     |<span data-ttu-id="023f3-107">Afficher ce rapport</span><span class="sxs-lookup"><span data-stu-id="023f3-107">See this report</span></span>       |
|-------|----------------------|
|<span data-ttu-id="023f3-108">Imprimer un état Balance détaillé pour un ou plusieurs comptes bancaires avec des informations supplémentaires sur des écritures individuelles.</span><span class="sxs-lookup"><span data-stu-id="023f3-108">Print a detailed trial balance report for one or more bank accounts with additional information about individual entries.</span></span>|<span data-ttu-id="023f3-109">Banque :</span><span class="sxs-lookup"><span data-stu-id="023f3-109">Bank Acc.</span></span> <span data-ttu-id="023f3-110">Grand livre</span><span class="sxs-lookup"><span data-stu-id="023f3-110">- Detail Trial Bal.</span></span>|
|<span data-ttu-id="023f3-111">Imprimer un Grand livre pour les clients sélectionnés.</span><span class="sxs-lookup"><span data-stu-id="023f3-111">Print a detail trial balance for selected customers.</span></span>|<span data-ttu-id="023f3-112">Clients : Balance</span><span class="sxs-lookup"><span data-stu-id="023f3-112">Customer - Trial Balance</span></span>|
|<span data-ttu-id="023f3-113">Imprimer un Grand livre avec des informations détaillées sur des écritures individuelles pour les clients sélectionnés et durant une période sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="023f3-113">Print a detail trial balance with detailed information about individual entries, for selected customers during a selected period.</span></span>|<span data-ttu-id="023f3-114">Clients : Grand livre client</span><span class="sxs-lookup"><span data-stu-id="023f3-114">Customer - Detail Trial Bal.</span></span>|
|<span data-ttu-id="023f3-115">Imprimer un Grand livre pour les fournisseurs sélectionnés.</span><span class="sxs-lookup"><span data-stu-id="023f3-115">Print a detail trial balance for selected vendors.</span></span>|<span data-ttu-id="023f3-116">Fourn. : Balance</span><span class="sxs-lookup"><span data-stu-id="023f3-116">Vendor - Trial Balance</span></span>|
|<span data-ttu-id="023f3-117">Imprimer un Grand livre avec des informations détaillées sur des écritures individuelles pour les fournisseurs sélectionnés et durant une période sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="023f3-117">Print a detail trial balance with detailed information about individual entries, for selected vendors during a selected period.</span></span>|<span data-ttu-id="023f3-118">Fourn. : Grand livre fourn.</span><span class="sxs-lookup"><span data-stu-id="023f3-118">Vendor - Detail Trial Balance</span></span>|
|<span data-ttu-id="023f3-119">Imprimer une balance avec les chiffres de l'exercice en cours et de l'exercice précédent.</span><span class="sxs-lookup"><span data-stu-id="023f3-119">Print a trial balance with the current year's and the previous year's figures.</span></span>|<span data-ttu-id="023f3-120">Balance de clôture</span><span class="sxs-lookup"><span data-stu-id="023f3-120">Closing Trial Balance</span></span>|
|<span data-ttu-id="023f3-121">Imprimer un état Grand livre pour les soldes des comptes généraux.</span><span class="sxs-lookup"><span data-stu-id="023f3-121">Print a detailed trial balance report for general ledger account balances.</span></span>|<span data-ttu-id="023f3-122">Grand livre</span><span class="sxs-lookup"><span data-stu-id="023f3-122">Detail Trial Balance</span></span>|
|<span data-ttu-id="023f3-123">Imprimer un état Balance comprenant les soldes et les soldes période pour les comptes généraux.</span><span class="sxs-lookup"><span data-stu-id="023f3-123">Print a trial balance report with balances and net changes for general ledger accounts.</span></span>|<span data-ttu-id="023f3-124">Balance</span><span class="sxs-lookup"><span data-stu-id="023f3-124">Trial Balance</span></span>|
|<span data-ttu-id="023f3-125">Imprimer une balance pour une société consolidée.</span><span class="sxs-lookup"><span data-stu-id="023f3-125">Print a trial balance for a consolidated company.</span></span>|<span data-ttu-id="023f3-126">Balance consolidée</span><span class="sxs-lookup"><span data-stu-id="023f3-126">Consolidated Trial Balance</span></span>|
<span data-ttu-id="023f3-127">Pour afficher un état, dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez le nom tel qu'il s'affiche dans la table, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="023f3-127">To see a report, in the top right corner, choose the **Search for Page or Report** icon, type the name as it appears in the table, and then choose the related link.</span></span>

## <a name="see-also"></a><span data-ttu-id="023f3-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="023f3-128">See Also</span></span>
[<span data-ttu-id="023f3-129">Clôture des exercices et des périodes</span><span class="sxs-lookup"><span data-stu-id="023f3-129">Close Years and Periods</span></span>](year-close-years-periods.md)

