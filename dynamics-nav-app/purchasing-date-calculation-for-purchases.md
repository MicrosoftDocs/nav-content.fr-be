---
title: Calcul de la date des achats
description: "Le programme calcule automatiquement la date à laquelle vous devez commander un article pour l'avoir en stock à une certaine date. Il s'agit de la date à laquelle des articles commandés à une date donnée devraient être disponibles pour le prélèvement."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/10/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3f3f87311f0971b2901852a9aa0c766c6c806190
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="date-calculation-for-purchases"></a><span data-ttu-id="42204-104">Calcul de la date des achats</span><span class="sxs-lookup"><span data-stu-id="42204-104">Date Calculation for Purchases</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="42204-105"> calcule automatiquement la date à laquelle vous devez commander un article pour l'avoir en stock à une certaine date.</span><span class="sxs-lookup"><span data-stu-id="42204-105"> automatically calculates the date on which you must order an item to have it in inventory on a certain date.</span></span> <span data-ttu-id="42204-106">Il s'agit de la date à laquelle des articles commandés à une date donnée devraient être disponibles pour le prélèvement.</span><span class="sxs-lookup"><span data-stu-id="42204-106">This is the date on which you can expect items ordered on a particular date to be available for picking.</span></span>  

<span data-ttu-id="42204-107">Si vous saisissez une date de réception souhaitée sur un en-tête de commande achat, la date de commande calculée est la date à laquelle la commande doit être passée pour recevoir les articles à la date que vous avez demandée.</span><span class="sxs-lookup"><span data-stu-id="42204-107">If you specify a requested receipt date on a purchase order header, then the calculated order date is the date on which the order must be placed to receive the items on the date that you requested.</span></span> <span data-ttu-id="42204-108">Ensuite, la date à laquelle les articles peuvent être prélevés est calculée et saisie dans le champ **Date réception prévue**.</span><span class="sxs-lookup"><span data-stu-id="42204-108">Then, the date on which the items are available for picking is calculated and entered in the **Expected Receipt Date** field.</span></span>  

<span data-ttu-id="42204-109">Si vous n'indiquez aucune date réception demandée, le programme utilise la date commande de la ligne comme point de départ pour le calcul de la date à laquelle vous souhaitez recevoir les articles et la date disponibilité des articles pour leur prélèvement.</span><span class="sxs-lookup"><span data-stu-id="42204-109">If you do not specify a requested receipt date, then the order date on the line is used as the starting point for calculating the date on which you can expect to receive the items and the date on which the items are available for picking.</span></span>  

## <a name="calculating-with-a-requested-receipt-date"></a><span data-ttu-id="42204-110">Calcul avec une date réception demandée</span><span class="sxs-lookup"><span data-stu-id="42204-110">Calculating with a Requested Receipt Date</span></span>  
<span data-ttu-id="42204-111">Si la ligne commande achat indique une date réception demandée, le programme l'utilise comme point de départ pour les calculs suivants :</span><span class="sxs-lookup"><span data-stu-id="42204-111">If there is a requested receipt date on the purchase order line, then that date is used as the starting point for the following calculations.</span></span>  

- <span data-ttu-id="42204-112">date réception demandée - délai réapprovisionnement = date commande</span><span class="sxs-lookup"><span data-stu-id="42204-112">requested receipt date - lead time calculation = order date</span></span>  
- <span data-ttu-id="42204-113">date réception demandée + délai enlogement + délai sécurité = date réception prévue</span><span class="sxs-lookup"><span data-stu-id="42204-113">requested receipt date + inbound whse. handling time + safety lead time = expected receipt date</span></span>  

<span data-ttu-id="42204-114">Si vous indiquez une date réception demandée sur l'en-tête commande achat, le programme la copie dans le champ correspondant sur toutes les lignes.</span><span class="sxs-lookup"><span data-stu-id="42204-114">If you entered a requested receipt date on the purchase order header, then that date is copied to the corresponding field on all the lines.</span></span> <span data-ttu-id="42204-115">Vous pouvez modifier ou supprimer cette date sur n'importe quelle ligne.</span><span class="sxs-lookup"><span data-stu-id="42204-115">You can change this date on any of the lines, or you can remove the date on the line.</span></span>  

## <a name="calculating-without-a-requested-delivery-date"></a><span data-ttu-id="42204-116">Calcul sans date livraison demandée</span><span class="sxs-lookup"><span data-stu-id="42204-116">Calculating without a Requested Delivery Date</span></span>  
<span data-ttu-id="42204-117">Si vous indiquez une ligne commande achat sans date livraison demandée, le champ **Date commande** sur la ligne est renseigné avec la date du champ **Date commande** sur l'en\-tête commande achat.</span><span class="sxs-lookup"><span data-stu-id="42204-117">If you enter a purchase order line without a requested delivery date, then the **Order Date** field on the line is filled with the date in the **Order Date** field on the purchase order header.</span></span> <span data-ttu-id="42204-118">Il s'agit de la date que vous avez indiquée ou de la date de travail.</span><span class="sxs-lookup"><span data-stu-id="42204-118">This is either the date that you entered or the work date.</span></span> <span data-ttu-id="42204-119">Le programme calcule ensuite les dates suivantes pour la ligne commande achat en utilisant comme point de départ la date commande.</span><span class="sxs-lookup"><span data-stu-id="42204-119">The following dates are then calculated for the purchase order line, with the order date as the starting point.</span></span>  

- <span data-ttu-id="42204-120">date commande + délai réapprovisionnement = date livraison fourn. prévue</span><span class="sxs-lookup"><span data-stu-id="42204-120">order date + lead time calculation = planned receipt date</span></span>  
- <span data-ttu-id="42204-121">date livraison fourn. prévue + délai enlogement + délai sécurité = date réception prévue</span><span class="sxs-lookup"><span data-stu-id="42204-121">planned receipt date + inbound whse. handling time + safety lead time = expected receipt date</span></span>  

<span data-ttu-id="42204-122">Si vous modifiez la date commande sur la ligne, par exemple lorsque des articles ne sont pas disponibles auprès de votre fournisseur avant une date ultérieure, le programme recalcule automatiquement les dates appropriées sur les lignes.</span><span class="sxs-lookup"><span data-stu-id="42204-122">If you change the order date on the line, such as when items are not available at your vendor until a later date, then the relevant dates on the line are automatically recalculated.</span></span>  

<span data-ttu-id="42204-123">Si vous modifiez la date commande sur l'en\-tête, celle\-ci est copiée dans le champ **Date commande** sur toutes les lignes et tous les champs date qui y sont liés sont recalculés.</span><span class="sxs-lookup"><span data-stu-id="42204-123">If you change the order date on the header, then that date is copied to the **Order Date** field on all the lines, and all the related date fields are then recalculated.</span></span>  

## <a name="see-also"></a><span data-ttu-id="42204-124">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="42204-124">See Also</span></span>  
 <span data-ttu-id="42204-125">[Calcul de la date des ventes](sales-date-calculation-for-sales.md) </span><span class="sxs-lookup"><span data-stu-id="42204-125">[Date Calculation for Sales](sales-date-calculation-for-sales.md) </span></span>  
 [<span data-ttu-id="42204-126">Comment calculer des dates promesse livraison</span><span class="sxs-lookup"><span data-stu-id="42204-126">How to: Calculate Order Promising Dates</span></span>](sales-how-to-calculate-order-promising-dates.md)  
 <span data-ttu-id="42204-127">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="42204-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
