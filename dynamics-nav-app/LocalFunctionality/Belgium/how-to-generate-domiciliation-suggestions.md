---
title: "Comment générer des propositions de domiciliation"
description: "Après avoir configuré des domiciliations, vous pouvez commencer à générer des propositions de domiciliation. Dans [!INCLUDE[navnow](../../includes/navnow_md.md)], vous pouvez uniquement créer des propositions de domiciliation pour des clients nationaux."
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
ms.openlocfilehash: 67e68d1e36cf5c3f480285203df33a8a3f386940
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-generate-domiciliation-suggestions"></a><span data-ttu-id="058f7-104">Comment générer des propositions de domiciliation</span><span class="sxs-lookup"><span data-stu-id="058f7-104">How to: Generate Domiciliation Suggestions</span></span>
<span data-ttu-id="058f7-105">Après avoir configuré des domiciliations, vous pouvez commencer à générer des propositions de domiciliation.</span><span class="sxs-lookup"><span data-stu-id="058f7-105">After you have set up domiciliations, you can start generating domiciliation suggestions.</span></span> <span data-ttu-id="058f7-106">Dans [!INCLUDE[navnow](../../includes/navnow_md.md)], vous pouvez uniquement créer des propositions de domiciliation pour des clients nationaux.</span><span class="sxs-lookup"><span data-stu-id="058f7-106">In [!INCLUDE[navnow](../../includes/navnow_md.md)], you can only create domiciliation suggestions for domestic customers.</span></span>  
  
### <a name="to-generate-domiciliation-suggestions"></a><span data-ttu-id="058f7-107">Pour générer des propositions de domiciliation</span><span class="sxs-lookup"><span data-stu-id="058f7-107">To generate domiciliation suggestions</span></span>  
  
1.  <span data-ttu-id="058f7-108">Sélectionnez l'icône ![Rechercher une page ou un état](media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Feuille saisie domiciliation**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="058f7-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Domiciliation Journal**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="058f7-109">Dans le champs **Nom feuille**, sélectionnez la feuille concernée, puis, sous l'onglet **Accueil**, dans le groupe **Progression**, sélectionnez **Proposer domiciliations**.</span><span class="sxs-lookup"><span data-stu-id="058f7-109">In the **Batch Name** field, select the required journal batch, and on the **Home** tab, in the **Progress** group, choose **Suggest Domiciliations**.</span></span>  
  
3.  <span data-ttu-id="058f7-110">Dans le raccourci **Options**, remplissez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="058f7-110">On the **Options** FastTab, fill in the fields as displayed in the following table.</span></span>  
  
    |<span data-ttu-id="058f7-111">Champ</span><span class="sxs-lookup"><span data-stu-id="058f7-111">Field</span></span>|<span data-ttu-id="058f7-112">Description</span><span class="sxs-lookup"><span data-stu-id="058f7-112">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="058f7-113">**Date besoin**</span><span class="sxs-lookup"><span data-stu-id="058f7-113">**Due Date**</span></span>|<span data-ttu-id="058f7-114">Entrez la date d'échéance à inclure dans le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="058f7-114">Enter the due date to be included in the batch job.</span></span> <span data-ttu-id="058f7-115">Seules les écritures ayant une date d'échéance antérieure ou identique à cette date seront incluses.</span><span class="sxs-lookup"><span data-stu-id="058f7-115">Only entries that have a due date before or on this date will be included.</span></span>|  
    |<span data-ttu-id="058f7-116">**Obtenir escomptes**</span><span class="sxs-lookup"><span data-stu-id="058f7-116">**Take Payment Discounts**</span></span>|<span data-ttu-id="058f7-117">Sélectionnez si vous souhaitez que le traitement par lots comprenne les écritures comptables client pour lesquelles vous pouvez obtenir un escompte.</span><span class="sxs-lookup"><span data-stu-id="058f7-117">Select if you want the batch job to include customer ledger entries for which you can receive a payment discount.</span></span>|  
    |<span data-ttu-id="058f7-118">**Date d'escompte**</span><span class="sxs-lookup"><span data-stu-id="058f7-118">**Payment Discount Date**</span></span>|<span data-ttu-id="058f7-119">Entrez la date qui sera utilisée pour calculer l'escompte.</span><span class="sxs-lookup"><span data-stu-id="058f7-119">Enter the date that will be used to calculate the payment discount.</span></span>|  
    |<span data-ttu-id="058f7-120">**Inclure remboursements poss.**</span><span class="sxs-lookup"><span data-stu-id="058f7-120">**Select Possible Refunds**</span></span>|<span data-ttu-id="058f7-121">Sélectionnez si vous souhaitez que le traitement par lots inclue les remboursements.</span><span class="sxs-lookup"><span data-stu-id="058f7-121">Select if you want the batch job to include refunds.</span></span>|  
    |<span data-ttu-id="058f7-122">**Date comptabilisation**</span><span class="sxs-lookup"><span data-stu-id="058f7-122">**Posting Date**</span></span>|<span data-ttu-id="058f7-123">Entrez la date qui apparaîtra comme date de validation sur les lignes que le traitement par lots insère dans la feuille domiciliation.</span><span class="sxs-lookup"><span data-stu-id="058f7-123">Enter the date that will appear as the posting date on the lines that the batch job inserts in the domiciliation journal.</span></span>|  
  
4.  <span data-ttu-id="058f7-124">Dans le raccourci **Client**, entrez les éventuels critères de filtre supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="058f7-124">On the **Customer** FastTab, enter any additional filter criteria.</span></span>  
  
5.  <span data-ttu-id="058f7-125">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="058f7-125">Choose the **OK** button.</span></span>  
  
     <span data-ttu-id="058f7-126">Lorsque le traitement par lots est terminé, la feuille domiciliation contient toutes les écritures comptables client ouvertes qui correspondent aux filtres.</span><span class="sxs-lookup"><span data-stu-id="058f7-126">When the batch job is finished, the domiciliation journal contains all open customer ledger entries that match the filters.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="058f7-127">Les propositions de domiciliation incluront uniquement les clients qui ont un numéro de domiciliation configuré.</span><span class="sxs-lookup"><span data-stu-id="058f7-127">The domiciliation suggestions will only include customers who have a Domiciliation number set up.</span></span> <span data-ttu-id="058f7-128">Pour plus d'informations, voir [Comment configurer des domiciliations](how-to-set-up-domiciliations.md).</span><span class="sxs-lookup"><span data-stu-id="058f7-128">For more information, see [How to: Set Up Domiciliations](how-to-set-up-domiciliations.md).</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="058f7-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="058f7-129">See Also</span></span>  
 <span data-ttu-id="058f7-130">[Banque électronique belge](belgian-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="058f7-130">[Belgian Electronic Banking](belgian-electronic-banking.md) </span></span>  
 <span data-ttu-id="058f7-131">[Domiciliation européenne](direct-debit-using-domiciliation.md) </span><span class="sxs-lookup"><span data-stu-id="058f7-131">[Direct Debit Using Domiciliation](direct-debit-using-domiciliation.md) </span></span>  
 <span data-ttu-id="058f7-132">[Comment configurer des domiciliations](how-to-set-up-domiciliations.md) </span><span class="sxs-lookup"><span data-stu-id="058f7-132">[How to: Set Up Domiciliations](how-to-set-up-domiciliations.md) </span></span>  
 <span data-ttu-id="058f7-133">[Comment tester les domiciliations](how-to-test-domiciliations.md) </span><span class="sxs-lookup"><span data-stu-id="058f7-133">[How to: Test Domiciliations](how-to-test-domiciliations.md) </span></span>  
 <span data-ttu-id="058f7-134">[Comment modifier et supprimer des lignes domiciliation](how-to-edit-and-delete-domiciliation-lines.md) </span><span class="sxs-lookup"><span data-stu-id="058f7-134">[How to: Edit and Delete Domiciliation Lines](how-to-edit-and-delete-domiciliation-lines.md) </span></span>  
 [<span data-ttu-id="058f7-135">Comment exporter et valider des domiciliations</span><span class="sxs-lookup"><span data-stu-id="058f7-135">How to: Export and Post Domiciliations</span></span>](how-to-export-and-post-domiciliations.md)
