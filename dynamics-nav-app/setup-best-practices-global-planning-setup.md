---
title: "Pratiques recommandées pour la configuration du planning général"
description: "Le raccourci **Planning** de la fenêtre **Paramètres production** comporte plusieurs champs permettant de définir les règles globales pour la planification des approvisionnements."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: d851626e2a107f7f5857fc81013ea0c16d209cca
ms.contentlocale: fr-be
ms.lasthandoff: 12/01/2017

---
# <a name="setup-best-practices-global-planning-setup"></a><span data-ttu-id="e5d62-103">Configurer des recommandations : configuration du planning général</span><span class="sxs-lookup"><span data-stu-id="e5d62-103">Setup Best Practices: Global Planning Setup</span></span>
<span data-ttu-id="e5d62-104">Le raccourci **Planning** de la fenêtre**Paramètres production** comporte plusieurs champs permettant de définir les règles globales pour la planification des approvisionnements.</span><span class="sxs-lookup"><span data-stu-id="e5d62-104">The **Planning** FastTab in the **Manufacturing Setup** window contains several fields that define global rules for supply planning.</span></span>  

 <span data-ttu-id="e5d62-105">Le tableau suivant fournit les meilleures pratiques sur la procédure de configuration de champs paramètres sélectionnés de planification générale.</span><span class="sxs-lookup"><span data-stu-id="e5d62-105">The following table provides best practices on how to set up selected global planning parameter fields.</span></span> <span data-ttu-id="e5d62-106">Pour plus d'informations sur un champ donné, sélectionnez le lien correspondant dans la colonne **Configuration d'un champ**.</span><span class="sxs-lookup"><span data-stu-id="e5d62-106">For more information about a field, choose the link in the **Setup field** column.</span></span>  

|<span data-ttu-id="e5d62-107">Paramétrage de champ</span><span class="sxs-lookup"><span data-stu-id="e5d62-107">Setup field</span></span>|<span data-ttu-id="e5d62-108">Meilleure pratique</span><span class="sxs-lookup"><span data-stu-id="e5d62-108">Best practice</span></span>|<span data-ttu-id="e5d62-109">Commentaire</span><span class="sxs-lookup"><span data-stu-id="e5d62-109">Comment</span></span>|  
|-----------------|-------------------|-------------|  
|<span data-ttu-id="e5d62-110">Prévision sur magasin</span><span class="sxs-lookup"><span data-stu-id="e5d62-110">Use Forecast on Locations</span></span>|<span data-ttu-id="e5d62-111">Indiquez si vous avez des prévisions pour des entrepôts spécifiques.</span><span class="sxs-lookup"><span data-stu-id="e5d62-111">Select if you have forecasts for specific locations.</span></span>||  
|<span data-ttu-id="e5d62-112">Mag. composant par déf.</span><span class="sxs-lookup"><span data-stu-id="e5d62-112">Components at Location</span></span>|<span data-ttu-id="e5d62-113">Si les articles ne sont pas définis comme points de stock, sélectionnez le code magasin de l'entrepôt principal.</span><span class="sxs-lookup"><span data-stu-id="e5d62-113">If items are not defined as SKUs, select the location code of your main warehouse.</span></span>|<span data-ttu-id="e5d62-114">Cela s'applique également si vous utilisez uniquement la demande achat.</span><span class="sxs-lookup"><span data-stu-id="e5d62-114">This also applies if you only use the requisition worksheet.</span></span>|  
|<span data-ttu-id="e5d62-115">Niveau de dépassement de capacité vide</span><span class="sxs-lookup"><span data-stu-id="e5d62-115">Blank Overflow Level</span></span>|<span data-ttu-id="e5d62-116">Sélectionnez **Autoriser calcul par défaut** si vous effectuez une migration de Microsoft Dynamics NAV 5.0 ou d'une version antérieure.</span><span class="sxs-lookup"><span data-stu-id="e5d62-116">Select **Allow Default Calculation** if you are migrating from Microsoft Dynamics NAV 5.0 or earlier.</span></span>|<span data-ttu-id="e5d62-117">Ne l'utilisez que si vous souhaitez autoriser tout ou partie de vos articles à franchir le point de réapprovisionnement.</span><span class="sxs-lookup"><span data-stu-id="e5d62-117">Use only if you want to allow all or some of your items to overflow the reorder point.</span></span>|  
|<span data-ttu-id="e5d62-118">Période tampon par défaut</span><span class="sxs-lookup"><span data-stu-id="e5d62-118">Default Dampener Period</span></span>|<span data-ttu-id="e5d62-119">Doit être compris entre 1D et 5D.</span><span class="sxs-lookup"><span data-stu-id="e5d62-119">Set between 1D and 5D.</span></span><br /><br /> <span data-ttu-id="e5d62-120">Si vous débutez en planification avec [!INCLUDE[d365fin](includes/d365fin_md.md)], définissez une plus longue période.</span><span class="sxs-lookup"><span data-stu-id="e5d62-120">If new to planning in [!INCLUDE[d365fin](includes/d365fin_md.md)], then set a longer period.</span></span>|<span data-ttu-id="e5d62-121">Quand les utilisateurs sont plus au fait des différents motifs des messages d'action, raccourcissez la période tampon pour autoriser plus de propositions de modification.</span><span class="sxs-lookup"><span data-stu-id="e5d62-121">When users are more familiar with the different reasons for action messages, then shorten the dampener period to allow more change suggestions.</span></span>|  
|<span data-ttu-id="e5d62-122">Quantité tampon par défaut</span><span class="sxs-lookup"><span data-stu-id="e5d62-122">Default Dampener Quantity</span></span>|<span data-ttu-id="e5d62-123">Définissez à entre 5 et 20 % de la taille du lot de l'article.</span><span class="sxs-lookup"><span data-stu-id="e5d62-123">Set between 5 and 20 percent of the item’s lot size.</span></span>||  

## <a name="see-also"></a><span data-ttu-id="e5d62-124">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e5d62-124">See Also</span></span>  
 <span data-ttu-id="e5d62-125">[Pratiques de configuration recommandées : planification de l'approvisionnement](setup-best-practices-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="e5d62-125">[Setup Best Practices: Supply Planning](setup-best-practices-supply-planning.md) </span></span>  
 <span data-ttu-id="e5d62-126">[Détails de conception : planification de l'approvisionnement](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="e5d62-126">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
 [<span data-ttu-id="e5d62-127">Configurer les modules complexes à l'aide des meilleures pratiques</span><span class="sxs-lookup"><span data-stu-id="e5d62-127">Set Up Complex Application Areas Using Best Practices</span></span>](set-up-complex-application-areas-using-best-practices.md)  
 <span data-ttu-id="e5d62-128">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e5d62-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

