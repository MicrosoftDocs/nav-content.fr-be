---
title: "Détails de conception - Affecter une priorité aux commandes"
description: "Découvrez comment affecter une priorité pour répondre à la demande et l'approvisionnement."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, priority, prioritize, order, sku, demand, supply
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c01ad1bb74e01ff81f35159865eddf14e9a34910
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-prioritizing-orders"></a><span data-ttu-id="aa711-103">Détails de conception : Affecter une priorité aux commandes</span><span class="sxs-lookup"><span data-stu-id="aa711-103">Design Details: Prioritizing Orders</span></span>
<span data-ttu-id="aa711-104">Dans un point de stock donné, la date demandée ou disponible représente la priorité la plus élevée ; la demande du jour doit être traitée avant la demande de la semaine suivante.</span><span class="sxs-lookup"><span data-stu-id="aa711-104">Within a given SKU, the requested or available date represents the highest priority; the demand of today should be dealt with before the demand of next week.</span></span> <span data-ttu-id="aa711-105">Mais en plus de cette priorité générale, le système de planification suggère également que le type de demande doit être rempli avant de répondre à une autre demande.</span><span class="sxs-lookup"><span data-stu-id="aa711-105">But in addition to this overall priority, the planning system will also suggest which type of demand should be fulfilled before fulfilling another demand.</span></span> <span data-ttu-id="aa711-106">De même, il suggère que la source d'approvisionnement soit lettrée avant d'appliquer d'autres sources d'approvisionnement.</span><span class="sxs-lookup"><span data-stu-id="aa711-106">Likewise, it will suggest what source of supply should be applied before applying other sources of supply.</span></span> <span data-ttu-id="aa711-107">Ceci est effectué en fonction des priorités de la commande.</span><span class="sxs-lookup"><span data-stu-id="aa711-107">This is done according to order priorities.</span></span>  
  
<span data-ttu-id="aa711-108">La demande et l'approvisionnement chargés contribuent à un profil pour le stock prévisionnel en fonction des priorités suivantes :</span><span class="sxs-lookup"><span data-stu-id="aa711-108">Loaded demand and supply contribute to a profile for the projected inventory according to the following priorities:</span></span>  
  
## <a name="priorities-on-the-demand-side"></a><span data-ttu-id="aa711-109">Priorités du côté de la demande</span><span class="sxs-lookup"><span data-stu-id="aa711-109">Priorities on the Demand Side</span></span>  
1. <span data-ttu-id="aa711-110">Déjà expédié : écriture comptable article</span><span class="sxs-lookup"><span data-stu-id="aa711-110">Already shipped: Item Ledger Entry</span></span>  
2. <span data-ttu-id="aa711-111">Retour achat</span><span class="sxs-lookup"><span data-stu-id="aa711-111">Purchase Return Order</span></span>  
3. <span data-ttu-id="aa711-112">Ecriture réservation</span><span class="sxs-lookup"><span data-stu-id="aa711-112">Sales Order</span></span>  
4. <span data-ttu-id="aa711-113">Commande service</span><span class="sxs-lookup"><span data-stu-id="aa711-113">Service Order</span></span>  
5. <span data-ttu-id="aa711-114">Besoin de composants de production</span><span class="sxs-lookup"><span data-stu-id="aa711-114">Production Component Need</span></span>  
6. <span data-ttu-id="aa711-115">Ligne d'ordre d'assemblage</span><span class="sxs-lookup"><span data-stu-id="aa711-115">Assembly Order Line</span></span>  
7. <span data-ttu-id="aa711-116">Commande désenlogement transfert</span><span class="sxs-lookup"><span data-stu-id="aa711-116">Outbound Transfer Order</span></span>  
8. <span data-ttu-id="aa711-117">Commande ouverte (qui n'a pas déjà été consommée par les commandes vente associées)</span><span class="sxs-lookup"><span data-stu-id="aa711-117">Blanket Order (that has not already been consumed by related sales orders)</span></span>  
9. <span data-ttu-id="aa711-118">Prévision (qui n'a pas déjà été consommée par d'autres commandes vente)</span><span class="sxs-lookup"><span data-stu-id="aa711-118">Forecast (that has not already been consumed by other sales orders)</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="aa711-119">Les retours achat ne sont généralement pas impliqués dans la planification d'approvisionnement ; ils doivent toujours être réservés à partir du lot qui va être retourné.</span><span class="sxs-lookup"><span data-stu-id="aa711-119">Purchase returns are usually not involved in supply planning; they should always be reserved from the lot that is going to be returned.</span></span> <span data-ttu-id="aa711-120">S'il ne sont pas réservés, les retours achat jouent un rôle dans la disponibilité et sont classés en priorité élevée pour éviter que le système de planification suggère une commande approvisionnement uniquement pour servir un retour achat.</span><span class="sxs-lookup"><span data-stu-id="aa711-120">If not reserved, purchase returns play a role in the availability and are highly prioritized to avoid that the planning system suggests a supply order just to serve a purchase return.</span></span>  
  
## <a name="priorities-on-the-supply-side"></a><span data-ttu-id="aa711-121">Priorités du côté de l'approvisionnement</span><span class="sxs-lookup"><span data-stu-id="aa711-121">Priorities on the Supply Side</span></span>  
1. <span data-ttu-id="aa711-122">Déjà dans le stock : écriture comptable article (Flexibilité planification = Aucune)</span><span class="sxs-lookup"><span data-stu-id="aa711-122">Already in inventory: Item Ledger Entry (Planning Flexibility = None)</span></span>  
2. <span data-ttu-id="aa711-123">Retour vente (flexibilité de planification = aucune)</span><span class="sxs-lookup"><span data-stu-id="aa711-123">Sales Return Order (Planning Flexibility = None)</span></span>  
3. <span data-ttu-id="aa711-124">Enlogement transfert</span><span class="sxs-lookup"><span data-stu-id="aa711-124">Inbound Transfer Order</span></span>  
4. <span data-ttu-id="aa711-125">Ordre de fabrication</span><span class="sxs-lookup"><span data-stu-id="aa711-125">Production Order</span></span>  
5. <span data-ttu-id="aa711-126">Ordre d'assemblage</span><span class="sxs-lookup"><span data-stu-id="aa711-126">Assembly Order</span></span>  
6. <span data-ttu-id="aa711-127">Commande achat</span><span class="sxs-lookup"><span data-stu-id="aa711-127">Purchase Order</span></span>  
  
## <a name="priority-related-to-the-state-of-demand-and-supply"></a><span data-ttu-id="aa711-128">Priorité liée à l'état de la demande et de l'approvisionnement</span><span class="sxs-lookup"><span data-stu-id="aa711-128">Priority Related to the State of Demand and Supply</span></span>  
<span data-ttu-id="aa711-129">Outre les priorités accordées par le type d'offre et de demande, l'état actuel des commandes dans le processus d'exécution définit également une priorité.</span><span class="sxs-lookup"><span data-stu-id="aa711-129">Apart from priorities given by the type of demand and supply, the present state of the orders in the execution process also defines a priority.</span></span> <span data-ttu-id="aa711-130">Par exemple, les activités entrepôt ont un effet et le statut des commandes vente, des commandes achat, des ordres de transfert, des ordres d'assemblage et des ordres de fabrication est pris en compte :</span><span class="sxs-lookup"><span data-stu-id="aa711-130">For example, warehouse activities have an impact, and the status of sales, purchase, transfer, assembly, and production orders is taken into account:</span></span>  
  
1. <span data-ttu-id="aa711-131">En partie géré (flexibilité de planification = Aucune)</span><span class="sxs-lookup"><span data-stu-id="aa711-131">Partly handled (Planning Flexibility = None)</span></span>  
2. <span data-ttu-id="aa711-132">Déjà en cours de traitement dans l'entrepôt (Flexibilité planification = Aucune)</span><span class="sxs-lookup"><span data-stu-id="aa711-132">Already in process in the warehouse (Planning Flexibility = None)</span></span>  
3. <span data-ttu-id="aa711-133">Lancé - tous types de commande (flexibilité de planification = illimitée)</span><span class="sxs-lookup"><span data-stu-id="aa711-133">Released – all order types (Planning Flexibility = Unlimited)</span></span>  
4. <span data-ttu-id="aa711-134">Ordre de fabrication planifié ferme (flexibilité de planification = illimitée)</span><span class="sxs-lookup"><span data-stu-id="aa711-134">Firm Planned Production Order (Planning Flexibility = Unlimited)</span></span>  
5. <span data-ttu-id="aa711-135">Planifié/ouvert - tous types de commande (flexibilité de planification = illimitée)</span><span class="sxs-lookup"><span data-stu-id="aa711-135">Planned/Open – all order types (Planning Flexibility = Unlimited)</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="aa711-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="aa711-136">See Also</span></span>  
<span data-ttu-id="aa711-137">[Détails de conception : équilibrage de la demande et de l'approvisionnement](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="aa711-137">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
<span data-ttu-id="aa711-138">[Détails de conception : concepts centraux du système de planification](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="aa711-138">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
[<span data-ttu-id="aa711-139">Détails de conception : planification de l'approvisionnement</span><span class="sxs-lookup"><span data-stu-id="aa711-139">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)