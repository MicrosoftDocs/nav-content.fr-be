---
title: Comment configurer des points de stock
description: "Vous pouvez utiliser des points de stock pour enregistrer des informations relatives à vos articles pour un code magasin ou variante donné."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 7ea31e21df842e63dc9d75998d2a0c3dfe65f1d3
ms.contentlocale: fr-be
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-set-up-stockkeeping-units"></a><span data-ttu-id="47bf1-103">Comment configurer des points de stock</span><span class="sxs-lookup"><span data-stu-id="47bf1-103">How to: Set Up Stockkeeping Units</span></span>
<span data-ttu-id="47bf1-104">Vous pouvez utiliser des points de stock pour enregistrer des informations relatives à vos articles pour un code magasin ou variante donné.</span><span class="sxs-lookup"><span data-stu-id="47bf1-104">You can use stockkeeping units to record information about your items for a specific location or a specific variant code.</span></span>  

 <span data-ttu-id="47bf1-105">Les points de stock représentent un supplément des fiches article.</span><span class="sxs-lookup"><span data-stu-id="47bf1-105">Stockkeeping units are a supplement to item cards.</span></span> <span data-ttu-id="47bf1-106">Ils ne les remplacent pas, bien qu'ils soient liés à ces documents.</span><span class="sxs-lookup"><span data-stu-id="47bf1-106">They do not replace them, although they are related to them.</span></span> <span data-ttu-id="47bf1-107">Les points de stock vous permettent de différencier des informations relatives à un article pour un magasin donné, comme un entrepôt ou un centre de distribution, ou une variante donnée, comme plusieurs numéros d'étagère et plusieurs informations de réapprovisionnement, pour un même article.</span><span class="sxs-lookup"><span data-stu-id="47bf1-107">Stockkeeping units allow you to differentiate information about an item for a specific location, such as a warehouse or distribution center, or a specific variant, such as different shelf numbers and different replenishment information, for the same item.</span></span>  

## <a name="to-set-up-a-stockkeeping-unit"></a><span data-ttu-id="47bf1-108">Pour configurer un point de stock</span><span class="sxs-lookup"><span data-stu-id="47bf1-108">To set up a stockkeeping unit</span></span>  

1.  <span data-ttu-id="47bf1-109">Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Points de stock**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="47bf1-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Stockkeeping Units**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="47bf1-110">Sélectionnez l'action **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="47bf1-110">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="47bf1-111">Renseignez les champs de la fiche.</span><span class="sxs-lookup"><span data-stu-id="47bf1-111">Fill in the fields on the card.</span></span> <span data-ttu-id="47bf1-112">Les champs suivants sont nécessaires : **N° article**, **Code magasin** et/ou **Code variante**.</span><span class="sxs-lookup"><span data-stu-id="47bf1-112">The following fields are required: **Item No.**, **Location Code**, and/or **Variant Code**.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

<span data-ttu-id="47bf1-113">Après avoir configuré le premier point de stock pour un article, la case à cocher **Point de stock** sur la fiche **Article** est activée.</span><span class="sxs-lookup"><span data-stu-id="47bf1-113">When you have set up the first stockkeeping unit for an item, the **Stockkeeping Unit Exists** check box on the **Item** card is selected.</span></span>  

<span data-ttu-id="47bf1-114">Pour créer plusieurs points de stock pour un article, utilisez le traitement par lots **Créer point de stock**.</span><span class="sxs-lookup"><span data-stu-id="47bf1-114">To create several stockkeeping units for an item, use the **Create Stockkeeping Unit** batch job.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="47bf1-115">Les informations de la fiche **Point de stock** sont prioritaires par rapport à celles de la fiche **Article**.</span><span class="sxs-lookup"><span data-stu-id="47bf1-115">The information on the **Stockkeeping Unit** card has priority over the **Item** card.</span></span>  

## <a name="see-also"></a><span data-ttu-id="47bf1-116">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="47bf1-116">See Also</span></span>  
[<span data-ttu-id="47bf1-117">Procédure : enregistrer de nouveaux articles</span><span class="sxs-lookup"><span data-stu-id="47bf1-117">How to: Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="47bf1-118">Configuration de la gestion des entrepôts</span><span class="sxs-lookup"><span data-stu-id="47bf1-118">Setting Up Warehouse Management</span></span>](warehouse-setup-warehouse.md)  
[<span data-ttu-id="47bf1-119">Gestion d'entrepôt</span><span class="sxs-lookup"><span data-stu-id="47bf1-119">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="47bf1-120">STOCKS ET EN-COURS</span><span class="sxs-lookup"><span data-stu-id="47bf1-120">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="47bf1-121">[Gestion des assemblages](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="47bf1-121">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="47bf1-122">Détails de conception : gestion d'entrepôt</span><span class="sxs-lookup"><span data-stu-id="47bf1-122">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="47bf1-123">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="47bf1-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

