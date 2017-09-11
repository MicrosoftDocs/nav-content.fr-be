---
title: "Procédure : utilisation des chèques"
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
ms.openlocfilehash: 421516a7580a90d6eabc8ecfcc841215839994c9
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-work-with-checks"></a><span data-ttu-id="af7e0-102">Procédure : utilisation des chèques</span><span class="sxs-lookup"><span data-stu-id="af7e0-102">How to: Work With Checks</span></span>
<span data-ttu-id="af7e0-103">Dynamics NAV prend en charge l'émission électronique et manuelle de chèques.</span><span class="sxs-lookup"><span data-stu-id="af7e0-103">Dynamics NAV supports electronic and manual check issuance.</span></span> <span data-ttu-id="af7e0-104">Ces deux méthodes utilisent la feuille paiement pour émettre des chèques aux fournisseurs.</span><span class="sxs-lookup"><span data-stu-id="af7e0-104">Both methods use the payment journal to issue checks to vendors.</span></span> <span data-ttu-id="af7e0-105">Vous pouvez également annuler des chèques et afficher les écritures comptables chèque.</span><span class="sxs-lookup"><span data-stu-id="af7e0-105">You can also void checks and view check ledger entries.</span></span>

<span data-ttu-id="af7e0-106">La procédure d'émission de chèques propose des paiements, crée des écritures comptables et imprime les chèques informatiques.</span><span class="sxs-lookup"><span data-stu-id="af7e0-106">The process of issuing checks suggests payments, creates ledger entries, and prints the computer checks.</span></span>

<span data-ttu-id="af7e0-107">Votre imprimante doit être correctement configurée pour les formulaires chèque, et vous devez définir la mise en page de chèque à utiliser.</span><span class="sxs-lookup"><span data-stu-id="af7e0-107">Your printer must be correctly set up with the check forms, and you must define which check layout to use.</span></span> <span data-ttu-id="af7e0-108">Pour plus d'informations, reportez-vous à [Procédure : définir les mises en page de chèques](finance-setup-how-define-check-layouts.md)</span><span class="sxs-lookup"><span data-stu-id="af7e0-108">For more information, see [How to: Define Check Layouts](finance-setup-how-define-check-layouts.md)</span></span>

## <a name="to-issue-checks"></a><span data-ttu-id="af7e0-109">Pour émettre des chèques</span><span class="sxs-lookup"><span data-stu-id="af7e0-109">To issue checks</span></span>
1. <span data-ttu-id="af7e0-110">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Feuilles paiement**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="af7e0-110">In the top right corner, choose the **Search for Page or Report** icon, enter **Payment Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="af7e0-111">Remplissez la feuille avec les paiements appropriés, par exemple à l'aide de la fonction Proposer paiements fournisseur.</span><span class="sxs-lookup"><span data-stu-id="af7e0-111">Fill in the journal with relevant payments, for example by using the Suggest Vendor Payments function.</span></span> <span data-ttu-id="af7e0-112">Pour plus d'informations, reportez vous à [Procédure : proposer des paiements fournisseur](payables-how-suggest-vendor-payments.md).</span><span class="sxs-lookup"><span data-stu-id="af7e0-112">For more information, see [How to: Suggest Vendor Payments](payables-how-suggest-vendor-payments.md).</span></span>
3. <span data-ttu-id="af7e0-113">Dans le champ **Mode émission paiement** des lignes feuille pour le paiement que vous souhaitez effectuer avec des chèques, sélectionnez l'une des options suivantes :</span><span class="sxs-lookup"><span data-stu-id="af7e0-113">In the **Bank Payment Type** field on journal lines for payment that you want to make with checks, select one of the following options:</span></span>

 - <span data-ttu-id="af7e0-114">**Informatique** : sélectionnez cette option si vous souhaitez imprimer un chèque du montant de la ligne feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="af7e0-114">**Computer Check**: Select this option if you want to print a check for the amount on the payment journal line.</span></span> <span data-ttu-id="af7e0-115">Vous devez imprimer les chèques avant de pouvoir valider les lignes feuille.</span><span class="sxs-lookup"><span data-stu-id="af7e0-115">You must print the checks before you can post the journal lines.</span></span> <span data-ttu-id="af7e0-116">Vous pouvez uniquement sélectionner **Informatique** si le **Type compte contrepartie** ou le **Type compte** est **Compte bancaire**.</span><span class="sxs-lookup"><span data-stu-id="af7e0-116">You can only select **Computer Check** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span></span>

 - <span data-ttu-id="af7e0-117">**Manuel** : sélectionnez cette option si vous avez créé un chèque manuellement et que vous souhaitez créer une écriture comptable chèque correspondante de ce montant.</span><span class="sxs-lookup"><span data-stu-id="af7e0-117">**Manual Check**: Select this option if you have created a check manually and want to create a corresponding check ledger entry for this amount.</span></span> <span data-ttu-id="af7e0-118">Si vous utilisez cette option, vous ne pouvez pas imprimer de chèque à partir de Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="af7e0-118">By using this option, you cannot print checks from Dynamics NAV.</span></span> <span data-ttu-id="af7e0-119">Vous pouvez uniquement sélectionner **Manuel** si le **Type compte contrepartie** ou le **Type compte** est **Compte bancaire**.</span><span class="sxs-lookup"><span data-stu-id="af7e0-119">You can only select **Manual Check** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span></span>

    <span data-ttu-id="af7e0-120">**Remarque** : vous devez imprimer les chèques informatiques avant de valider les lignes feuille correspondantes.</span><span class="sxs-lookup"><span data-stu-id="af7e0-120">**Note**: You must print computer checks before you post the related journal lines.</span></span>
4. <span data-ttu-id="af7e0-121">Dans le cas de chèques informatiques, sélectionnez **Imprimer chèque**.</span><span class="sxs-lookup"><span data-stu-id="af7e0-121">In case of computer checks, choose **Print Check**.</span></span>
5. <span data-ttu-id="af7e0-122">Dans la fenêtre **Chèque**, renseignez les champs selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="af7e0-122">In the **Check** window, fill in the fields as necessary.</span></span> <span data-ttu-id="af7e0-123">Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.</span><span class="sxs-lookup"><span data-stu-id="af7e0-123">Choose a field to read a short description of the field or link to more information.</span></span>
6. <span data-ttu-id="af7e0-124">Cliquez sur le bouton **Imprimer**.</span><span class="sxs-lookup"><span data-stu-id="af7e0-124">Choose the **Print** button.</span></span>

<span data-ttu-id="af7e0-125">**Remarque** : si vous souhaitez imprimer des chèques en plusieurs devises sur des comptes bancaires différents, vous devez exécuter le traitement par lots **Imprimer chèque** pour chacune de ces devises et préciser le compte bancaire concerné.</span><span class="sxs-lookup"><span data-stu-id="af7e0-125">**Note**: If you want to print checks in more than one currency from different bank accounts, you must run the **Print Check** batch job separately for each currency and specify the appropriate bank account.</span></span>

## <a name="to-cancel-printed-checks-that-are-not-posted"></a><span data-ttu-id="af7e0-126">Pour annuler des chèques imprimés qui ne sont pas validés</span><span class="sxs-lookup"><span data-stu-id="af7e0-126">To cancel printed checks that are not posted</span></span>
<span data-ttu-id="af7e0-127">Vous pouvez annuler des chèques non validés après leur impression par l'intermédiaire de l'action **Annuler chèque** de la fenêtre **Feuille paiement**.</span><span class="sxs-lookup"><span data-stu-id="af7e0-127">You can cancel non-posted checks after they have been printed by using the **Void Check** action in the **Payment Journal** window.</span></span>
1. <span data-ttu-id="af7e0-128">Dans la fenêtre **Feuille paiement**, sélectionnez **Annuler chèque**, puis sélectionnez les chèques à annuler.</span><span class="sxs-lookup"><span data-stu-id="af7e0-128">In the **Payment Journal** window, choose the **Void Check**, and then choose which checks to cancel.</span></span>

## <a name="to-void-checks"></a><span data-ttu-id="af7e0-129">Pour annuler des chèques</span><span class="sxs-lookup"><span data-stu-id="af7e0-129">To void checks</span></span>
<span data-ttu-id="af7e0-130">Lorsque des paiements par chèque ont été validés, vous pouvez uniquement annuler des chèques à partir des écritures comptables banque ainsi obtenues.</span><span class="sxs-lookup"><span data-stu-id="af7e0-130">When check payment have been posted, you can only cancel (void) checks from the resulting bank ledger entries.</span></span>

1. <span data-ttu-id="af7e0-131">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Comptes bancaires**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="af7e0-131">In the top right corner, choose the **Search for Page or Report** icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="af7e0-132">Sélectionnez le compte bancaire approprié, sélectionnez l'action **Modifier**, puis l'action **Écritures comptables chèque**.</span><span class="sxs-lookup"><span data-stu-id="af7e0-132">Select the relevant bank account, choose the **Edit** action, and then choose the **Check Ledger Entries** action.</span></span>
3. <span data-ttu-id="af7e0-133">Dans la fenêtre **Écritures comptables chèque**, sélectionnez l'action **Annuler chèque**.</span><span class="sxs-lookup"><span data-stu-id="af7e0-133">In the **Check Ledger Entries** window, choose the **Void Check** action.</span></span>
4. <span data-ttu-id="af7e0-134">Cochez la case **Annuler chèque uniquement**.</span><span class="sxs-lookup"><span data-stu-id="af7e0-134">Select the **Void Check Only** check box.</span></span>
5. <span data-ttu-id="af7e0-135">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="af7e0-135">Choose the **OK**button.</span></span>

## <a name="see-also"></a><span data-ttu-id="af7e0-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="af7e0-136">See Also</span></span>
[<span data-ttu-id="af7e0-137">Gestion des comptes fournisseur</span><span class="sxs-lookup"><span data-stu-id="af7e0-137">Manage Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="af7e0-138">Configuration des opérations bancaires</span><span class="sxs-lookup"><span data-stu-id="af7e0-138">Set Up Banking</span></span>](bank-setup-banking.md)  

