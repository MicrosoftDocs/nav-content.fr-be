---
title: "Configurer une fiche magasin et définir des acheminements de transfert"
description: "Vous créez une fiche magasin pour chaque emplacement où vous stockez des articles d'inventaire, par exemple, un entrepôt ou un centre de distribution, et configurez des acheminements pour le transfert d'articles entre magasins."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, distribution center
ms.date: 06/02/2017
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ca48f5df7977328aec3cc6ba352eadb361144bcb
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-locations"></a><span data-ttu-id="fd97f-103">Comment configurer des magasins</span><span class="sxs-lookup"><span data-stu-id="fd97f-103">How to: Set Up Locations</span></span>
<span data-ttu-id="fd97f-104">Si vous achetez, enregistrez, ou vendez des articles à plusieurs magasins ou entrepôt, vous devez spécifier chaque magasin avec une fiche magasin et définir des acheminements transfert.</span><span class="sxs-lookup"><span data-stu-id="fd97f-104">If you buy, store, or sell items at more than one place or warehouse, you must set each location up with a location card and define transfer routes.</span></span>

<span data-ttu-id="fd97f-105">Vous pouvez ensuite créer des lignes de document pour un magasin spécifique, voir la disponibilité par magasin, et transférer le stock entre magasins.</span><span class="sxs-lookup"><span data-stu-id="fd97f-105">You can then create document lines for a specific location, view availability by location, and transfer inventory between locations.</span></span> <span data-ttu-id="fd97f-106">Pour plus d'informations, reportez-vous à [Gestion du stock](inventory-manage-inventory.md).</span><span class="sxs-lookup"><span data-stu-id="fd97f-106">For more information, see [Manage Inventory](inventory-manage-inventory.md).</span></span>

## <a name="to-create-a-location-card"></a><span data-ttu-id="fd97f-107">Pour créer une fiche magasin</span><span class="sxs-lookup"><span data-stu-id="fd97f-107">To create a location card</span></span>
1. <span data-ttu-id="fd97f-108">Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Magasins**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="fd97f-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.</span></span>
2. <span data-ttu-id="fd97f-109">Sélectionnez l'action **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="fd97f-109">Choose the **New** action.</span></span>
3. <span data-ttu-id="fd97f-110">Dans la fenêtre **Fiche magasin**, renseignez les champs comme nécessaire.</span><span class="sxs-lookup"><span data-stu-id="fd97f-110">In the **Location Card** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="fd97f-111">Répétez les étapes 2 et 3 pour chaque magasin dans lequel vous souhaitez conserver le stock.</span><span class="sxs-lookup"><span data-stu-id="fd97f-111">Repeat steps 2 and 3 for every location where you want to keep inventory.</span></span>

> [!NOTE]  
> <span data-ttu-id="fd97f-112">De nombreux champs de la fiche magasin se rapportent à la gestion des articles dans les processus enlogement et désenlogement.</span><span class="sxs-lookup"><span data-stu-id="fd97f-112">Many fields on the location card refer to the handling of items in inbound and outbound warehouse processes.</span></span> <span data-ttu-id="fd97f-113">Pour plus d'informations, voir [Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="fd97f-113">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span></span>

## <a name="to-create-a-transfer-route"></a><span data-ttu-id="fd97f-114">Pour créer un acheminement transfert</span><span class="sxs-lookup"><span data-stu-id="fd97f-114">To create a transfer route</span></span>
1. <span data-ttu-id="fd97f-115">Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Magasins**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="fd97f-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Transfer Routes**, and then choose the related link.</span></span>
2. <span data-ttu-id="fd97f-116">Sinon, à partir de n'importe quelle fenêtre **Fiche magasin**, cliquez sur **Acheminements transfert**.</span><span class="sxs-lookup"><span data-stu-id="fd97f-116">Alternatively, from any **Location Card** window, choose the **Transfer Routes** action.</span></span>
3. <span data-ttu-id="fd97f-117">Sélectionnez l'action **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="fd97f-117">Choose the **New** action.</span></span>
4. <span data-ttu-id="fd97f-118">Dans la fenêtre **Fiche magasin**, renseignez les champs comme nécessaire.</span><span class="sxs-lookup"><span data-stu-id="fd97f-118">In the **Location Card** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="fd97f-119">Vous pouvez à présent transférer des articles en stock entre deux magasins.</span><span class="sxs-lookup"><span data-stu-id="fd97f-119">You can now transfer inventory items between two locations.</span></span> <span data-ttu-id="fd97f-120">Pour plus d'informations, voir [Procédure : Transfert de stock entre des magasins](inventory-how-transfer-between-locations.md).</span><span class="sxs-lookup"><span data-stu-id="fd97f-120">For more information, see [How to: Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md).</span></span>    

## <a name="see-also"></a><span data-ttu-id="fd97f-121">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fd97f-121">See Also</span></span>
[<span data-ttu-id="fd97f-122">Gestion du stock</span><span class="sxs-lookup"><span data-stu-id="fd97f-122">Manage Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="fd97f-123">[Procédure : transfert de stock entre des magasins](inventory-how-transfer-between-locations.md)  </span><span class="sxs-lookup"><span data-stu-id="fd97f-123">[How to: Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md)  </span></span>  
<span data-ttu-id="fd97f-124">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="fd97f-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
<span data-ttu-id="fd97f-125">[Personnalisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-customizing-overview.md)</span><span class="sxs-lookup"><span data-stu-id="fd97f-125">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-customizing-overview.md)</span></span>  
[<span data-ttu-id="fd97f-126">Fonctionnalités marché</span><span class="sxs-lookup"><span data-stu-id="fd97f-126">General Business Functionality</span></span>](ui-across-business-areas.md)
