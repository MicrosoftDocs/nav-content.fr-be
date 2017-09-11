---
title: "Spécifier la sélection de l'imprimante pour les états"
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 56a5c1428651162293e56d71e2369fe55d291594
ms.contentlocale: fr-be
ms.lasthandoff: 07/19/2017

---
    
# <a name="specify-printer-selection-for-reports"></a><span data-ttu-id="e072a-102">Spécifier la sélection de l'imprimante pour les états</span><span class="sxs-lookup"><span data-stu-id="e072a-102">Specify Printer Selection for Reports</span></span>
<span data-ttu-id="e072a-103">Vous pouvez configurer les états de sorte qu'ils soient imprimés sur une imprimante spécifique.</span><span class="sxs-lookup"><span data-stu-id="e072a-103">You can set up reports so that they must be printed on a specific printer.</span></span> <span data-ttu-id="e072a-104">Voici quelques exemples de sélections d'imprimante :</span><span class="sxs-lookup"><span data-stu-id="e072a-104">The following are some uses of printer selection:</span></span> 

- <span data-ttu-id="e072a-105">Vous pouvez imprimer des états sur un en-tête de la société.</span><span class="sxs-lookup"><span data-stu-id="e072a-105">You can print reports on special company letterhead.</span></span>
- <span data-ttu-id="e072a-106">Vous pouvez imprimer des états sur des formats de papier différents.</span><span class="sxs-lookup"><span data-stu-id="e072a-106">You can print reports on different paper sizes.</span></span>
- <span data-ttu-id="e072a-107">Vous pouvez imprimer des états sur l'imprimante par défaut d'un employé spécifié.</span><span class="sxs-lookup"><span data-stu-id="e072a-107">You can print reports on the default printer of a specified employee.</span></span>

<span data-ttu-id="e072a-108">La fenêtre **Sélections d'imprimantes** pour définir différentes valeurs afin d'obtenir des sorties différentes.</span><span class="sxs-lookup"><span data-stu-id="e072a-108">You use the **Printer Selections** window to set different values to obtain different output.</span></span> <span data-ttu-id="e072a-109">Si vous configurez une sélection d'imprimante spécifique, cette sélection a priorité sur une sélection d'imprimante plus générale.</span><span class="sxs-lookup"><span data-stu-id="e072a-109">If you set a specific printer selection, then it takes precedence over a more general printer selection.</span></span> <span data-ttu-id="e072a-110">Par exemple, vous pouvez configurer une sélection d'imprimante en entrant une valeur dans les champs **ID utilisateur**, **ID état** et **Nom de l'imprimante**.</span><span class="sxs-lookup"><span data-stu-id="e072a-110">For example, you can set a printer selection that has values in the **User ID**, **Report ID**, and **Printer Name** fields.</span></span> <span data-ttu-id="e072a-111">Cette sélection d'imprimante a priorité sur une sélection d'imprimante dont les champs **ID utilisateur** ou **ID état** sont vides.</span><span class="sxs-lookup"><span data-stu-id="e072a-111">This printer selection takes precedence over a printer selection that has blank entries in the **User ID** or **Report ID** fields.</span></span> 

<span data-ttu-id="e072a-112">Le tableau suivant décrit les combinaisons de valeurs à spécifier lors de la configuration de sélections d'imprimante pour un état.</span><span class="sxs-lookup"><span data-stu-id="e072a-112">The following table describes the combination of values to specify when you set up printer selections for a report.</span></span>

|<span data-ttu-id="e072a-113">Pour</span><span class="sxs-lookup"><span data-stu-id="e072a-113">To</span></span>                                                 |<span data-ttu-id="e072a-114">Configurez les valeurs suivantes</span><span class="sxs-lookup"><span data-stu-id="e072a-114">Set the following values</span></span>                                             |
|---------------------------------------------------|---------------------------------------------------------------------|
|<span data-ttu-id="e072a-115">Imprimer un état sur une imprimante spécifique pour tous les utilisateurs</span><span class="sxs-lookup"><span data-stu-id="e072a-115">Print a report to a specific printer for all users</span></span> |<span data-ttu-id="e072a-116">Spécifiez une valeur dans les champs **ID état** et **Nom de l'imprimante** et ne renseignez pas le champ **ID utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="e072a-116">Specify values in the **Report ID** and **Printer Name** fields and leave the **User ID** field blank.</span></span>|
|<span data-ttu-id="e072a-117">Imprimer tous les états sur une imprimante spécifique pour un utilisateur spécifique</span><span class="sxs-lookup"><span data-stu-id="e072a-117">Print all reports to a specific printer for a specific user</span></span>|<span data-ttu-id="e072a-118">Spécifiez une valeur dans les champs **ID utilisateur** et **Nom de l'imprimante** et ne renseignez pas le champ **ID état**.</span><span class="sxs-lookup"><span data-stu-id="e072a-118">Specify values in the **User ID** and **Printer Name** fields and leave the **Report ID** field blank.</span></span>|
|<span data-ttu-id="e072a-119">Définir l'imprimante par défaut pour tous les états</span><span class="sxs-lookup"><span data-stu-id="e072a-119">Set the default printer for all reports</span></span>|<span data-ttu-id="e072a-120">Spécifiez une valeur dans le champ **Nom de l'imprimante** et ne renseignez pas les champs **ID utilisateur** et **ID état**.</span><span class="sxs-lookup"><span data-stu-id="e072a-120">Specify a value in the **Printer Name** field and leave the **User ID** and **Report ID** fields blank.</span></span>|
|<span data-ttu-id="e072a-121">Imprimer un état spécifique sur l'imprimante par défaut de l'utilisateur</span><span class="sxs-lookup"><span data-stu-id="e072a-121">Print a specific report to the user’s default printer</span></span>|<span data-ttu-id="e072a-122">Spécifiez une valeur dans le champ **ID état** et ne renseignez pas les champs **Nom de l'imprimante** et **ID utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="e072a-122">Specify a value in the **Report ID** field and leave the **Printer Name** and **User ID** fields blank.</span></span>|
|<span data-ttu-id="e072a-123">Imprimer un état spécifique sur une imprimante spécifique pour un utilisateur spécifique</span><span class="sxs-lookup"><span data-stu-id="e072a-123">Print a specific report to a specific printer for a specific user</span></span>|<span data-ttu-id="e072a-124">Spécifiez une valeur dans les trois champs.</span><span class="sxs-lookup"><span data-stu-id="e072a-124">Specify values in all three fields.</span></span>|

## <a name="see-also"></a><span data-ttu-id="e072a-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e072a-125">See Also</span></span>
[<span data-ttu-id="e072a-126">Utiliser Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="e072a-126">Work with Dynamics NAV</span></span>](ui-work-product.md)

