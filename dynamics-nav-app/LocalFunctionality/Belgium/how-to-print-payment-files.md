---
title: Comment imprimer les fichiers paiement
description: "Après avoir imprimé un test et corrigé toutes les erreurs, vous pouvez imprimer les lignes feuille paiement dans un fichier paiement."
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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 49936b0396a4c52ca78d150feeeeaff96c149ae9
ms.contentlocale: fr-be
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-print-payment-files"></a><span data-ttu-id="2b43e-103">Comment imprimer les fichiers paiement</span><span class="sxs-lookup"><span data-stu-id="2b43e-103">How to: Print Payment Files</span></span>
<span data-ttu-id="2b43e-104">Après avoir imprimé un test et corrigé toutes les erreurs, vous pouvez imprimer les lignes feuille paiement dans un fichier paiement.</span><span class="sxs-lookup"><span data-stu-id="2b43e-104">After you have printed a test report and corrected all errors, you can print the payment journal lines to a payment file.</span></span>  

<span data-ttu-id="2b43e-105">Un fichier paiement contient des paiements nationaux, internationaux, SEPA ou SEPA non libellés en Euro.</span><span class="sxs-lookup"><span data-stu-id="2b43e-105">A payment file contains either domestic, international, SEPA, or non-euro SEPA payments.</span></span> <span data-ttu-id="2b43e-106">Le fichier peut être envoyé à une banque sur disquette, par un modem ou via Isabel (Interbanks Standards Association Belgium).</span><span class="sxs-lookup"><span data-stu-id="2b43e-106">The file can be sent to a bank either on disk, by modem, or via Interbanks Standards Association Belgium (Isabel).</span></span> <span data-ttu-id="2b43e-107">Vous ne pouvez créer qu'un fichier par date de validation et par code devise.</span><span class="sxs-lookup"><span data-stu-id="2b43e-107">You can only create one file for each posting date and each currency code.</span></span> <span data-ttu-id="2b43e-108">Lorsque vous exportez les paiements dans un fichier, une note d'accompagnement est imprimée et peut aussi être envoyée à la banque.</span><span class="sxs-lookup"><span data-stu-id="2b43e-108">When you export the payments to a file, an accompanying note is printed, which can also be sent to the bank.</span></span>  

<span data-ttu-id="2b43e-109">Dans la feuille paiement, le champ **Statut** des lignes exportées sera défini sur **Validé**.</span><span class="sxs-lookup"><span data-stu-id="2b43e-109">In the payment journal, the **Status** field on the exported lines will be set to **Posted**.</span></span>  

## <a name="to-print-a-payment-file"></a><span data-ttu-id="2b43e-110">Pour imprimer un fichier paiement</span><span class="sxs-lookup"><span data-stu-id="2b43e-110">To print a payment file</span></span>  

1.  <span data-ttu-id="2b43e-111">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Feuille paiement**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="2b43e-111">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journal**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="2b43e-112">Dans le raccourci **Options**, remplissez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="2b43e-112">On the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="2b43e-113">Champ</span><span class="sxs-lookup"><span data-stu-id="2b43e-113">Field</span></span>|<span data-ttu-id="2b43e-114">Description</span><span class="sxs-lookup"><span data-stu-id="2b43e-114">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="2b43e-115">**Nom de la feuille**</span><span class="sxs-lookup"><span data-stu-id="2b43e-115">**Batch Name**</span></span>|<span data-ttu-id="2b43e-116">Spécifiez le nom de la feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="2b43e-116">Specify the batch name of the payment journal.</span></span>|  
    |<span data-ttu-id="2b43e-117">**Compte bancaire**</span><span class="sxs-lookup"><span data-stu-id="2b43e-117">**Bank Account**</span></span>|<span data-ttu-id="2b43e-118">Spécifiez le compte bancaire de la feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="2b43e-118">Specify the bank account of the payment journal.</span></span>|  
    |<span data-ttu-id="2b43e-119">**Protocole d'exportation**</span><span class="sxs-lookup"><span data-stu-id="2b43e-119">**Export Protocol**</span></span>|<span data-ttu-id="2b43e-120">Spécifiez le code du protocole d'exportation de la ligne feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="2b43e-120">Specify the export protocol code of the payment journal line.</span></span> <span data-ttu-id="2b43e-121">Exportez des protocoles qui contrôlent le fichier de paiement qui sera généré dans la feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="2b43e-121">Export protocols control which payment file will be generated in the payment journal.</span></span><br /><br /> <span data-ttu-id="2b43e-122">Vous pouvez avoir plusieurs formats d'exportation différents dans un seul lot, comme les formats national, international, SEPA, ou un ensemble des trois.</span><span class="sxs-lookup"><span data-stu-id="2b43e-122">You can have a mixture of export formats in a single batch, such as domestic, international, SEPA, or a combination of these.</span></span> <span data-ttu-id="2b43e-123">Toutefois, lorsque vous exportez les lignes paiement dans un fichier, vous ne pouvez utiliser qu'un format ou protocole d'exportation.</span><span class="sxs-lookup"><span data-stu-id="2b43e-123">However, when exporting the payment lines to a file, you can only use one export format, or export protocol.</span></span> <span data-ttu-id="2b43e-124">**Note :**  En définissant le protocole d'exportation, vous définissez également le type de validation qui sera effectuée dans la feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="2b43e-124">**Note:**  By defining the export protocol, you also define the type of validation that will be performed in the payment journal.</span></span>|  

3.  <span data-ttu-id="2b43e-125">Choisissez l'action **Vérifier les lignes de paiement**.</span><span class="sxs-lookup"><span data-stu-id="2b43e-125">Choose the **Check Payment Lines** action.</span></span>

    <span data-ttu-id="2b43e-126">La fenêtre **Exporter les journaux d'erreur de chèque** affiche les erreurs éventuelles qui pourraient exister.</span><span class="sxs-lookup"><span data-stu-id="2b43e-126">The **Export Check Error Logs** window displays any errors that may exist.</span></span> <span data-ttu-id="2b43e-127">S'il y a des erreurs, vous devez les corriger avant de continuer.</span><span class="sxs-lookup"><span data-stu-id="2b43e-127">If there are errors, you must fix the errors before you can continue.</span></span>

4. <span data-ttu-id="2b43e-128">S'il n'y a pas d'erreur, choisissez l'action **Exporter les lignes de paiement**.</span><span class="sxs-lookup"><span data-stu-id="2b43e-128">If there are no errors, choose the **Export Payment Lines** action.</span></span>  

    <span data-ttu-id="2b43e-129">L'état que vous avez spécifié dans le champ **ID impression test** des **Modèles FS paiements EB** s'ouvre.</span><span class="sxs-lookup"><span data-stu-id="2b43e-129">The report that you specified in the **Test Report ID** field in the **EB Payment Journal Templates** will open.</span></span>  

5.  <span data-ttu-id="2b43e-130">Cliquez sur le bouton **Imprimer**.</span><span class="sxs-lookup"><span data-stu-id="2b43e-130">Choose the **Print** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="2b43e-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2b43e-131">See Also</span></span>  
 <span data-ttu-id="2b43e-132">[Banque électronique belge](belgian-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="2b43e-132">[Belgian Electronic Banking](belgian-electronic-banking.md) </span></span>  
 <span data-ttu-id="2b43e-133">[Paiements électroniques belges](belgian-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="2b43e-133">[Belgian Electronic Payments](belgian-electronic-payments.md) </span></span>  
 <span data-ttu-id="2b43e-134">[Comment configurer la banque électronique](how-to-set-up-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="2b43e-134">[How to: Set Up Electronic Banking](how-to-set-up-electronic-banking.md) </span></span>  
 <span data-ttu-id="2b43e-135">[Comment configurer les codes transaction IBLC/BLWI](how-to-set-up-iblc-blwi-transaction-codes.md) </span><span class="sxs-lookup"><span data-stu-id="2b43e-135">[How to: Set Up IBLC-BLWI Transaction Codes](how-to-set-up-iblc-blwi-transaction-codes.md) </span></span>  
 <span data-ttu-id="2b43e-136">[Comment configurer les fournisseurs pour les propositions de paiement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="2b43e-136">[How to: Set Up Vendors for Automatic Payment Suggestions](how-to-set-up-vendors-for-automatic-payment-suggestions.md) </span></span>  
 <span data-ttu-id="2b43e-137">[Comment générer des propositions de paiement](how-to-generate-payment-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="2b43e-137">[How to: Generate Payment Suggestions](how-to-generate-payment-suggestions.md) </span></span>  
 <span data-ttu-id="2b43e-138">[Comment créer des modèles et lots feuille paiement](how-to-create-payment-journal-templates-and-batches.md) </span><span class="sxs-lookup"><span data-stu-id="2b43e-138">[How to: Create Payment Journal Templates and Batches](how-to-create-payment-journal-templates-and-batches.md) </span></span>  
 <span data-ttu-id="2b43e-139">[Comment tester les paiements électroniques](how-to-test-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="2b43e-139">[How to: Test Electronic Payments](how-to-test-electronic-payments.md) </span></span>  
 [<span data-ttu-id="2b43e-140">Comment gérer les lignes paiement électronique</span><span class="sxs-lookup"><span data-stu-id="2b43e-140">How to: Manage Electronic Payment Lines</span></span>](how-to-manage-electronic-payment-lines.md)

