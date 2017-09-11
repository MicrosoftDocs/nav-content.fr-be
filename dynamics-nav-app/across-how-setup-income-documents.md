---
title: "Procédure : configurer les documents entrants"
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
ms.openlocfilehash: d55329b571e4c59d4821a86a39362ea58480b86a
ms.contentlocale: fr-be
ms.lasthandoff: 07/19/2017

---

# <a name="how-to-set-up-incoming-documents"></a><span data-ttu-id="ac1b5-102">Procédure : configurer les documents entrants</span><span class="sxs-lookup"><span data-stu-id="ac1b5-102">How to: Set Up Incoming Documents</span></span>
<span data-ttu-id="ac1b5-103">Si vous créez des lignes feuille comptabilité à partir des enregistrements de documents entrants, vous devez spécifier dans la fenêtre **Paramètres des documents entrants** quels modèle et nom de feuille utiliser.</span><span class="sxs-lookup"><span data-stu-id="ac1b5-103">If you create general journal lines from incoming document records, you must specify in the **Incoming Documents Setup** window which journal template and batch to use.</span></span>

<span data-ttu-id="ac1b5-104">Si vous ne souhaitez pas que les utilisateurs créent des factures ou des lignes feuille comptabilité à partir d'enregistrements de documents entrants, sauf si les documents ont été préalablement approuvés, vous devez paramétrer des approbateurs dans la fenêtre **Approbateurs de document entrant**.</span><span class="sxs-lookup"><span data-stu-id="ac1b5-104">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up approvers in the **Incoming Document Approvers** window.</span></span>

<span data-ttu-id="ac1b5-105">Pour convertir les fichiers PDF et image en documents électroniques que vous pouvez convertir, par exemple, en factures achat dans Dynamics NAV, vous devez d'abord configurer la fonctionnalité OCR et activer le service.</span><span class="sxs-lookup"><span data-stu-id="ac1b5-105">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside Dynamics NAV, you must first set up the OCR feature and enable the service.</span></span>

<span data-ttu-id="ac1b5-106">Une fois que la fonctionnalité Documents entrants est configurée, vous pouvez utiliser différentes fonctions pour examiner les reçus de dépenses, gérer les tâches ROC et convertir les fichiers document entrants, manuellement ou automatiquement, en documents ou lignes feuille appropriés.</span><span class="sxs-lookup"><span data-stu-id="ac1b5-106">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="ac1b5-107">Les fichiers externes peuvent être joints à n'importe quelle étape du processus, notamment en ce qui concerne les documents validés et au fournisseur, au client qui en résulte, et dans les écritures comptables.</span><span class="sxs-lookup"><span data-stu-id="ac1b5-107">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span> <span data-ttu-id="ac1b5-108">Pour plus d'informations, reportez vous à [Procédure : traiter les documents entrants](across-process-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="ac1b5-108">For more information, see [How to: Process Incoming Documents](across-process-income-documents.md).</span></span>

## <a name="to-set-up-the-incoming-documents-feature"></a><span data-ttu-id="ac1b5-109">Configurer la fonctionnalité Documents entrants</span><span class="sxs-lookup"><span data-stu-id="ac1b5-109">To set up the Incoming Documents feature</span></span>
1. <span data-ttu-id="ac1b5-110">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Configuration document entrant**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="ac1b5-110">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="ac1b5-111">Renseignez les champs selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="ac1b5-111">Fill in the fields as necessary.</span></span> <span data-ttu-id="ac1b5-112">Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.</span><span class="sxs-lookup"><span data-stu-id="ac1b5-112">Choose a field to read a short description of the field or link to more information.</span></span>

## <a name="to-set-up-approvers-of-incoming-document-records"></a><span data-ttu-id="ac1b5-113">Configurer des approbateurs d'enregistrements document entrant</span><span class="sxs-lookup"><span data-stu-id="ac1b5-113">To set up approvers of incoming document records</span></span>
1. <span data-ttu-id="ac1b5-114">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Configuration document entrant**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="ac1b5-114">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ac1b5-115">Dans la fenêtre **Paramètres des documents entrants**, sélectionnez l'action **Approbateurs**.</span><span class="sxs-lookup"><span data-stu-id="ac1b5-115">In the **Incoming Documents Setup** window, choose the **Approvers** action.</span></span>

    <span data-ttu-id="ac1b5-116">La fenêtre **Approbateurs de document entrant** affiche tous les utilisateurs configurés dans votre solution Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="ac1b5-116">The **Incoming Document Approvers** window shows all users that are set up in your Dynamics NAV .</span></span>  
3. <span data-ttu-id="ac1b5-117">Sélectionnez un ou plusieurs utilisateurs pouvant approuver un document entrant pour qu'un document ou une ligne feuille connexe puisse être créée.</span><span class="sxs-lookup"><span data-stu-id="ac1b5-117">Select one or more users that can approve an incoming document before a related document or journal line can be created.</span></span>

<span data-ttu-id="ac1b5-118">Lorsque des approbateurs ont été configurés dans la fenêtre **Approbateurs de document entrant**, seuls ces utilisateurs peuvent approuver un document entrant si la case **Exiger une approbation pour créer** est cochée dans la fenêtre **Paramètres des documents entrants**.</span><span class="sxs-lookup"><span data-stu-id="ac1b5-118">When approvers have been set up in the **Incoming Document Approvers** window, only those users can approve an incoming document if the **Require Approval To Create** check box in the **Incoming Documents Setup** window is selected.</span></span>

<span data-ttu-id="ac1b5-119">**Remarque** : ce paramétrage d'approbation n'est pas lié aux flux d'approbation.</span><span class="sxs-lookup"><span data-stu-id="ac1b5-119">**Note**: This approval setup is not related to approval workflows.</span></span> <span data-ttu-id="ac1b5-120">Pour plus d'informations, reportez-vous à [Procédure : utilisation des flux d'approbation](across-how-use-approval-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="ac1b5-120">For more information, see [How to: Use Approval Workflows](across-how-use-approval-workflows.md).</span></span>

## <a name="to-set-up-an-ocr-service"></a><span data-ttu-id="ac1b5-121">Configurer un service ROC</span><span class="sxs-lookup"><span data-stu-id="ac1b5-121">To set up an OCR service</span></span>
1. <span data-ttu-id="ac1b5-122">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Paramètres service OCR**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="ac1b5-122">In the top right corner, choose the **Search for Page or Report** icon, enter **OCR Service Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="ac1b5-123">Renseignez les champs selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="ac1b5-123">Fill in the fields as necessary.</span></span> <span data-ttu-id="ac1b5-124">Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.</span><span class="sxs-lookup"><span data-stu-id="ac1b5-124">Choose a field to read a short description of the field or link to more information.</span></span>


## <a name="to-encrypt-your-login-information"></a><span data-ttu-id="ac1b5-125">Chiffrer les informations de connexion</span><span class="sxs-lookup"><span data-stu-id="ac1b5-125">To encrypt your login information</span></span>
<span data-ttu-id="ac1b5-126">Il est recommandé de protéger les informations de connexion que vous saisissez dans la fenêtre **Paramètres service OCR**.</span><span class="sxs-lookup"><span data-stu-id="ac1b5-126">It is recommended that you protect the logon information that you enter in the **OCR Service Setup** window.</span></span> <span data-ttu-id="ac1b5-127">Vous pouvez chiffrer des données sur le serveur en générant de nouvelles clés de chiffrement ou en important des clés existantes que vous activez sur l'instance de serveur qui est connectée à la base de données.</span><span class="sxs-lookup"><span data-stu-id="ac1b5-127">You can encrypt data on the server by generating new or importing existing encryption keys that you enable on the server instance that connects to the database.</span></span>

1. <span data-ttu-id="ac1b5-128">Dans la fenêtre **Paramètres service OCR**, sélectionnez l'action **Gestion du chiffrement**.</span><span class="sxs-lookup"><span data-stu-id="ac1b5-128">In the **OCR Service Setup** window, choose the **Encryption Management** action.</span></span>
2. <span data-ttu-id="ac1b5-129">Dans la fenêtre **Gestion du chiffrement des données**, activez le chiffrement de vos données.</span><span class="sxs-lookup"><span data-stu-id="ac1b5-129">In the **Data Encryption Management** window, enable encryption of your data.</span></span>

## <a name="see-also"></a><span data-ttu-id="ac1b5-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ac1b5-130">See Also</span></span>  
[<span data-ttu-id="ac1b5-131">Traiter les documents entrants</span><span class="sxs-lookup"><span data-stu-id="ac1b5-131">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="ac1b5-132">Documents entrants</span><span class="sxs-lookup"><span data-stu-id="ac1b5-132">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="ac1b5-133">Gestion des achats</span><span class="sxs-lookup"><span data-stu-id="ac1b5-133">Manage Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="ac1b5-134">Utiliser Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="ac1b5-134">Work With Dynamics NAV</span></span>](ui-work-product.md)

