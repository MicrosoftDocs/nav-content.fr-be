---
title: Rangement d'articles
description: "L'activité entrepôt consistant à ranger les articles une fois reçus ou fabriqués s'exécute différemment selon la configuration des fonctionnalités du module Gestion d'entrepôt."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/31/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 0b68ef1b4c73eef1ac82d59587011a0fcdead096
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="putting-items-away"></a><span data-ttu-id="96801-103">Rangement des articles</span><span class="sxs-lookup"><span data-stu-id="96801-103">Putting Items Away</span></span>
<span data-ttu-id="96801-104">L'activité entrepôt consistant à ranger les articles une fois reçus ou fabriqués s'exécute différemment selon la configuration des fonctionnalités du module Gestion d'entrepôt.</span><span class="sxs-lookup"><span data-stu-id="96801-104">The warehouse activity of putting items away after they are received or output is performed in different ways depending on how warehouse management features are configured.</span></span> <span data-ttu-id="96801-105">Le niveau de complexité du paramétrage varie : aucune fonctionnalité entrepôt, configurations de stockage de base pour le traitement par commande dans une ou plusieurs activités uniquement, configurations avancées dans lesquelles toutes les activités entrepôt doivent être exécutées dans un flux suggéré.</span><span class="sxs-lookup"><span data-stu-id="96801-105">The complexity can rank from no warehouse features, through basic warehouse configurations for order-by order handling in one or more activities only, to advanced configurations where all warehouse activities must be performed in a directed workflow.</span></span> <span data-ttu-id="96801-106">Pour plus d'informations, voir [Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="96801-106">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span></span>

<span data-ttu-id="96801-107">Si vous décidez d'organiser et d'enregistrer vos informations de rangement avec des documents entrepôt, activez le champ **Rangement requis** dans la fiche magasin.</span><span class="sxs-lookup"><span data-stu-id="96801-107">If you decide that you want to organize and record put-away information with warehouse documents, you place a check mark in the **Require Put-away** field on the location card.</span></span> <span data-ttu-id="96801-108">Ceci indique à l'application que, lorsque vous avez des articles qui entrent dans l'entrepôt via un document origine entrant, vous souhaitez que le rangement de ces articles soit contrôlé par le système.</span><span class="sxs-lookup"><span data-stu-id="96801-108">This indicates that when you have items coming into the warehouse location through an inbound source document, you want the put-away of those items to be controlled by the system.</span></span> <span data-ttu-id="96801-109">Un document origine entrant peut être une commande achat, un retour vente, un enlogement transfert ou un ordre de fabrication dont la fabrication est prête à être rangée.</span><span class="sxs-lookup"><span data-stu-id="96801-109">An inbound source document can be a purchase order, a sales return order, an inbound transfer order, or a production order whose output is ready for put-away.</span></span>  

<span data-ttu-id="96801-110">Si votre magasin est configuré pour nécessiter un traitement des rangements, mais pas un traitement des réceptions, vous utilisez la fenêtre **Rangement stock** pour organiser les informations de rangement, les imprimer, entrer le résultat du rangement effectif et valider les informations de rangement, ce qui valide les informations de réception pour le document source.</span><span class="sxs-lookup"><span data-stu-id="96801-110">If your location is set up to use put-away processing but not receive processing, you use the **Inventory Put-away** window to organize the put-away information, print it, enter the result of the actual put-away and post the put-away information, which in turn posts the receipt information for the source document.</span></span> <span data-ttu-id="96801-111">En cas d'ordre de fabrication, le processus de validation valide la production de l'ordre et termine l'ordre de fabrication.</span><span class="sxs-lookup"><span data-stu-id="96801-111">In the case of a production order, the posting process posts the output of the order and finishes the production order.</span></span>

<span data-ttu-id="96801-112">Si votre magasin est configuré pour exiger à la fois le traitement des réceptions et des rangements, de sorte que vous ayez activé les deux champs **Réception requise** et **Rangement requis** dans la fiche magasin, le rangement des articles exige un processus différent.</span><span class="sxs-lookup"><span data-stu-id="96801-112">If your location is set up to require both receive and put-away processing, so that you have placed check marks in both the **Require Receive** and the **Require Put-away** field on the location card, there is a different process for putting items away.</span></span> <span data-ttu-id="96801-113">Dans ce cas, vous utilisez la fenêtre **Rangement entrepôt** pour traiter le rangement.</span><span class="sxs-lookup"><span data-stu-id="96801-113">In this case, you will use the **Warehouse Put-away** window to handle the put-away.</span></span> <span data-ttu-id="96801-114">Le rangement entrepôt fonctionne comme le rangement stock, si ce n'est qu'au lieu de valider les informations, vous enregistrez le rangement.</span><span class="sxs-lookup"><span data-stu-id="96801-114">The warehouse put-away functions similarly to the inventory put-away, except that instead of posting the information, you register the put-away.</span></span> <span data-ttu-id="96801-115">Remarquez que l'enregistrement du rangement entrepôt ne valide pas la réception des articles.</span><span class="sxs-lookup"><span data-stu-id="96801-115">Note that the registering of the warehouse put-away does not post the receipt of the items.</span></span> <span data-ttu-id="96801-116">Il met simplement à jour le contenu de l'emplacement.</span><span class="sxs-lookup"><span data-stu-id="96801-116">It merely updates the bin content.</span></span> <span data-ttu-id="96801-117">En tant qu'administrateur entrepôt, vous pouvez utiliser des feuilles rangement pour organiser les informations de rangement avant de créer des instructions de rangement entrepôt.</span><span class="sxs-lookup"><span data-stu-id="96801-117">As a warehouse manager, you can use a put-away worksheets to organize put-away information before creating the individual warehouse put-away instructions.</span></span>

<span data-ttu-id="96801-118">Le tableau suivant décrit une série de tâches et inclut des liens vers les rubriques qui les décrivent.</span><span class="sxs-lookup"><span data-stu-id="96801-118">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="96801-119">**Pour**</span><span class="sxs-lookup"><span data-stu-id="96801-119">**To**</span></span>|<span data-ttu-id="96801-120">**Voir**</span><span class="sxs-lookup"><span data-stu-id="96801-120">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="96801-121">Valider la réception d'articles directement à partir du document commande entrante et donc enregistrer le rangement, car aucune fonctionnalité entrepôt n'existe.</span><span class="sxs-lookup"><span data-stu-id="96801-121">Post the receipt of items directly from the inbound order document and thereby record the put away, because no warehouse configuration exists.</span></span>|[<span data-ttu-id="96801-122">Procédure : réceptionner des articles</span><span class="sxs-lookup"><span data-stu-id="96801-122">How to: Receive Items</span></span>](warehouse-how-receive-items.md)|  
|<span data-ttu-id="96801-123">Ranger les articles par commande et valider la réception dans la même activité dans une configuration entrepôt de base.</span><span class="sxs-lookup"><span data-stu-id="96801-123">Put items away order by order and post the receipt in the same activity, in a basic warehouse configuration.</span></span>|[<span data-ttu-id="96801-124">Comment ranger des articles avec le rangement stock</span><span class="sxs-lookup"><span data-stu-id="96801-124">How to: Put Items Away with Inventory Put-aways</span></span>](warehouse-how-to-put-items-away-with-inventory-put-aways.md)|  
|<span data-ttu-id="96801-125">Ranger les articles de plusieurs commandes dans une configuration entrepôt avancée.</span><span class="sxs-lookup"><span data-stu-id="96801-125">Put items away for multiple orders in an advanced warehouse configuration.</span></span>|[<span data-ttu-id="96801-126">Comment ranger des articles avec le rangement entrepôt</span><span class="sxs-lookup"><span data-stu-id="96801-126">How to: Put Items Away with Warehouse Put-aways</span></span>](warehouse-how-to-put-items-away-with-warehouse-put-aways.md)|  
|<span data-ttu-id="96801-127">Ranger les articles fabriqués ou assemblés dans une configuration de stockage de base ou avancée.</span><span class="sxs-lookup"><span data-stu-id="96801-127">Put produced or assembled items away in a basic or an advanced warehouse configuration.</span></span>|[<span data-ttu-id="96801-128">Procédure : rangement du résultat de fabrication ou d'assemblage</span><span class="sxs-lookup"><span data-stu-id="96801-128">How to: Put Away Production or Assembly Output</span></span>](warehouse-how-to-put-away-production-output.md)|
|<span data-ttu-id="96801-129">Planifier des instructions de rangement optimisées pour plusieurs réceptions entrepôt validées. Dans ce cas, les magasiniers n'ont pas à agir directement sur les réceptions.</span><span class="sxs-lookup"><span data-stu-id="96801-129">Plan optimized put-away instructions for a number of posted warehouse receipts rather than have warehouse workers act directly on receipts.</span></span>|[<span data-ttu-id="96801-130">Comment planifier des rangements dans la feuille</span><span class="sxs-lookup"><span data-stu-id="96801-130">How to: Plan Put-aways in Worksheets</span></span>](warehouse-how-to-plan-put-aways-in-worksheets.md)|  
|<span data-ttu-id="96801-131">Replacer les articles prélevés techniquement à l'aide d'un prélèvement interne, par exemple dans le cadre d'un ordre de fabrication pour lequel la quantité prévue n'a pas été consommée.</span><span class="sxs-lookup"><span data-stu-id="96801-131">Put back items that were picked technically with an internal pick, for example for a production order that did not consume the expected quantity.</span></span>|[<span data-ttu-id="96801-132">Procédure : Prélever et ranger sans document origine</span><span class="sxs-lookup"><span data-stu-id="96801-132">How to: Pick and Put Away Without a Source Document</span></span>](warehouse-how-to-create-put-aways-from-internal-put-aways.md)|
|<span data-ttu-id="96801-133">Répartir une ligne rangement pour placer une partie de la quantité rangée dans les emplacements disponibles en raison du remplissage de l'emplacement désigné.</span><span class="sxs-lookup"><span data-stu-id="96801-133">Split a put-away line to place part of the put-away quantity in available bins because the designated bin is filled up.</span></span>|[<span data-ttu-id="96801-134">Procédure : répartir des lignes activité entrepôt</span><span class="sxs-lookup"><span data-stu-id="96801-134">How to: Split Warehouse Activity Lines</span></span>](warehouse-how-to-split-warehouse-activity-lines.md)|
|<span data-ttu-id="96801-135">Accéder immédiatement aux rangements qui vous ont été affectés en tant que magasinier.</span><span class="sxs-lookup"><span data-stu-id="96801-135">Get immediate access to put-aways that are assigned to you as a warehouse worker.</span></span>|[<span data-ttu-id="96801-136">Procédure : trouver vos affectations d'entrepôt</span><span class="sxs-lookup"><span data-stu-id="96801-136">How to: Find Your Warehouse Assignments</span></span>](warehouse-how-to-find-your-warehouse-assignments.md)|    

## <a name="see-also"></a><span data-ttu-id="96801-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="96801-137">See Also</span></span>  
[<span data-ttu-id="96801-138">Gestion d'entrepôt</span><span class="sxs-lookup"><span data-stu-id="96801-138">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="96801-139">STOCKS ET EN-COURS</span><span class="sxs-lookup"><span data-stu-id="96801-139">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="96801-140">[Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="96801-140">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="96801-141">[Gestion des assemblages](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="96801-141">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="96801-142">Détails de conception : gestion d'entrepôt</span><span class="sxs-lookup"><span data-stu-id="96801-142">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="96801-143">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="96801-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
