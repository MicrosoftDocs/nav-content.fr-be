---
title: "Procédure : utiliser l'unité de lot de fabrication"
description: "Si un article est stocké dans une unité mais produit dans une autre, l'ordre de fabrication doit utiliser une unité de lot de fabrication pour calculer la quantité correcte des composants. Une situation dans laquelle un article fabriqué est stocké en pièces mais produit en tonnes est un exemple d'un calcul d'unité de lot de fabrication."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/14/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: cf0c91b076f473c12e61ce82d870a66e352c1920
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-work-with-manufacturing-batch-units-of-measure"></a><span data-ttu-id="243ed-104">Procédure : utiliser les unités de lot de fabrication</span><span class="sxs-lookup"><span data-stu-id="243ed-104">How to: Work with Manufacturing Batch Units of Measure</span></span>
<span data-ttu-id="243ed-105">Si un article est stocké dans une unité mais produit dans une autre, un ordre de fabrication utilisant une unité de lot de fabrication est créé pour calculer la quantité correcte des composants durant le traitement par lots **Actualiser O.F.**.</span><span class="sxs-lookup"><span data-stu-id="243ed-105">If an item is stocked in one unit of measure but produced in another, a production order is created that uses a manufacturing batch unit of measure to calculate the correct quantity of the components during the **Refresh Production Order** batch job.</span></span> <span data-ttu-id="243ed-106">Une situation dans laquelle un article fabriqué est stocké en pièces mais produit en tonnes est un exemple d'un calcul d'unité de lot de fabrication.</span><span class="sxs-lookup"><span data-stu-id="243ed-106">An example of a manufacturing batch unit of measure calculation is when a manufactured item is stocked in pieces but produced in tons.</span></span>  

## <a name="to-create-a-production-bom-using-a-batch-unit-of-measure"></a><span data-ttu-id="243ed-107">Pour créer une nomenclature de production à l'aide d'une unité de lot</span><span class="sxs-lookup"><span data-stu-id="243ed-107">To create a production BOM using a batch unit of measure</span></span>  
1.  <span data-ttu-id="243ed-108">L'unité de lot de fabrication est configurée comme unité alternative dans la fenêtre **Unités article** pour l'article à produire.</span><span class="sxs-lookup"><span data-stu-id="243ed-108">The manufacturing batch unit of measure is set up as an alternative unit of measure in the **Item Units of Measure** window on the item to be produced.</span></span> <span data-ttu-id="243ed-109">L'unité de lot ne remplace pas l'unité de base pour l'article.</span><span class="sxs-lookup"><span data-stu-id="243ed-109">The batch unit of measure will not replace the base unit of measure on the item.</span></span>  
2.  <span data-ttu-id="243ed-110">Créez une nomenclature de production pour l'article configuré avec l'unité de lot de fabrication.</span><span class="sxs-lookup"><span data-stu-id="243ed-110">Create a production BOM for the item set up with the manufacturing batch unit of measure.</span></span> <span data-ttu-id="243ed-111">Pour plus d'informations, reportez\-vous à [Procédure : créer des nomenclatures de production](production-how-to-create-production-boms.md).</span><span class="sxs-lookup"><span data-stu-id="243ed-111">For more information, see [How to: Create Production BOMs](production-how-to-create-production-boms.md).</span></span>  
3.  <span data-ttu-id="243ed-112">Dans le champ **Code unité**, sélectionnez l'unité de lot de fabrication.</span><span class="sxs-lookup"><span data-stu-id="243ed-112">In the **Unit of Measure Code** field, select the manufacturing batch unit of measure.</span></span>  
4.  <span data-ttu-id="243ed-113">Pour chaque ligne de nomenclature de production, dans le champ **Quantité par**, entrez la quantité de cet article composant requise pour créer cette unité de lot.</span><span class="sxs-lookup"><span data-stu-id="243ed-113">For each production BOM line, in the **Quantity Per** field, enter the quantity of this component item that is required to create this batch unit of measure.</span></span>  
5.  <span data-ttu-id="243ed-114">Ouvrez la fenêtre **Fiche article** pour l'article en question.</span><span class="sxs-lookup"><span data-stu-id="243ed-114">Open the **Item Card** for the related item.</span></span>  

    <span data-ttu-id="243ed-115">Sur le raccourci **Réapprovisionnement**, dans le champ **N° nomenclature production**, sélectionnez la nomenclature de production créée précédemment.</span><span class="sxs-lookup"><span data-stu-id="243ed-115">On the **Replenishment** FastTab, in the **Production BOM No.** field, select the production BOM created above.</span></span>  
6.  <span data-ttu-id="243ed-116">Créez un en-tête d'ordre de fabrication en utilisant l'article configuré avec l'unité de lot de fabrication.</span><span class="sxs-lookup"><span data-stu-id="243ed-116">Create a production order header using the item set up with the manufacturing batch unit of measure.</span></span> <span data-ttu-id="243ed-117">Pour plus d'informations, voir [Procédure : créer des ordres de fabrication](production-how-to-create-production-orders.md).</span><span class="sxs-lookup"><span data-stu-id="243ed-117">For more information, see [How to: Create Production Orders](production-how-to-create-production-orders.md).</span></span>  
7.  <span data-ttu-id="243ed-118">Choisissez l'action **Actualiser**, puis le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="243ed-118">Choose the **Refresh** action, and then choose  the **OK** button.</span></span>  

<span data-ttu-id="243ed-119">Sur le raccourci **Lignes**, choisissez l'action **Ligne**, puis l'action **Composants** pour afficher le résultat.</span><span class="sxs-lookup"><span data-stu-id="243ed-119">On the **Lines** FastTab, choose the **Line** action, and then choose the **Components** action to view the result.</span></span> <span data-ttu-id="243ed-120">Le programme calcule la quantité correcte de composants nécessaire pour satisfaire la nomenclature de production, basée sur l'unité de lot de fabrication.</span><span class="sxs-lookup"><span data-stu-id="243ed-120">The program calculates the correct quantity of the components needed to satisfy the production BOM based on the manufacturing batch unit of measure.</span></span>  

## <a name="to-calculate-a-manufacturing-batch-unit-of-measure-on-a-production-order"></a><span data-ttu-id="243ed-121">Pour calculer une unité de lot de fabrication sur un ordre de fabrication</span><span class="sxs-lookup"><span data-stu-id="243ed-121">To calculate a manufacturing batch unit of measure on a production order</span></span>  
1.  <span data-ttu-id="243ed-122">Créez un en-tête d'ordre de fabrication en utilisant l'article configuré avec l'unité de lot de fabrication.</span><span class="sxs-lookup"><span data-stu-id="243ed-122">Create a production order header using the item set up with the manufacturing batch unit of measure.</span></span>  
2.  <span data-ttu-id="243ed-123">Dans le champ **N° article** de la ligne ordre de fabrication, tapez le numéro article utilisé dans l'en-tête.</span><span class="sxs-lookup"><span data-stu-id="243ed-123">In the **Item No.** field in the Production Order line, type the same item number used in the header.</span></span>  
3.  <span data-ttu-id="243ed-124">Dans le champ **Quantité**, entrez la quantité utilisée dans l'en-tête.</span><span class="sxs-lookup"><span data-stu-id="243ed-124">In the **Quantity** field, enter the same quantity used in the header.</span></span>  
4.  <span data-ttu-id="243ed-125">Dans le champ **Code unité**, sélectionnez le code unité de lot de fabrication.</span><span class="sxs-lookup"><span data-stu-id="243ed-125">In the **Unit of Measure Code** field, select the manufacturing batch unit of measure code.</span></span>  
5.  <span data-ttu-id="243ed-126">Sélectionnez l'action **Actualiser**.</span><span class="sxs-lookup"><span data-stu-id="243ed-126">Choose the **Refresh** action.</span></span>
6.  <span data-ttu-id="243ed-127">Sur le raccourci **Calculer**, désactivez la case à cocher **Lignes**.</span><span class="sxs-lookup"><span data-stu-id="243ed-127">On the **Calculate** FastTab, clear the **Lines** check box.</span></span>  
7.  <span data-ttu-id="243ed-128">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="243ed-128">Choose the **OK** button.</span></span>  
8.  <span data-ttu-id="243ed-129">Sur le raccourci **Lignes**, choisissez l'action **Ligne**, puis l'action **Composants** pour afficher le résultat.</span><span class="sxs-lookup"><span data-stu-id="243ed-129">On the **Lines** FastTab, choose the **Line** action, and then choose the **Components** action to view the result.</span></span> <span data-ttu-id="243ed-130">La quantité correcte de composants nécessaire pour satisfaire la nomenclature de production est calculée sur la base de l'unité de lot de fabrication.</span><span class="sxs-lookup"><span data-stu-id="243ed-130">The correct quantity of the components needed to satisfy the production BOM is calculated based on the manufacturing batch unit of measure.</span></span>  

## <a name="see-also"></a><span data-ttu-id="243ed-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="243ed-131">See Also</span></span>  
[<span data-ttu-id="243ed-132">Procédure : créer des gammes</span><span class="sxs-lookup"><span data-stu-id="243ed-132">How to: Create Routings</span></span>](production-how-to-create-routings.md)  
<span data-ttu-id="243ed-133">[Procédure : créer des nomenclatures de production](production-how-to-create-production-boms.md)   </span><span class="sxs-lookup"><span data-stu-id="243ed-133">[How to: Create Production BOMs](production-how-to-create-production-boms.md)   </span></span>  
[<span data-ttu-id="243ed-134">Paramétrage de la production</span><span class="sxs-lookup"><span data-stu-id="243ed-134">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="243ed-135">[Production](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="243ed-135">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
<span data-ttu-id="243ed-136">[Planifié](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="243ed-136">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="243ed-137">STOCKS ET EN-COURS</span><span class="sxs-lookup"><span data-stu-id="243ed-137">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="243ed-138">Achats</span><span class="sxs-lookup"><span data-stu-id="243ed-138">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="243ed-139">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="243ed-139">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
