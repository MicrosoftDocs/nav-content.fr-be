---
title: "Comment configurer la banque électronique"
description: "Avec la banque électronique, vous pouvez effectuer des paiements électroniques pour des fournisseurs et des clients nationaux, internationaux, SEPA ou SEPA non libellés en Euro."
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
ms.openlocfilehash: 63ddc88627d5c3a9d6692d7e9573617da8aaea30
ms.contentlocale: fr-be
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-set-up-electronic-banking"></a><span data-ttu-id="fe6a9-103">Comment configurer la banque électronique</span><span class="sxs-lookup"><span data-stu-id="fe6a9-103">How to: Set Up Electronic Banking</span></span>
<span data-ttu-id="fe6a9-104">Avec la banque électronique, vous pouvez effectuer des paiements électroniques pour des fournisseurs et des clients nationaux, internationaux, SEPA ou SEPA non libellés en Euro.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-104">With electronic banking, you can make electronic payments to domestic, international, SEPA, and non-Euro SEPA vendors and customers.</span></span>  

<span data-ttu-id="fe6a9-105">Votre société souscrit un contrat eBanking avec la banque pour maintenir un certain compte bancaire ou plusieurs comptes bancaires.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-105">Your company subscribes to an eBanking contract with the bank to maintain a certain bank account or several bank accounts.</span></span> <span data-ttu-id="fe6a9-106">La société s'inscrit également auprès d'Isabel pour envoyer des fichiers paiement à la banque et recevoir des fichiers relevé bancaire de la banque par voie électronique.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-106">The company also subscribes to Isabel to send payment files to and receive bank statement files from the bank electronically.</span></span> <span data-ttu-id="fe6a9-107">La société reçoit ainsi des cartes à puce liées au contrat eBanking.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-107">Therefore, the company receives smartcards linked to the eBanking contract.</span></span> <span data-ttu-id="fe6a9-108">Les cartes à puce sont sécurisées par code PIN.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-108">The smartcards are secured by PIN codes.</span></span>  

<span data-ttu-id="fe6a9-109">Vous recevrez l'une de ces cartes à puce pour vous connecter à IBS et être lié au contrat eBanking de la société.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-109">You will receive one of these smartcards to connect to IBS so that you are connected to the eBanking contract of the company.</span></span>  

<span data-ttu-id="fe6a9-110">Lors du téléchargement de fichiers vers ou depuis la plateforme IBS, vous insérerez la carte à puce dans le lecteur de carte et utiliserez un code PIN pour établir la connexion à IBS.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-110">When uploading to or downloading files from the IBS platform, you will insert the smartcard in the card reader and use a PIN code to make connection to IBS.</span></span> <span data-ttu-id="fe6a9-111">Lorsque la connexion à IBS est établie, le contrat eBanking et l'utilisateur eBanking sont reconnus par le système.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-111">When the IBS session is established, the eBanking contract and eBanking user is known by the system.</span></span> <span data-ttu-id="fe6a9-112">Les numéros de compte liés du contrat eBanking et de l'utilisateur sont également reconnus.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-112">Also the eBanking contract and user linked bank account numbers are known.</span></span>  

<span data-ttu-id="fe6a9-113">Avant de pouvoir utiliser la banque électronique, vous devez configurer les informations suivantes :</span><span class="sxs-lookup"><span data-stu-id="fe6a9-113">Before you can use electronic banking, you must set up the following information:</span></span>  

- <span data-ttu-id="fe6a9-114">Configuration de la banque électronique.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-114">Electronic banking setup.</span></span>  
- <span data-ttu-id="fe6a9-115">Codes IBLC/BLWI : pour plus d'informations, voir [Comment configurer des codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md).</span><span class="sxs-lookup"><span data-stu-id="fe6a9-115">IBLC/BLWI codes - For more information, see [How to: Set Up IBLC-BLWI Transaction Codes](how-to-set-up-iblc-blwi-transaction-codes.md).</span></span>  
- <span data-ttu-id="fe6a9-116">Comptes bancaires préférés (facultatif).</span><span class="sxs-lookup"><span data-stu-id="fe6a9-116">Preferred bank accounts (optional).</span></span>  

## <a name="to-set-up-electronic-banking"></a><span data-ttu-id="fe6a9-117">Pour configurer la banque électronique</span><span class="sxs-lookup"><span data-stu-id="fe6a9-117">To set up electronic banking</span></span>  

1.  <span data-ttu-id="fe6a9-118">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Configuration de la banque électronique**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-118">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Electronic Banking Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="fe6a9-119">Dans la fenêtre **Configuration de la banque électronique**, dans le raccourci **Général**, remplissez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-119">In the **Electronic Banking Setup** window, on the **General** FastTab, fill in the fields as described in the following table.</span></span>   

    |<span data-ttu-id="fe6a9-120">Champ</span><span class="sxs-lookup"><span data-stu-id="fe6a9-120">Field</span></span>|<span data-ttu-id="fe6a9-121">Description</span><span class="sxs-lookup"><span data-stu-id="fe6a9-121">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="fe6a9-122">**Résumer lignes FS**</span><span class="sxs-lookup"><span data-stu-id="fe6a9-122">**Summarize Gen. Jnl. Lines**</span></span>|<span data-ttu-id="fe6a9-123">Sélectionnez pour indiquer si vous souhaitez regrouper les lignes feuilles paiement pour chaque fournisseur.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-123">Select to indicate if you want to group the payment journal lines for each vendor.</span></span>|  
    |<span data-ttu-id="fe6a9-124">**Couper comm. de paiement**</span><span class="sxs-lookup"><span data-stu-id="fe6a9-124">**Cut off Payment Message Texts**</span></span>|<span data-ttu-id="fe6a9-125">Sélectionnez pour indiquer si vous souhaitez tronquer les longues communications de paiement.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-125">Select to indicate if you want to truncate long payment messages.</span></span> <span data-ttu-id="fe6a9-126">Les communications seront tronquées si elles contiennent plus de 106 caractères pour les paiements nationaux et plus de 140 caractères pour les paiements internationaux.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-126">Messages will be truncated if greater than 106 characters for domestic payments and less than 140 characters for international payments.</span></span>|  
    |<span data-ttu-id="fe6a9-127">**Version IBS**</span><span class="sxs-lookup"><span data-stu-id="fe6a9-127">**IBS Version**</span></span>|<span data-ttu-id="fe6a9-128">Spécifiez la version d'Isabel actuellement utilisée pour la fonction de banque électronique dans votre organisation.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-128">Specify the version of Isabel that is currently used for electronic banking in your organization.</span></span>|  
    |<span data-ttu-id="fe6a9-129">**Adresse électronique de notification**</span><span class="sxs-lookup"><span data-stu-id="fe6a9-129">**Notification E-mail address**</span></span>|<span data-ttu-id="fe6a9-130">Spécifiez l'adresse électronique de notification que vous souhaitez utiliser pour les messages concernant les transactions et le solde de la banque électronique.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-130">Specify the notification email address that you want to use for electronic banking balance and transaction messages.</span></span> <span data-ttu-id="fe6a9-131">Il s'agit de l'adresse par défaut utilisée pour contacter le serveur Isabel.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-131">This is the default address that is used to contact the Isabel server.</span></span>|  
    |<span data-ttu-id="fe6a9-132">**Langue**</span><span class="sxs-lookup"><span data-stu-id="fe6a9-132">**Language**</span></span>|<span data-ttu-id="fe6a9-133">Spécifiez la langue que vous souhaitez utiliser pour les messages concernant les transactions et le solde de la banque électronique.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-133">Specify the language that you want to use for electronic bank balance and transaction messages.</span></span>|  
    |<span data-ttu-id="fe6a9-134">**Version de service IBS**</span><span class="sxs-lookup"><span data-stu-id="fe6a9-134">**IBS Service Version**</span></span>|<span data-ttu-id="fe6a9-135">Spécifiez la version du service utilisée pour communiquer avec le serveur Isabel.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-135">Specify the service version that is used to communicate with the Isabel server.</span></span>|  

3.  <span data-ttu-id="fe6a9-136">Dans le raccourci **Télécharger**, remplissez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-136">On the **Upload** FastTab, fill in the fields as described in the following table.</span></span>   

    |<span data-ttu-id="fe6a9-137">Champ</span><span class="sxs-lookup"><span data-stu-id="fe6a9-137">Field</span></span>|<span data-ttu-id="fe6a9-138">Description</span><span class="sxs-lookup"><span data-stu-id="fe6a9-138">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="fe6a9-139">**Mode d'intégration du téléchargement (amont)**</span><span class="sxs-lookup"><span data-stu-id="fe6a9-139">**Upload integration Mode**</span></span>|<span data-ttu-id="fe6a9-140">Spécifiez le mode que vous souhaitez utiliser pour télécharger du contenu sur le serveur Isabel.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-140">Specify the mode that you want to use to upload content to the Isabel server.</span></span> <span data-ttu-id="fe6a9-141">Les options du mode d'intégration incluent **Interactif** et **Manuel**.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-141">The integration mode options include **Attended** and **Manual**.</span></span> <span data-ttu-id="fe6a9-142">Si le mode d'intégration est défini sur **Interactif**, vous devez définir le champ **Version IBS** sur **6**.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-142">If the integration mode is set to **Attended**, you must set the **IBS Version** field to **6**.</span></span> <span data-ttu-id="fe6a9-143">Les écritures de la table **Journal IBS** seront créées lorsque les fichiers paiement seront générés.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-143">The entries in the **IBS Log** table will be created when payment files are generated.</span></span> <span data-ttu-id="fe6a9-144">Si le mode d'intégration est défini sur **Manuel**, vous devez vous connecter au serveur Isabel manuellement, et aucune écriture ne sera créée.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-144">If the integration mode is set to **Manual**, you must log on to the Isabel server manually and no log entries will be created.</span></span>|  
    |<span data-ttu-id="fe6a9-145">**Chemin du téléchargement (amont)**</span><span class="sxs-lookup"><span data-stu-id="fe6a9-145">**Upload Path**</span></span>|<span data-ttu-id="fe6a9-146">Spécifiez le chemin d'accès au dossier où les fichiers sont enregistrés au cours du téléchargement sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-146">Specify the path to the folder where the files will be saved during the upload process.</span></span>|  

4.  <span data-ttu-id="fe6a9-147">Dans le raccourci **Télécharger**, remplissez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-147">On the **Download** FastTab, fill in the fields as described in the following table.</span></span>   

    |<span data-ttu-id="fe6a9-148">Champ</span><span class="sxs-lookup"><span data-stu-id="fe6a9-148">Field</span></span>|<span data-ttu-id="fe6a9-149">Description</span><span class="sxs-lookup"><span data-stu-id="fe6a9-149">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="fe6a9-150">**Mode d'intégration du téléchargement (aval)**</span><span class="sxs-lookup"><span data-stu-id="fe6a9-150">**Download integration Mode**</span></span>|<span data-ttu-id="fe6a9-151">Spécifiez le mode que vous souhaitez utiliser pour télécharger du contenu sur le serveur Isabel.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-151">Specify the mode that you want to use to download content to the Isabel server.</span></span> <span data-ttu-id="fe6a9-152">Les options incluent **Interactif** et **Manuel**.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-152">The options include **Attended** and **Manual**.</span></span> <span data-ttu-id="fe6a9-153">Si le mode d'intégration est défini sur **Interactif**, vous devez définir le champ **Version IBS** sur **6**.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-153">If the integration mode is set to **Attended**, you must set the **IBS Version** field to **6**.</span></span> <span data-ttu-id="fe6a9-154">Les écritures de la table **Journal IBS** seront créées à l'issue du téléchargement.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-154">The entries in the **IBS Log** table will be created when the download is performed.</span></span> <span data-ttu-id="fe6a9-155">Si le mode d'intégration est défini sur **Manuel**, vous devez vous connecter au serveur Isabel manuellement, et aucune écriture ne sera créée.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-155">If the integration mode is set to **Manual**, you must log on to the Isabel server manually and no log entries will be created.</span></span>|  
    |<span data-ttu-id="fe6a9-156">**Chemin du téléchargement (aval)**</span><span class="sxs-lookup"><span data-stu-id="fe6a9-156">**Download Path**</span></span>|<span data-ttu-id="fe6a9-157">Spécifiez le chemin d'accès au dossier où les fichiers sont enregistrés au cours du téléchargement depuis le serveur.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-157">Specify the path to the folder where the files will be saved during the download process.</span></span>|  

5.  <span data-ttu-id="fe6a9-158">Dans le raccourci **Numérotation**, remplissez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-158">On the **Numbering** FastTab, fill in the fields as described in the following table.</span></span>   

    |<span data-ttu-id="fe6a9-159">Champ</span><span class="sxs-lookup"><span data-stu-id="fe6a9-159">Field</span></span>|<span data-ttu-id="fe6a9-160">Description</span><span class="sxs-lookup"><span data-stu-id="fe6a9-160">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="fe6a9-161">**Nos de téléchargement (amont) du journal IBS**</span><span class="sxs-lookup"><span data-stu-id="fe6a9-161">**IBS Log Upload Nos.**</span></span>|<span data-ttu-id="fe6a9-162">Spécifiez la souche de numéros utilisée pour les écritures journal Isabel qui sont créées au cours du téléchargement sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-162">Specify the number series that is used for Isabel log entries created during the file upload process.</span></span>|  
    |<span data-ttu-id="fe6a9-163">**Nos de téléchargement (aval) du journal IBS**</span><span class="sxs-lookup"><span data-stu-id="fe6a9-163">**IBS Log Download Nos.**</span></span>|<span data-ttu-id="fe6a9-164">Spécifiez la souche de numéros utilisée pour les écritures journal Isabel qui sont créées au cours du téléchargement des fichiers du serveur.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-164">Specify the number series that is used for Isabel log entries created during the file download process.</span></span>|  
    |<span data-ttu-id="fe6a9-165">**ID demande IBS**</span><span class="sxs-lookup"><span data-stu-id="fe6a9-165">**IBS Request ID**</span></span>|<span data-ttu-id="fe6a9-166">Spécifiez une séquence de numéros utilisée pour la numérotation automatique et unique des demandes.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-166">Specify a number sequence used for automatic and unique numbering of the requests.</span></span>|  

6.  <span data-ttu-id="fe6a9-167">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-167">Choose the **OK** button.</span></span>  

<span data-ttu-id="fe6a9-168">Si vous le souhaitez, vous pouvez attribuer des comptes bancaires à chaque client et à chaque fournisseur.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-168">Optionally, you can assign bank accounts to each customer and vendor.</span></span> <span data-ttu-id="fe6a9-169">Cela facilite les paiements électroniques.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-169">This helps make electronic payments simpler.</span></span> <span data-ttu-id="fe6a9-170">La procédure suivante est consacrée à l'attribution de comptes bancaires préférés aux clients, mais les mêmes instructions s'appliquent aux fournisseurs.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-170">The following procedure explains how to assign preferred bank accounts to customers, but the same steps also apply to vendors.</span></span>  

## <a name="to-add-a-preferred-bank-account-to-a-customer"></a><span data-ttu-id="fe6a9-171">Pour ajouter un compte bancaire préféré à un client</span><span class="sxs-lookup"><span data-stu-id="fe6a9-171">To add a preferred bank account to a customer</span></span>  

1.  <span data-ttu-id="fe6a9-172">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Clients**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-172">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="fe6a9-173">Sélectionnez un client, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-173">Select a customer, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="fe6a9-174">Dans le raccourci **Paiements**, entrez le **Compte bancaire préféré**, puis cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-174">On the **Payments** FastTab, enter the **Preferred Bank Account**, and then choose the **OK** button.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="fe6a9-175">Pour tous les paiements, utilisez un compte bancaire par client ou par fournisseur.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-175">For all payments, use one bank account for each customer or vendor.</span></span>  

4.  <span data-ttu-id="fe6a9-176">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-176">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fe6a9-177">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fe6a9-177">See Also</span></span>  
 <span data-ttu-id="fe6a9-178">[Site Web Isabel](http://go.microsoft.com/fwlink/?LinkId=210323) </span><span class="sxs-lookup"><span data-stu-id="fe6a9-178">[Isabel website](http://go.microsoft.com/fwlink/?LinkId=210323) </span></span>  
 <span data-ttu-id="fe6a9-179">[Banque électronique belge](belgian-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="fe6a9-179">[Belgian Electronic Banking](belgian-electronic-banking.md) </span></span>  
 <span data-ttu-id="fe6a9-180">[Paiements électroniques belges](belgian-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="fe6a9-180">[Belgian Electronic Payments](belgian-electronic-payments.md) </span></span>  
 <span data-ttu-id="fe6a9-181">[Comment configurer les codes transaction IBLC/BLWI](how-to-set-up-iblc-blwi-transaction-codes.md) </span><span class="sxs-lookup"><span data-stu-id="fe6a9-181">[How to: Set Up IBLC-BLWI Transaction Codes](how-to-set-up-iblc-blwi-transaction-codes.md) </span></span>  
 <span data-ttu-id="fe6a9-182">[Comment configurer les fournisseurs pour les propositions de paiement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="fe6a9-182">[How to: Set Up Vendors for Automatic Payment Suggestions](how-to-set-up-vendors-for-automatic-payment-suggestions.md) </span></span>  
 <span data-ttu-id="fe6a9-183">[Comment générer des propositions de paiement](how-to-generate-payment-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="fe6a9-183">[How to: Generate Payment Suggestions](how-to-generate-payment-suggestions.md) </span></span>  
 <span data-ttu-id="fe6a9-184">[Comment créer des modèles et lots feuille paiement](how-to-create-payment-journal-templates-and-batches.md) </span><span class="sxs-lookup"><span data-stu-id="fe6a9-184">[How to: Create Payment Journal Templates and Batches](how-to-create-payment-journal-templates-and-batches.md) </span></span>  
 <span data-ttu-id="fe6a9-185">[Comment tester les paiements électroniques](how-to-test-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="fe6a9-185">[How to: Test Electronic Payments](how-to-test-electronic-payments.md) </span></span>  
 <span data-ttu-id="fe6a9-186">[Comment gérer les lignes paiement électronique](how-to-manage-electronic-payment-lines.md) </span><span class="sxs-lookup"><span data-stu-id="fe6a9-186">[How to: Manage Electronic Payment Lines](how-to-manage-electronic-payment-lines.md) </span></span>  
 [<span data-ttu-id="fe6a9-187">Comment imprimer les fichiers paiement</span><span class="sxs-lookup"><span data-stu-id="fe6a9-187">How to: Print Payment Files</span></span>](how-to-print-payment-files.md)
