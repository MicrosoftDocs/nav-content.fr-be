---
title: "Procédure : valider par lots la consommation"
description: "Si le champ Méthode consommation indique **Manuelle**, vous devez valider les composants manuellement à l'aide d'une feuille consommation."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: bd4cedaf3fdb2d0f5627120836580fc82f4befa3
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-batch-post-production-consumption"></a><span data-ttu-id="52d18-103">Procédure : valider par lots la consommation de la production</span><span class="sxs-lookup"><span data-stu-id="52d18-103">How to: Batch Post Production Consumption</span></span>
<span data-ttu-id="52d18-104">Si le champ Méthode consommation indique **Manuelle**, vous devez valider les composants manuellement à l'aide d'une feuille consommation.</span><span class="sxs-lookup"><span data-stu-id="52d18-104">If the flushing method is **Manual**, you must post the components manually, using a consumption journal.</span></span>

<span data-ttu-id="52d18-105">Vous pouvez également configurer le système pour valider automatiquement (*consommer*) les composants lorsque vous lancez ou terminez des ordres de fabrication.</span><span class="sxs-lookup"><span data-stu-id="52d18-105">You can also set the system up to automatically post (*flush*) components when you start or finish production orders.</span></span> <span data-ttu-id="52d18-106">Pour plus d'informations, voir [Activer la consommation en aval des composants en fonction de la production réalisée](production-how-to-flush-components-according-to-operation-output.md).</span><span class="sxs-lookup"><span data-stu-id="52d18-106">For more information, see [Enable Flushing of Components According to Operation Output](production-how-to-flush-components-according-to-operation-output.md).</span></span>

## <a name="to-post-consumption-for-one-or-more-production-order-lines"></a><span data-ttu-id="52d18-107">Pour valider la consommation pour une ou plusieurs lignes ordre de fabrication</span><span class="sxs-lookup"><span data-stu-id="52d18-107">To post consumption for one or more production order lines</span></span>  
1.  <span data-ttu-id="52d18-108">Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuille consommation**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="52d18-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Consumption Journal**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="52d18-109">Renseignez les champs en indiquant les données relatives à l'ordre de fabrication et à la consommation.</span><span class="sxs-lookup"><span data-stu-id="52d18-109">Fill in the fields with the production order data and the consumption data.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    <span data-ttu-id="52d18-110">Si l'entrepôt dans lequel les composants sont stockés est configuré pour utiliser des emplacements mais pas le traitement de prélèvement, affectez un code emplacement à la ligne feuille pour indiquer d'où les articles doivent être prélevés dans l'entrepôt.</span><span class="sxs-lookup"><span data-stu-id="52d18-110">If the warehouse location where the components are stored is set up to use bins but does not require pick processing, assign a bin code to the journal line to indicate where the items should be taken from in the warehouse.</span></span> <span data-ttu-id="52d18-111">Pour plus d'informations, reportez-vous à [Procédure : prélever pour la fabrication ou l'assemblage](warehouse-how-to-pick-for-production.md).</span><span class="sxs-lookup"><span data-stu-id="52d18-111">For more information, see [How to: Pick for Production or Assembly](warehouse-how-to-pick-for-production.md).</span></span>  
3.  <span data-ttu-id="52d18-112">Choisissez l'action **Valider** pour valider la consommation.</span><span class="sxs-lookup"><span data-stu-id="52d18-112">Choose the **Post** action to post the consumption.</span></span> <span data-ttu-id="52d18-113">Les écritures comptables article associées sont réduites.</span><span class="sxs-lookup"><span data-stu-id="52d18-113">The related item ledger entries are reduced.</span></span>

## <a name="see-also"></a><span data-ttu-id="52d18-114">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="52d18-114">See Also</span></span>  
<span data-ttu-id="52d18-115">[Production](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="52d18-115">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="52d18-116">Paramétrage de la production</span><span class="sxs-lookup"><span data-stu-id="52d18-116">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="52d18-117">[Planifié](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="52d18-117">[Planning](production-planning.md)    </span></span>  
[<span data-ttu-id="52d18-118">STOCKS ET EN-COURS</span><span class="sxs-lookup"><span data-stu-id="52d18-118">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="52d18-119">Achats</span><span class="sxs-lookup"><span data-stu-id="52d18-119">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="52d18-120">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="52d18-120">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
