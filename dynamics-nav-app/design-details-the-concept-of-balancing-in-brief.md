---
title: "Détails de conception - Le concept d'équilibrage en bref"
description: "La demande est faite par les clients d'une société. L'approvisionnement est ce que la société peut créer et supprimer pour établir l'équilibre. Le système de planification commence avec la demande indépendante et effectue une traçabilité en amont jusqu'à l'approvisionnement."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 577f4a3a0b242c02ba62fd4746d2a1c96959b0fe
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-the-concept-of-balancing-in-brief"></a><span data-ttu-id="01a48-105">Détails de conception : Le concept d'équilibrage en bref</span><span class="sxs-lookup"><span data-stu-id="01a48-105">Design Details: The Concept of Balancing in Brief</span></span>
<span data-ttu-id="01a48-106">La demande est faite par les clients d'une société.</span><span class="sxs-lookup"><span data-stu-id="01a48-106">Demand is given by a company’s customers.</span></span> <span data-ttu-id="01a48-107">L'approvisionnement est ce que la société peut créer et supprimer pour établir l'équilibre.</span><span class="sxs-lookup"><span data-stu-id="01a48-107">Supply is what the company can create and remove to establish balance.</span></span> <span data-ttu-id="01a48-108">Le système de planification commence avec la demande indépendante et effectue une traçabilité en amont jusqu'à l'approvisionnement.</span><span class="sxs-lookup"><span data-stu-id="01a48-108">The planning system starts with the independent demand and then tracks backwards to the supply.</span></span>  
  
 <span data-ttu-id="01a48-109">Les profils de stock sont utilisés pour contenir des informations sur les demandes et les approvisionnements, les quantités et les délais.</span><span class="sxs-lookup"><span data-stu-id="01a48-109">The inventory profiles are used to contain information about the demands and supplies, quantities, and timing.</span></span> <span data-ttu-id="01a48-110">Ces profils constituent essentiellement les deux côtés de l'échelle de contrepartie.</span><span class="sxs-lookup"><span data-stu-id="01a48-110">These profiles essentially make up the two sides of the balancing scale.</span></span>  
  
 <span data-ttu-id="01a48-111">L'objectif du mécanisme de planification est d'équilibrer la demande et l'approvisionnement d'un article pour s'assurer que l'approvisionnement correspond à la demande de manière faisable, telle qu'elle est définie par les paramètres et les règles de planification.</span><span class="sxs-lookup"><span data-stu-id="01a48-111">The objective of the planning mechanism is to counterbalance the demand and supply of an item to ensure that supply will match demand in a feasible way as defined by the planning parameters and rules.</span></span>  
  
 ![](media/nav_app_supply_planning_2_balancing.png "NAV_APP_supply_planning_2_balancing")  
  
## <a name="see-also"></a><span data-ttu-id="01a48-112">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="01a48-112">See Also</span></span>  
 <span data-ttu-id="01a48-113">[Détails de conception : équilibrage de la demande et de l'approvisionnement](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="01a48-113">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
 <span data-ttu-id="01a48-114">[Détails de conception : concepts centraux du système de planification](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="01a48-114">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
 [<span data-ttu-id="01a48-115">Détails de conception : planification de l'approvisionnement</span><span class="sxs-lookup"><span data-stu-id="01a48-115">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
