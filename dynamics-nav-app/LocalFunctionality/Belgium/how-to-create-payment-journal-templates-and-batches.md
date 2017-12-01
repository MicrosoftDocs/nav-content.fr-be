---
title: "Comment créer des modèles et lots feuille paiement"
description: "Dans [!INCLUDE[navnow](../../includes/navnow_md.md)], des propositions de paiement sont générées et validées dans les feuilles paiement. La structure de la feuille paiement est semblable à celle des autres types de feuilles."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 13d9aaf1187e4b5da3f4482ad50b45949a1486d2
ms.contentlocale: fr-be
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-create-payment-journal-templates-and-batches"></a><span data-ttu-id="9d43f-104">Comment créer des modèles et lots feuille paiement</span><span class="sxs-lookup"><span data-stu-id="9d43f-104">How to: Create Payment Journal Templates and Batches</span></span>
<span data-ttu-id="9d43f-105">Dans [!INCLUDE[navnow](../../includes/navnow_md.md)], des propositions de paiement sont générées et validées dans les feuilles paiement.</span><span class="sxs-lookup"><span data-stu-id="9d43f-105">In [!INCLUDE[navnow](../../includes/navnow_md.md)], payment suggestions are generated and posted in payment journals.</span></span> <span data-ttu-id="9d43f-106">La structure de la feuille paiement est semblable à celle des autres types de feuilles.</span><span class="sxs-lookup"><span data-stu-id="9d43f-106">The structure of the payment journal is similar to the structure of other journal types.</span></span> <span data-ttu-id="9d43f-107">Toutefois, la feuille paiement contient des champs spécifiques au traitement des paiements.</span><span class="sxs-lookup"><span data-stu-id="9d43f-107">However, the payment journal contains some fields that are specific for processing payments.</span></span> <span data-ttu-id="9d43f-108">Avant de pouvoir commencer à générer des propositions de paiement, vous devez configurer un modèle feuille paiement et un nom feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="9d43f-108">Before you can start generating payment suggestions, you have to set up a payment journal template and a payment journal batch.</span></span>  

<span data-ttu-id="9d43f-109">Si vous attribuez un compte bancaire au modèle feuille paiement, le compte bancaire sera inséré dans tous les noms feuille paiement et toutes les lignes feuille paiement créés à l'aide de ce modèle.</span><span class="sxs-lookup"><span data-stu-id="9d43f-109">If you assign a bank account to the payment journal template, the bank account will be inserted on all payment journal batches and payment journal lines that are created by using this template.</span></span> <span data-ttu-id="9d43f-110">En indiquant un compte bancaire pour le modèle feuille, vous pouvez réduire le délai de vérification des propositions de paiement.</span><span class="sxs-lookup"><span data-stu-id="9d43f-110">By specifying a bank account for the journal template, you can reduce the time that is required for checking the payment suggestions.</span></span>  

## <a name="to-create-a-payment-journal-template"></a><span data-ttu-id="9d43f-111">Pour créer un modèle feuille paiement</span><span class="sxs-lookup"><span data-stu-id="9d43f-111">To create a payment journal template</span></span>  

1.  <span data-ttu-id="9d43f-112">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Modèles FS paiements**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="9d43f-112">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journal Templates**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="9d43f-113">Choisissez l'action **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="9d43f-113">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="9d43f-114">Dans la fenêtre **Modèles FS paiements EB**, renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="9d43f-114">In the **EB Payment Journal Templates** window, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="9d43f-115">Champ</span><span class="sxs-lookup"><span data-stu-id="9d43f-115">Field</span></span>|<span data-ttu-id="9d43f-116">Description</span><span class="sxs-lookup"><span data-stu-id="9d43f-116">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="9d43f-117">**Nom**</span><span class="sxs-lookup"><span data-stu-id="9d43f-117">**Name**</span></span>|<span data-ttu-id="9d43f-118">Entrez le nom unique du modèle feuille paiement que vous créez.</span><span class="sxs-lookup"><span data-stu-id="9d43f-118">Enter the unique name for the payment journal template that you are creating.</span></span>|  
    |<span data-ttu-id="9d43f-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="9d43f-119">**Description**</span></span>|<span data-ttu-id="9d43f-120">Entrez une description du modèle feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="9d43f-120">Enter a description of the payment journal template.</span></span>|  
    |<span data-ttu-id="9d43f-121">**Compte bancaire**</span><span class="sxs-lookup"><span data-stu-id="9d43f-121">**Bank Account**</span></span>|<span data-ttu-id="9d43f-122">Sélectionnez le compte bancaire qui sera utilisé lorsque vous créerez une proposition de paiement.</span><span class="sxs-lookup"><span data-stu-id="9d43f-122">Select the bank account that will be used when you create a payment suggestion.</span></span>|  
    |<span data-ttu-id="9d43f-123">**Code motif**</span><span class="sxs-lookup"><span data-stu-id="9d43f-123">**Reason Code**</span></span>|<span data-ttu-id="9d43f-124">Sélectionnez le code motif qui sera utilisé sur tous les noms et lignes feuille créés à l'aide du modèle feuille.</span><span class="sxs-lookup"><span data-stu-id="9d43f-124">Select the reason code that will be used on all the journal batches and lines that are created by using the journal template.</span></span> <span data-ttu-id="9d43f-125">Si vous souhaitez utiliser un autre code motif sur une ligne feuille, vous pouvez le modifier manuellement.</span><span class="sxs-lookup"><span data-stu-id="9d43f-125">If you want to use a different reason code on a journal line, you can manually change it.</span></span>|  
    |<span data-ttu-id="9d43f-126">**Code journal**</span><span class="sxs-lookup"><span data-stu-id="9d43f-126">**Source Code**</span></span>|<span data-ttu-id="9d43f-127">Sélectionnez le code source qui sera utilisé sur tous les noms et lignes feuille créés à l'aide du modèle feuille.</span><span class="sxs-lookup"><span data-stu-id="9d43f-127">Select the source code that will be used on all the journal batches and lines that are created by using the journal template.</span></span>|  

4.  <span data-ttu-id="9d43f-128">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="9d43f-128">Choose the **OK** button.</span></span>  

## <a name="to-add-payment-journal-batches-to-the-journal-template"></a><span data-ttu-id="9d43f-129">Pour ajouter des noms feuille paiement au modèle feuille</span><span class="sxs-lookup"><span data-stu-id="9d43f-129">To add payment journal batches to the journal template</span></span>  

1.  <span data-ttu-id="9d43f-130">Dans la fenêtre **Modèles FS paiements**, choisissez l'action **Noms feuilles**.</span><span class="sxs-lookup"><span data-stu-id="9d43f-130">In the **Payment Journal Templates** window, choose the **Batches** action.</span></span>  
2.  <span data-ttu-id="9d43f-131">Dans la fenêtre **Nom FS paiements**, renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="9d43f-131">In the **Paym. Journal Batch** window, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="9d43f-132">Champ</span><span class="sxs-lookup"><span data-stu-id="9d43f-132">Field</span></span>|<span data-ttu-id="9d43f-133">Description</span><span class="sxs-lookup"><span data-stu-id="9d43f-133">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="9d43f-134">**Nom modèle feuille**</span><span class="sxs-lookup"><span data-stu-id="9d43f-134">**Journal Template Name**</span></span>|<span data-ttu-id="9d43f-135">Spécifiez un nom de modèle feuille pour le nom feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="9d43f-135">Specify a journal template name for the payment journal batch.</span></span>|  
    |<span data-ttu-id="9d43f-136">**Nom**</span><span class="sxs-lookup"><span data-stu-id="9d43f-136">**Name**</span></span>|<span data-ttu-id="9d43f-137">Entrez un nom unique pour le nom feuille.</span><span class="sxs-lookup"><span data-stu-id="9d43f-137">Enter a unique name for the journal batch.</span></span><br /><br /> <span data-ttu-id="9d43f-138">**NOTE :** pour que le nom feuille se mette à jour de façon numérique, ajoutez un numéro dans le nom feuille.</span><span class="sxs-lookup"><span data-stu-id="9d43f-138">**NOTE:** To have the journal name update numerically, include a number in the journal batch name.</span></span> <span data-ttu-id="9d43f-139">Par exemple, à chaque validation, le nom KBC1 sera mis à jour en KBC2, KBC3, etc.</span><span class="sxs-lookup"><span data-stu-id="9d43f-139">For example, the name KBC1 will increment by one number with every posting to KBC2, KBC3, and so on.</span></span>|  
    |<span data-ttu-id="9d43f-140">**Description**</span><span class="sxs-lookup"><span data-stu-id="9d43f-140">**Description**</span></span>|<span data-ttu-id="9d43f-141">Entrez une description pour le nom feuille.</span><span class="sxs-lookup"><span data-stu-id="9d43f-141">Enter a description for the journal batch.</span></span>|  
    |<span data-ttu-id="9d43f-142">**Code motif**</span><span class="sxs-lookup"><span data-stu-id="9d43f-142">**Reason Code**</span></span>|<span data-ttu-id="9d43f-143">Spécifie le code motif lié à ce nom feuille.</span><span class="sxs-lookup"><span data-stu-id="9d43f-143">Specifies the reason code that is linked to this journal batch.</span></span>|  
    |<span data-ttu-id="9d43f-144">**Statut**</span><span class="sxs-lookup"><span data-stu-id="9d43f-144">**Status**</span></span>|<span data-ttu-id="9d43f-145">Indique le statut du lot.</span><span class="sxs-lookup"><span data-stu-id="9d43f-145">Specifies the status of the batch.</span></span>|  

3.  <span data-ttu-id="9d43f-146">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="9d43f-146">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9d43f-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9d43f-147">See Also</span></span>  
 <span data-ttu-id="9d43f-148">[Paiements électroniques belges](belgian-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="9d43f-148">[Belgian Electronic Payments](belgian-electronic-payments.md) </span></span>  
 <span data-ttu-id="9d43f-149">[Comment configurer la banque électronique](how-to-set-up-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="9d43f-149">[How to: Set Up Electronic Banking](how-to-set-up-electronic-banking.md) </span></span>  
 [<span data-ttu-id="9d43f-150">Comment configurer les codes transaction IBLC/BLWI</span><span class="sxs-lookup"><span data-stu-id="9d43f-150">How to: Set Up IBLC-BLWI Transaction Codes</span></span>](how-to-set-up-iblc-blwi-transaction-codes.md)

