---
title: "Procédure : créer des enregistrements document entrant"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: e91c4570ff60d991974ac6afd16ba3bc3e73e44f
ms.contentlocale: fr-be
ms.lasthandoff: 07/19/2017

---

# <a name="how-to-create-incoming-document-records"></a><span data-ttu-id="1cfb3-102">Procédure : créer des enregistrements document entrant</span><span class="sxs-lookup"><span data-stu-id="1cfb3-102">How to: Create Incoming Document Records</span></span>
<span data-ttu-id="1cfb3-103">Dans la fenêtre **Documents entrants**, vous pouvez utiliser différentes fonctions pour examiner les reçus de dépenses, gérer les tâches ROC et convertir les fichiers document entrants, manuellement ou automatiquement, en documents ou lignes feuille appropriés.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-103">In the **Incoming Documents** window, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="1cfb3-104">Les fichiers externes peuvent être joints à n'importe quelle étape du processus, notamment en ce qui concerne les documents validés et au fournisseur, au client qui en résulte, et dans les écritures comptables.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-104">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span>

<span data-ttu-id="1cfb3-105">Pour enregistrer un document externe dans Dynamics NAV, vous devez d'abord créer ou terminer un enregistrement document entrant.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-105">To record an external document in Dynamics NAV, you must first create or complete an incoming document record.</span></span> <span data-ttu-id="1cfb3-106">Vous pouvez effectuer cette opération manuellement ou prendre une photo du document externe puis créer l'enregistrement document entrant avec le fichier image joint.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-106">You can do this manually, or you can take a photo of the external document and then create the incoming document record with the image file attached.</span></span>

<span data-ttu-id="1cfb3-107">Avant d'utiliser la fonctionnalité Documents entrants, vous devez exécuter la configuration requise.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-107">Before you can use the Incoming Documents feature, you must perform the required setup.</span></span> <span data-ttu-id="1cfb3-108">Pour plus d'informations, reportez vous à [Procédure : configurer des documents entrants](across-how-setup-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="1cfb3-108">For more information, see [How to: Set Up Incoming Documents](across-how-setup-income-documents.md).</span></span>

## <a name="to-approve-or-reject-an-incoming-document"></a><span data-ttu-id="1cfb3-109">Approbation ou rejet d'un document entrant</span><span class="sxs-lookup"><span data-stu-id="1cfb3-109">To approve or reject an incoming document</span></span>
<span data-ttu-id="1cfb3-110">Si vous souhaitez autoriser des utilisateurs à créer des factures ou des lignes feuille comptabilité à partir d'enregistrements document entrant, sauf s'ils sont approbateurs, vous pouvez configurer des approbateurs qui doivent approuver les enregistrements avant de pouvoir être traités.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-110">If you do want to allow users to create invoices or general journal lines from incoming document records unless they are approved, you can set up approvers who must approve the records before they can be processed.</span></span>

1. <span data-ttu-id="1cfb3-111">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Documents entrants**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-111">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Documents**, and then choose the related link.</span></span>
2. <span data-ttu-id="1cfb3-112">Sélectionnez la ligne contenant le document à approuver ou rejeter, puis sélectionnez l'action **Approuver** or **Rejeter**.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-112">Select the line with the document that you want to approve or reject, and then choose the **Approve** or **Reject** actions.</span></span>

<span data-ttu-id="1cfb3-113">Si vous approuvez l'enregistrement document entrant, la case à cocher **Lancé** de la ligne document entrant est activée.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-113">If you approve the incoming document record, the **Released** check box on the incoming document line is selected.</span></span> <span data-ttu-id="1cfb3-114">L'utilisateur chargé de créer, par exemple, des factures achat peut continuer à traiter l'enregistrement.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-114">The user in charge of creating, for example, purchase invoices can proceed to process the record.</span></span>

## <a name="to-create-an-incoming-document-record-by-taking-a-photo"></a><span data-ttu-id="1cfb3-115">Pour créer un enregistrement de document entrant en prenant une photo</span><span class="sxs-lookup"><span data-stu-id="1cfb3-115">To create an incoming document record by taking a photo</span></span>
<span data-ttu-id="1cfb3-116">**Remarque** : la procédure suivante s'applique uniquement aux tablettes et téléphones clients Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-116">**Note**: The following procedure only applies to the Dynamics NAV Tablet and Phone clients.</span></span>

1. <span data-ttu-id="1cfb3-117">Dans la barre d'application, sélectionnez la mosaïque **Créer le document entrant à partir de l'appareil photo**, puis passez à l'étape 4.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-117">On the app bar, choose the **Create Incoming Document from Camera** tile, and then go to step 4.</span></span>
2. <span data-ttu-id="1cfb3-118">Sinon, dans la barre d'application, cliquez sur le bouton Options, choisissez **Documents entrants**, puis **Tous**.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-118">Alternatively, on the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span></span>
3. <span data-ttu-id="1cfb3-119">Dans la fenêtre **Documents entrants**, sélectionnez le bouton de sélection, puis **Créer à partir de l'appareil photo**.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-119">In the **Incoming Documents** window, choose the ellipsis button, and then choose **Create from Camera**.</span></span> <span data-ttu-id="1cfb3-120">L'appareil photo de la tablette ou du téléphone est activé.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-120">The camera on the tablet or phone is activated.</span></span>
4. <span data-ttu-id="1cfb3-121">Prenez une photo d'un document, tel qu'un reçu d'achat, que vous souhaitez traiter en tant que document entrant, puis sélectionnez le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-121">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span></span>

<span data-ttu-id="1cfb3-122">Un enregistrement de document entrant est créé, avec l'image jointe.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-122">A new incoming document record is created, with the image attached.</span></span>

## <a name="to-attach-an-image-to-an-incoming-document-record-by-taking-a-photo"></a><span data-ttu-id="1cfb3-123">Pour joindre une image à un enregistrement de document entrant en prenant une photo</span><span class="sxs-lookup"><span data-stu-id="1cfb3-123">To attach an image to an incoming document record by taking a photo</span></span>
<span data-ttu-id="1cfb3-124">**Remarque** : la procédure suivante s'applique uniquement aux tablettes et téléphones clients Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-124">**Note**: The following procedure only applies to the Dynamics NAV Tablet and Phone clients.</span></span>

1. <span data-ttu-id="1cfb3-125">Dans la barre d'application, cliquez sur le bouton Options, choisissez **Documents entrants**, puis **Tous**.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-125">On the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span></span>
2. <span data-ttu-id="1cfb3-126">Ouvrez la fiche de l'enregistrement de document entrant existant.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-126">Open the card for an existing incoming document record.</span></span>
3. <span data-ttu-id="1cfb3-127">Dans la fenêtre **Document entrant**, sélectionnez le bouton de sélection, puis **Joindre l'image de l'appareil photo**.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-127">In the **Incoming Document** window, choose the ellipsis button, and then choose **Attach Image from Camera**.</span></span> <span data-ttu-id="1cfb3-128">L'appareil photo de la tablette ou du téléphone est activé.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-128">The camera on the tablet or phone is activated.</span></span>
4. <span data-ttu-id="1cfb3-129">Prenez une photo d'un document, tel qu'un reçu d'achat, que vous souhaitez traiter en tant que document entrant, puis sélectionnez le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-129">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span></span>

<span data-ttu-id="1cfb3-130">L'image est jointe à l'enregistrement de document entrant.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-130">The image is attached to the incoming document record.</span></span>

## <a name="to-create-an-incoming-document-record-manually"></a><span data-ttu-id="1cfb3-131">Pour créer un enregistrement document entrant manuellement</span><span class="sxs-lookup"><span data-stu-id="1cfb3-131">To create an incoming document record manually</span></span>
1. <span data-ttu-id="1cfb3-132">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Documents entrants**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-132">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Documents**, and then choose the related link.</span></span>
2. <span data-ttu-id="1cfb3-133">Choisissez l'action **Créer à partir d'un fichier**.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-133">Choose the **Create from File** action.</span></span>  
3. <span data-ttu-id="1cfb3-134">Dans la fenêtre **Insérer un fichier**, sélectionnez un fichier, puis choisissez **Ouvrir**.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-134">In the **Insert File** window, select a file, and then choose **Open**.</span></span>

    <span data-ttu-id="1cfb3-135">Le fichier est automatiquement joint.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-135">The file is automatically attached.</span></span>
4. <span data-ttu-id="1cfb3-136">Sinon, choisissez l'action **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-136">Alternatively, choose the **New** action.</span></span>
5. <span data-ttu-id="1cfb3-137">Pour joindre un fichier, choisissez l'action **Joindre fichier**.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-137">To attach a file, choose the **Attach File** action.</span></span>
6. <span data-ttu-id="1cfb3-138">Dans la fenêtre **Insérer un fichier**, sélectionnez le fichier qui représente le document entrant concerné, puis choisissez le bouton **Ouvrir**.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-138">In the **Insert File** window, select the file that represents the incoming document in question, and then choose the **Open** button.</span></span>
7. <span data-ttu-id="1cfb3-139">Dans la fenêtre **Document entrant**, renseignez les champs selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-139">In the **Incoming Document** window, fill in the fields as necessary.</span></span> <span data-ttu-id="1cfb3-140">Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.</span><span class="sxs-lookup"><span data-stu-id="1cfb3-140">Choose a field to read a short description of the field or link to more information.</span></span>

##<a name="see-also"></a><span data-ttu-id="1cfb3-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1cfb3-141">See Also</span></span>  
[<span data-ttu-id="1cfb3-142">Traiter les documents entrants</span><span class="sxs-lookup"><span data-stu-id="1cfb3-142">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="1cfb3-143">Documents entrants</span><span class="sxs-lookup"><span data-stu-id="1cfb3-143">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="1cfb3-144">Gestion des achats</span><span class="sxs-lookup"><span data-stu-id="1cfb3-144">Manage Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="1cfb3-145">Utiliser Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="1cfb3-145">Work With Dynamics NAV</span></span>](ui-work-product.md)

