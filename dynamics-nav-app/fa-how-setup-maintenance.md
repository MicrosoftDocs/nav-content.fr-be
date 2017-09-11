---
title: "Procédure : configurer une maintenance d'immobilisation"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: ace0fb13d2be71c7204f16f34f6b65b54ff98230
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-fixed-asset-maintenance"></a><span data-ttu-id="0f56a-102">Procédure : configurer une maintenance d'immobilisation</span><span class="sxs-lookup"><span data-stu-id="0f56a-102">How to: Set Up Fixed Asset Maintenance</span></span>
<span data-ttu-id="0f56a-103">Pour gérer la maintenance des immobilisations, vous devez configurer tout d'abord certaines informations générales de maintenance, un compte de validation pour les coûts de maintenance et les codes de maintenance pour les types de travaux, tels que le service de routine ou la réparation.</span><span class="sxs-lookup"><span data-stu-id="0f56a-103">To manage fixed asset maintenance, you must first set up some general maintenance information, a posting account for maintenance costs, and maintenance codes for types of work, such as Routine Service or Repair.</span></span>

## <a name="to-set-up-general-maintenance-information"></a><span data-ttu-id="0f56a-104">Pour configurer les informations générales de maintenance</span><span class="sxs-lookup"><span data-stu-id="0f56a-104">To set up general maintenance information</span></span>
<span data-ttu-id="0f56a-105">Si vous configurez les champs pour la maintenance, vous pouvez valider des frais de maintenance à partir d'une feuille immobilisation.</span><span class="sxs-lookup"><span data-stu-id="0f56a-105">If you set up the fields for maintenance, you can post maintenance expenses from the fixed asset journal.</span></span>
1. <span data-ttu-id="0f56a-106">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Immobilisations**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="0f56a-106">In the top right corner, choose the **Search for Page or Report** icon, enter **Fixed Assets**, and then choose the related link.</span></span>
2. <span data-ttu-id="0f56a-107">Sélectionnez l'immobilisation pour laquelle vous souhaitez définir la couverture d'assurance, puis sélectionnez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="0f56a-107">Select the fixed asset that you to define insurance coverage for, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="0f56a-108">Sur le raccourci **Maintenance**, complétez les champs, comme nécessaire.</span><span class="sxs-lookup"><span data-stu-id="0f56a-108">On the **Maintenance** FastTab, fill in the fields as necessary.</span></span> <span data-ttu-id="0f56a-109">Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.</span><span class="sxs-lookup"><span data-stu-id="0f56a-109">Choose a field to read a short description of the field or link to more information.</span></span>

## <a name="to-set-up-maintenance-codes"></a><span data-ttu-id="0f56a-110">Pour configurer des codes maintenance</span><span class="sxs-lookup"><span data-stu-id="0f56a-110">To set up maintenance codes</span></span>  
<span data-ttu-id="0f56a-111">Lorsque vous validez des coûts de maintenance à partir d'une feuille comptabilité, vous renseignez le champ **Code maintenance** pour enregistrer le type de maintenance effectuée, telle qu'un service de routine ou une réparation.</span><span class="sxs-lookup"><span data-stu-id="0f56a-111">When you post maintenance costs from a general journal, you fill in the **Maintenance Code** field to record what kind of maintenance has been performed, such as routine service or repair.</span></span>
1. <span data-ttu-id="0f56a-112">Sinon, dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Maintenance**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="0f56a-112">In the top right corner, choose the **Search for Page or Report** icon, enter **Maintenance**, and then choose the related link.</span></span>
2. <span data-ttu-id="0f56a-113">Dans la fenêtre **Maintenance**, configurez les codes pour les différents types de travaux de maintenance.</span><span class="sxs-lookup"><span data-stu-id="0f56a-113">In the **Maintenance** window, set up codes for different types of maintenance work.</span></span>

## <a name="to-set-up-maintenance-expense-accounts"></a><span data-ttu-id="0f56a-114">Pour configurer des comptes frais de maintenance</span><span class="sxs-lookup"><span data-stu-id="0f56a-114">To set up maintenance expense accounts</span></span>  
<span data-ttu-id="0f56a-115">Pour valider les coûts de maintenance, vous devez tout d'abord saisir un numéro de compte dans la fenêtre **Groupes compta. immo**.</span><span class="sxs-lookup"><span data-stu-id="0f56a-115">To post maintenance costs, you must first enter an account number in the **FA Posting Groups** window.</span></span>
1. <span data-ttu-id="0f56a-116">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Groupes de validation immo.**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="0f56a-116">In the top right corner, choose the **Search for Page or Report** icon, enter **FA Posting Groups**, and then choose the related link.</span></span>
2. <span data-ttu-id="0f56a-117">Renseignez le champ **Compte frais maintenance** pour chaque groupe comptabilisation.</span><span class="sxs-lookup"><span data-stu-id="0f56a-117">Fill in the **Maintenance Expense Account** field for each posting group.</span></span>

<span data-ttu-id="0f56a-118">**Remarque** : pour définir que les coûts de maintenance sont attribués aux départements ou projets, configurez une clé d'allocation.</span><span class="sxs-lookup"><span data-stu-id="0f56a-118">**Note**: To define that maintenance costs are allocated to departments or projects, set up an allocation keys.</span></span> <span data-ttu-id="0f56a-119">Pour en savoir plus, voir [Procédure : configurer des fonctionnalités d'immobilisations](fa-how-setup-general.md).</span><span class="sxs-lookup"><span data-stu-id="0f56a-119">For more information, see [How to: Set Up General Fixed Assets Features](fa-how-setup-general.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="0f56a-120">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0f56a-120">See Also</span></span>
[<span data-ttu-id="0f56a-121">Configurer des immobilisations</span><span class="sxs-lookup"><span data-stu-id="0f56a-121">Set Up Fixed Assets</span></span>](fa-setup.md)  
[<span data-ttu-id="0f56a-122">Gérer des immobilisations</span><span class="sxs-lookup"><span data-stu-id="0f56a-122">Manage Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="0f56a-123">Finance</span><span class="sxs-lookup"><span data-stu-id="0f56a-123">Finance</span></span>](finance-setup.md)  
[<span data-ttu-id="0f56a-124">Bienvenue dans Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="0f56a-124">Welcome to Dynamics NAV</span></span>](across-get-started.md)

