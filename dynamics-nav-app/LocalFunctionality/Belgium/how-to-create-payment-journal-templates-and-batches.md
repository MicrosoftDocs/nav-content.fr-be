---
title: "Comment créer des modèles et lots feuille paiement"
description: "Dans [!INCLUDE[navnow](../../includes/navnow_md.md)], des propositions de paiement sont générées et validées dans les feuilles paiement. La structure de la feuille paiement est semblable à celle des autres types de feuilles. Toutefois, la feuille paiement contient des champs spécifiques au traitement des paiements. Avant de pouvoir commencer à générer des propositions de paiement, vous devez configurer un modèle feuille paiement et un nom feuille paiement."
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
ms.openlocfilehash: 67b116fd8b5fa5b63e8855922c793ca7d94b870f
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-payment-journal-templates-and-batches"></a><span data-ttu-id="a5654-106">Comment créer des modèles et lots feuille paiement</span><span class="sxs-lookup"><span data-stu-id="a5654-106">How to: Create Payment Journal Templates and Batches</span></span>
<span data-ttu-id="a5654-107">Dans [!INCLUDE[navnow](../../includes/navnow_md.md)], des propositions de paiement sont générées et validées dans les feuilles paiement.</span><span class="sxs-lookup"><span data-stu-id="a5654-107">In [!INCLUDE[navnow](../../includes/navnow_md.md)], payment suggestions are generated and posted in payment journals.</span></span> <span data-ttu-id="a5654-108">La structure de la feuille paiement est semblable à celle des autres types de feuilles.</span><span class="sxs-lookup"><span data-stu-id="a5654-108">The structure of the payment journal is similar to the structure of other journal types.</span></span> <span data-ttu-id="a5654-109">Toutefois, la feuille paiement contient des champs spécifiques au traitement des paiements.</span><span class="sxs-lookup"><span data-stu-id="a5654-109">However, the payment journal contains some fields that are specific for processing payments.</span></span> <span data-ttu-id="a5654-110">Avant de pouvoir commencer à générer des propositions de paiement, vous devez configurer un modèle feuille paiement et un nom feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="a5654-110">Before you can start generating payment suggestions, you have to set up a payment journal template and a payment journal batch.</span></span>  
  
 <span data-ttu-id="a5654-111">Si vous attribuez un compte bancaire au modèle feuille paiement, le compte bancaire sera inséré dans tous les noms feuille paiement et toutes les lignes feuille paiement créés à l'aide de ce modèle.</span><span class="sxs-lookup"><span data-stu-id="a5654-111">If you assign a bank account to the payment journal template, the bank account will be inserted on all payment journal batches and payment journal lines that are created by using this template.</span></span> <span data-ttu-id="a5654-112">En indiquant un compte bancaire pour le modèle feuille, vous pouvez réduire le délai de vérification des propositions de paiement.</span><span class="sxs-lookup"><span data-stu-id="a5654-112">By specifying a bank account for the journal template, you can reduce the time that is required for checking the payment suggestions.</span></span>  
  
### <a name="to-create-a-payment-journal-template"></a><span data-ttu-id="a5654-113">Pour créer un modèle feuille paiement</span><span class="sxs-lookup"><span data-stu-id="a5654-113">To create a payment journal template</span></span>  
  
1.  <span data-ttu-id="a5654-114">Sélectionnez l'icône ![Rechercher une page ou un état](media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Modèles FS paiements**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="a5654-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journal Templates**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="a5654-115">Dans l'onglet **Accueil**, dans le groupe **Nouveau**, sélectionnez **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="a5654-115">On the **Home** tab, in the **New** group, choose **New**.</span></span>  
  
3.  <span data-ttu-id="a5654-116">Dans la fenêtre **Modèles FS paiements EB**, renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="a5654-116">In the **EB Payment Journal Templates** window, fill in the fields as described in the following table.</span></span>  
  
    |<span data-ttu-id="a5654-117">Champ</span><span class="sxs-lookup"><span data-stu-id="a5654-117">Field</span></span>|<span data-ttu-id="a5654-118">Description</span><span class="sxs-lookup"><span data-stu-id="a5654-118">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="a5654-119">**Nom**</span><span class="sxs-lookup"><span data-stu-id="a5654-119">**Name**</span></span>|<span data-ttu-id="a5654-120">Entrez le nom unique du modèle feuille paiement que vous créez.</span><span class="sxs-lookup"><span data-stu-id="a5654-120">Enter the unique name for the payment journal template that you are creating.</span></span>|  
    |<span data-ttu-id="a5654-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="a5654-121">**Description**</span></span>|<span data-ttu-id="a5654-122">Entrez une description du modèle feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="a5654-122">Enter a description of the payment journal template.</span></span>|  
    |<span data-ttu-id="a5654-123">**Compte bancaire**</span><span class="sxs-lookup"><span data-stu-id="a5654-123">**Bank Account**</span></span>|<span data-ttu-id="a5654-124">Sélectionnez le compte bancaire qui sera utilisé lorsque vous créerez une proposition de paiement.</span><span class="sxs-lookup"><span data-stu-id="a5654-124">Select the bank account that will be used when you create a payment suggestion.</span></span>|  
    |<span data-ttu-id="a5654-125">**Code motif**</span><span class="sxs-lookup"><span data-stu-id="a5654-125">**Reason Code**</span></span>|<span data-ttu-id="a5654-126">Sélectionnez le code motif qui sera utilisé sur tous les noms et lignes feuille créés à l'aide du modèle feuille.</span><span class="sxs-lookup"><span data-stu-id="a5654-126">Select the reason code that will be used on all the journal batches and lines that are created by using the journal template.</span></span> <span data-ttu-id="a5654-127">Si vous souhaitez utiliser un autre code motif sur une ligne feuille, vous pouvez le modifier manuellement.</span><span class="sxs-lookup"><span data-stu-id="a5654-127">If you want to use a different reason code on a journal line, you can manually change it.</span></span>|  
    |<span data-ttu-id="a5654-128">**Code journal**</span><span class="sxs-lookup"><span data-stu-id="a5654-128">**Source Code**</span></span>|<span data-ttu-id="a5654-129">Sélectionnez le code source qui sera utilisé sur tous les noms et lignes feuille créés à l'aide du modèle feuille.</span><span class="sxs-lookup"><span data-stu-id="a5654-129">Select the source code that will be used on all the journal batches and lines that are created by using the journal template.</span></span>|  
  
4.  <span data-ttu-id="a5654-130">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="a5654-130">Choose the **OK** button.</span></span>  
  
### <a name="to-add-payment-journal-batches-to-the-journal-template"></a><span data-ttu-id="a5654-131">Pour ajouter des noms feuille paiement au modèle feuille</span><span class="sxs-lookup"><span data-stu-id="a5654-131">To add payment journal batches to the journal template</span></span>  
  
1.  <span data-ttu-id="a5654-132">Dans la fenêtre **Modèles FS paiements**, dans l'onglet **Naviguer**, dans le groupe **Modèle**, sélectionnez **Noms feuilles**.</span><span class="sxs-lookup"><span data-stu-id="a5654-132">In the **Payment Journal Templates** window, on the **Navigate** tab, in the **Template** group, choose **Batches**.</span></span>  
  
2.  <span data-ttu-id="a5654-133">Dans la fenêtre **Nom FS paiements**, renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="a5654-133">In the **Paym. Journal Batch** window, fill in the fields as described in the following table.</span></span>  
  
    |<span data-ttu-id="a5654-134">Champ</span><span class="sxs-lookup"><span data-stu-id="a5654-134">Field</span></span>|<span data-ttu-id="a5654-135">Description</span><span class="sxs-lookup"><span data-stu-id="a5654-135">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="a5654-136">**Nom modèle feuille**</span><span class="sxs-lookup"><span data-stu-id="a5654-136">**Journal Template Name**</span></span>|<span data-ttu-id="a5654-137">Spécifiez un nom de modèle feuille pour le nom feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="a5654-137">Specify a journal template name for the payment journal batch.</span></span>|  
    |<span data-ttu-id="a5654-138">**Nom**</span><span class="sxs-lookup"><span data-stu-id="a5654-138">**Name**</span></span>|<span data-ttu-id="a5654-139">Entrez un nom unique pour le nom feuille.</span><span class="sxs-lookup"><span data-stu-id="a5654-139">Enter a unique name for the journal batch.</span></span><br /><br /> <span data-ttu-id="a5654-140">**NOTE :** pour que le nom feuille se mette à jour de façon numérique, ajoutez un numéro dans le nom feuille.</span><span class="sxs-lookup"><span data-stu-id="a5654-140">**NOTE:** To have the journal name update numerically, include a number in the journal batch name.</span></span> <span data-ttu-id="a5654-141">Par exemple, à chaque validation, le nom KBC1 sera mis à jour en KBC2, KBC3, etc.</span><span class="sxs-lookup"><span data-stu-id="a5654-141">For example, the name KBC1 will increment by one number with every posting to KBC2, KBC3, and so on.</span></span>|  
    |<span data-ttu-id="a5654-142">**Description**</span><span class="sxs-lookup"><span data-stu-id="a5654-142">**Description**</span></span>|<span data-ttu-id="a5654-143">Entrez une description pour le nom feuille.</span><span class="sxs-lookup"><span data-stu-id="a5654-143">Enter a description for the journal batch.</span></span>|  
    |<span data-ttu-id="a5654-144">**Code motif**</span><span class="sxs-lookup"><span data-stu-id="a5654-144">**Reason Code**</span></span>|<span data-ttu-id="a5654-145">Spécifie le code motif lié à ce nom feuille.</span><span class="sxs-lookup"><span data-stu-id="a5654-145">Specifies the reason code that is linked to this journal batch.</span></span>|  
    |<span data-ttu-id="a5654-146">**Statut**</span><span class="sxs-lookup"><span data-stu-id="a5654-146">**Status**</span></span>|<span data-ttu-id="a5654-147">Indique le statut du lot.</span><span class="sxs-lookup"><span data-stu-id="a5654-147">Specifies the status of the batch.</span></span>|  
  
3.  <span data-ttu-id="a5654-148">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="a5654-148">Choose the **OK** button.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="a5654-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a5654-149">See Also</span></span>  
 <span data-ttu-id="a5654-150">[Paiements électroniques belges](belgian-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="a5654-150">[Belgian Electronic Payments](belgian-electronic-payments.md) </span></span>  
 <span data-ttu-id="a5654-151">[Comment configurer la banque électronique](how-to-set-up-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="a5654-151">[How to: Set Up Electronic Banking](how-to-set-up-electronic-banking.md) </span></span>  
 [<span data-ttu-id="a5654-152">Comment configurer les codes transaction IBLC/BLWI</span><span class="sxs-lookup"><span data-stu-id="a5654-152">How to: Set Up IBLC-BLWI Transaction Codes</span></span>](how-to-set-up-iblc-blwi-transaction-codes.md)
