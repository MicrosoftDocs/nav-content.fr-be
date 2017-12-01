---
title: "Exemple de scénario - Définition des ventilations dynamique sur la base des articles vendus"
description: "Cette rubrique explique comment définir les affectations à l'aide du mode de ventilation dynamique. Dans l'exemple, vous modifiez la ventilation dynamique des coûts pour que le centre de coûts VENTES prenne en charge le nouveau ÉQUIPEMENT IT de coûts associés. Les packages ÉQUIPEMENT IT ont des numéros d'articles dont la plage s'échelonne entre 8904-W et 8924-W. Vous pouvez utiliser les chiffres de ventes de l'exercice précédent pour en calculer la part. La ventilation est validée en fonction du type de coût 9903."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 32310933bb8eb483bd30270802c8943c55423a2f
ms.contentlocale: fr-be
ms.lasthandoff: 12/01/2017

---
# <a name="scenario-example-defining-dynamic-allocations-based-on-items-sold"></a><span data-ttu-id="f9b59-107">Exemple de scénario : Définition des ventilations dynamique sur la base des articles vendus</span><span class="sxs-lookup"><span data-stu-id="f9b59-107">Scenario Example: Defining Dynamic Allocations Based on Items Sold</span></span>
<span data-ttu-id="f9b59-108">Cette rubrique explique comment définir les affectations à l'aide du mode de ventilation dynamique.</span><span class="sxs-lookup"><span data-stu-id="f9b59-108">This topic shows an example of how to define allocations by using the dynamic allocation method.</span></span> <span data-ttu-id="f9b59-109">Dans l'exemple, vous modifiez la ventilation dynamique des coûts pour que le centre de coûts VENTES prenne en charge le nouveau ÉQUIPEMENT IT de coûts associés.</span><span class="sxs-lookup"><span data-stu-id="f9b59-109">In the example, you change the dynamic allocation of the costs for the SALES cost center to support the new cost object IT EQUIPMENT.</span></span> <span data-ttu-id="f9b59-110">Les packages ÉQUIPEMENT IT ont des numéros d'articles dont la plage s'échelonne entre 8904-W et 8924-W.</span><span class="sxs-lookup"><span data-stu-id="f9b59-110">IT EQUIPMENT packages have item numbers in the range from 8904-W to 8924-W.</span></span> <span data-ttu-id="f9b59-111">Vous pouvez utiliser les chiffres de ventes de l'exercice précédent pour en calculer la part.</span><span class="sxs-lookup"><span data-stu-id="f9b59-111">You use the previous year’s sales figures to calculate the share.</span></span> <span data-ttu-id="f9b59-112">La ventilation est validée en fonction du type de coût 9903.</span><span class="sxs-lookup"><span data-stu-id="f9b59-112">The allocation is posted to the helping cost type 9903.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="f9b59-113">L'exemple utilise les données de démonstration dans [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="f9b59-113">The example uses the demo data in the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="to-define-dynamic-allocations-based-on-items-sold-in-the-previous-year"></a><span data-ttu-id="f9b59-114">Pour définir les ventilations dynamique en fonction des articles vendus de l'exercice précédent</span><span class="sxs-lookup"><span data-stu-id="f9b59-114">To define dynamic allocations based on items sold in the previous year</span></span>  

1.  <span data-ttu-id="f9b59-115">Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Affectation des coûts**, puis choisissez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="f9b59-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Cost Allocations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f9b59-116">Dans la fenêtre **Affectation des coûts**, sélectionnez l'action **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="f9b59-116">In the **Cost Allocation** window, choose the **New** action.</span></span>  
3.  <span data-ttu-id="f9b59-117">Dans le champ **ID**, appuyez sur Entrée ou saisissez un ID.</span><span class="sxs-lookup"><span data-stu-id="f9b59-117">In the **ID** field, press Enter or enter an ID.</span></span>  
4.  <span data-ttu-id="f9b59-118">Dans le champ **Niveau**, saisissez **1**.</span><span class="sxs-lookup"><span data-stu-id="f9b59-118">In the **Level** field, enter **1**.</span></span>  
5.  <span data-ttu-id="f9b59-119">Dans les champs **Valide à partir de** et **Valide jusque**, entrez les dates appropriées.</span><span class="sxs-lookup"><span data-stu-id="f9b59-119">In the **Valid From** and **Valid To** fields, enter appropriate dates.</span></span>  
6.  <span data-ttu-id="f9b59-120">Dans le champ **Code centre de coûts**, entrez **VENTES**.</span><span class="sxs-lookup"><span data-stu-id="f9b59-120">In the **Cost Center Code** field, enter **SALES**.</span></span>  
7.  <span data-ttu-id="f9b59-121">Dans le champ **Type de crédit\\\/coût**, entrez le type de coût **9903**.</span><span class="sxs-lookup"><span data-stu-id="f9b59-121">In the **Credit to Cost Type** field, enter the cost type **9903**.</span></span>  
8.  <span data-ttu-id="f9b59-122">Dans le champ **Type coût cible**, entrez le type de coût **9903**.</span><span class="sxs-lookup"><span data-stu-id="f9b59-122">In the **Target Cost Type** field, enter the cost type **9903**.</span></span>  
9. <span data-ttu-id="f9b59-123">Dans le champ **Objet de coûts cible**, sélectionnez **Nouveau** pour créer un nouvel objet de coût ÉQUIPEMENT IT et renseigner les champs, le cas échéant.</span><span class="sxs-lookup"><span data-stu-id="f9b59-123">In the **Target Cost Object** field, choose **New** to create a new cost object IT EQUIPMENT and fill in fields as necessary.</span></span> <span data-ttu-id="f9b59-124">Sélectionnez **ÉQUIPEMENT IT**.</span><span class="sxs-lookup"><span data-stu-id="f9b59-124">Select **IT EQUIPMENT**.</span></span> <span data-ttu-id="f9b59-125">Laissez le champ **Centre de coûts cible** vide.</span><span class="sxs-lookup"><span data-stu-id="f9b59-125">Leave the **Target Cost Center** field blank.</span></span>  
10. <span data-ttu-id="f9b59-126">Dans le champ **Type cible affectation**, sélectionnez **Tous les coûts** pour définir le mode d'affectation de tous les coûts cumulés.</span><span class="sxs-lookup"><span data-stu-id="f9b59-126">In the **Allocation Target Type** field, select **All Costs** to define how all accumulated costs are allocated.</span></span>  
11. <span data-ttu-id="f9b59-127">Dans le champ **Base**, sélectionnez la base de ventilation **Articles vendus (Montant)**.</span><span class="sxs-lookup"><span data-stu-id="f9b59-127">In the **Base** field, select the allocation base **Items Sold (Amount)**.</span></span>  
12. <span data-ttu-id="f9b59-128">Dans le champ **Filtre n°**, entrez **8904-W..8924-W**.</span><span class="sxs-lookup"><span data-stu-id="f9b59-128">In the **No. Filter** field, enter **8904-W..8924-W**.</span></span>  
13. <span data-ttu-id="f9b59-129">Dans le champ **Code filtre date**, entrez **Année précédente**.</span><span class="sxs-lookup"><span data-stu-id="f9b59-129">In the **Date Filter Code** field, enter **Last Year**.</span></span>  
14. <span data-ttu-id="f9b59-130">Choisissez l'action **Calculer la clé de ventilation** pour calculer la part.</span><span class="sxs-lookup"><span data-stu-id="f9b59-130">Choose the **Calculate Allocation Key** action to calculate the share.</span></span>  

    > [!IMPORTANT]  
    >  [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="f9b59-131"> utilise les chiffres de ventes des exercices précédents pour calculer une part de 1596,50 DS avec 100 % alloués pour les packages ÉQUIPEMENT IT.</span><span class="sxs-lookup"><span data-stu-id="f9b59-131"> uses the previous years’ sales figures to calculate a share of 1596.50 LCY with 100 percent for the IT EQUIPMENT packages.</span></span> <span data-ttu-id="f9b59-132">Cela signifie que tous les articles vendus au cours de l'exercice précédent seront affectés au ÉQUIPEMENT IT des coûts associés.</span><span class="sxs-lookup"><span data-stu-id="f9b59-132">This means that all of the items sold last year will be allocated to the cost object IT EQUIPMENT.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f9b59-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f9b59-133">See Also</span></span>  
 <span data-ttu-id="f9b59-134">[Définition de filtres pour les bases de ventilation dynamique](finance-setting-filters-for-dynamic-allocation-bases.md) </span><span class="sxs-lookup"><span data-stu-id="f9b59-134">[Setting Filters for Dynamic Allocation Bases](finance-setting-filters-for-dynamic-allocation-bases.md) </span></span>  
 <span data-ttu-id="f9b59-135">[Procédure : configurer la source d'affectation et ses cibles](finance-how-to-set-up-allocation-source-and-targets.md) </span><span class="sxs-lookup"><span data-stu-id="f9b59-135">[How to: Set Up Allocation Source and Targets](finance-how-to-set-up-allocation-source-and-targets.md) </span></span>  
 <span data-ttu-id="f9b59-136">[Définition et répartition des coûts](finance-define-and-allocate-costs.md) </span><span class="sxs-lookup"><span data-stu-id="f9b59-136">[Defining and Allocating Costs](finance-define-and-allocate-costs.md) </span></span>  
 <span data-ttu-id="f9b59-137">[Terminologie en comptabilité analytique](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="f9b59-137">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
 [<span data-ttu-id="f9b59-138">À propos de la comptabilité analytique</span><span class="sxs-lookup"><span data-stu-id="f9b59-138">About Cost Accounting</span></span>](finance-about-cost-accounting.md)

