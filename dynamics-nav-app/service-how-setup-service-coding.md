---
title: Configurer des codes prestations standards
description: "Découvrez comment configurer des codes pour les activités de service que vous effectuez souvent."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: service, service item, service order, repairs, maintenance
ms.date: 08/22/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 109e71ab1b06ccbe0a931a998ae0681713eff9da
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-set-up-standard-service-codes"></a><span data-ttu-id="03ae8-103">Procédure : configurer des codes prestation standard :</span><span class="sxs-lookup"><span data-stu-id="03ae8-103">How to: Set Up Standard Service Codes</span></span>
<span data-ttu-id="03ae8-104">Lorsque vous exécutez un service courant, il est fréquent que vous deviez créer des documents service qui utilisent des lignes service contenant des informations similaires.</span><span class="sxs-lookup"><span data-stu-id="03ae8-104">When you perform typical service, you often have to create service documents that use service lines that contain similar information.</span></span> <span data-ttu-id="03ae8-105">Pour faciliter la création de ces lignes, vous pouvez configurer des codes prestation standard avec un ensemble prédéfini de lignes service.</span><span class="sxs-lookup"><span data-stu-id="03ae8-105">To make it easy to create these lines, you can set up standard service codes that have a predefined set of service lines.</span></span> <span data-ttu-id="03ae8-106">Lorsque vous sélectionnez le code sur un document service, les lignes sont saisies automatiquement.</span><span class="sxs-lookup"><span data-stu-id="03ae8-106">When you choose the code on a service document, the lines are entered automatically.</span></span> <span data-ttu-id="03ae8-107">Vous pouvez configurer autant de codes prestation standard que vous le souhaitez, et chaque code peut avoir un nombre illimité de lignes service de différents types, notamment l'article, la ressource, le coût ou le texte standard qui lui est associé.</span><span class="sxs-lookup"><span data-stu-id="03ae8-107">You can set up any number of standard service codes, and each code can have an unlimited number of service lines of different types, including item, resource, cost, or standrd text linked to it.</span></span> <span data-ttu-id="03ae8-108">Créez des lignes service pour chaque code prestation standard dans la fiche **Code prestation standard**.</span><span class="sxs-lookup"><span data-stu-id="03ae8-108">You create service lines of each standard serice code on the **Standard Service Code** card.</span></span> <span data-ttu-id="03ae8-109">Vous pouvez ensuite affecter les codes prestation standard à des groupes articles de service dans la page **Codes gpe articles de service standard**.</span><span class="sxs-lookup"><span data-stu-id="03ae8-109">You then assign standard service codes to service item groups on the **Standard Serv. Item Gr. Codes** page.</span></span> <span data-ttu-id="03ae8-110">Par la suite, lorsque vous créez un document service, vous pouvez utiliser l'action **Extraire codes prestation std** pour ajouter des lignes service.</span><span class="sxs-lookup"><span data-stu-id="03ae8-110">Later, when you create a service document, you can use the **Get Standard Service Codes** action to add service lines.</span></span>  
  
> [!Tip]
>  <span data-ttu-id="03ae8-111">Vous pouvez utiliser le même concept pour créer des lignes dans les documents achat et vente.</span><span class="sxs-lookup"><span data-stu-id="03ae8-111">You can use the same concept to create lines on sales and purchase documents.</span></span> <span data-ttu-id="03ae8-112">Pour plus d'informations, voir [Procédure : Créer des lignes vente et achat récurrentes](sales-how-work-standard-lines.md).</span><span class="sxs-lookup"><span data-stu-id="03ae8-112">For more information, see [How to: Create Recurring Sales and Purchase Lines](sales-how-work-standard-lines.md).</span></span>    
  
## <a name="to-set-up-a-standard-service-code"></a><span data-ttu-id="03ae8-113">Pour configurer un code prestation standard</span><span class="sxs-lookup"><span data-stu-id="03ae8-113">To set up a standard service code</span></span>    
1. <span data-ttu-id="03ae8-114">Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Codes prestation standard**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="03ae8-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Standard Service Codes**, and then choose the related link.</span></span>  
2. <span data-ttu-id="03ae8-115">Renseignez les champs selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="03ae8-115">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
4. <span data-ttu-id="03ae8-116">Renseignez les lignes service liées à ce code prestation.</span><span class="sxs-lookup"><span data-stu-id="03ae8-116">Fill in the service lines linked to this service code.</span></span>  

## <a name="to-assign-a-standard-service-code-to-a-service-item-group"></a><span data-ttu-id="03ae8-117">Pour affecter un code prestation standard à un groupe articles de service</span><span class="sxs-lookup"><span data-stu-id="03ae8-117">To assign a standard service code to a service item group</span></span>
1. <span data-ttu-id="03ae8-118">Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Groupes articles de service**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="03ae8-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service item Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="03ae8-119">Renseignez les champs selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="03ae8-119">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="03ae8-120">Renseignez les lignes service liées à ce code prestation.</span><span class="sxs-lookup"><span data-stu-id="03ae8-120">Fill in the service lines linked to this service code.</span></span>  

## <a name="see-also"></a><span data-ttu-id="03ae8-121">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="03ae8-121">See Also</span></span>
[<span data-ttu-id="03ae8-122">Gestion des services</span><span class="sxs-lookup"><span data-stu-id="03ae8-122">Service Management</span></span>](service-service.md)