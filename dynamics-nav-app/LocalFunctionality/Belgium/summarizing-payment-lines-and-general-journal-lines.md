---
title: "Récapitulatif des lignes paiements et des lignes feuille comptabilité"
description: "[!INCLUDE[navnow](../../includes/navnow_md.md)] traite différents types de transactions de la même manière."
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
ms.openlocfilehash: 80baa8f0f21cfac16fe522ea3a4ba606fb872cf1
ms.contentlocale: fr-be
ms.lasthandoff: 12/01/2017

---
# <a name="summarizing-payment-lines-and-general-journal-lines"></a><span data-ttu-id="84359-103">Récapitulatif des lignes paiements et des lignes feuille comptabilité</span><span class="sxs-lookup"><span data-stu-id="84359-103">Summarizing Payment Lines and General Journal Lines</span></span>
<span data-ttu-id="84359-104">[!INCLUDE[navnow](../../includes/navnow_md.md)] traite les différents types de transactions de la même manière :</span><span class="sxs-lookup"><span data-stu-id="84359-104">In [!INCLUDE[navnow](../../includes/navnow_md.md)] handles the following types of transactions in the same way:</span></span>  

- <span data-ttu-id="84359-105">Paiements intérieurs</span><span class="sxs-lookup"><span data-stu-id="84359-105">Domestic payments</span></span>  
- <span data-ttu-id="84359-106">Paiements étrangers</span><span class="sxs-lookup"><span data-stu-id="84359-106">International payments</span></span>  
- <span data-ttu-id="84359-107">Paiements SEPA</span><span class="sxs-lookup"><span data-stu-id="84359-107">SEPA payments</span></span>  
- <span data-ttu-id="84359-108">Paiements SEPA non libellés en Euro</span><span class="sxs-lookup"><span data-stu-id="84359-108">Non-euro SEPA payments</span></span>  

## <a name="how-payment-journal-lines-are-transferred-to-the-general-journal"></a><span data-ttu-id="84359-109">Comment les lignes feuille paiement sont transférées dans la feuille comptabilité</span><span class="sxs-lookup"><span data-stu-id="84359-109">How Payment Journal Lines are Transferred to the General Journal</span></span>  
<span data-ttu-id="84359-110">Lorsque vous exportez les lignes feuille paiement dans un fichier, [!INCLUDE[navnow](../../includes/navnow_md.md)] transfère les lignes feuille paiement dans la feuille comptabilité spécifiée.</span><span class="sxs-lookup"><span data-stu-id="84359-110">When you export the payment journal lines to a file, [!INCLUDE[navnow](../../includes/navnow_md.md)] transfers the payment journal lines to the specified general journal.</span></span> <span data-ttu-id="84359-111">Par défaut, une ligne feuille comptabilité est créée pour chaque ligne feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="84359-111">By default, a general journal line is created for each payment journal line.</span></span>  

<span data-ttu-id="84359-112">Les deux champs suivants dans la fenêtre **Configuration de la banque électronique** affectent la manière dont sont résumées les lignes paiement.</span><span class="sxs-lookup"><span data-stu-id="84359-112">The following two fields in the **Electronic Banking Setup** window affect how the payment lines are summarized:</span></span>  

- <span data-ttu-id="84359-113">**Résumer lignes FS**</span><span class="sxs-lookup"><span data-stu-id="84359-113">**Summarize Gen. Jnl. Lines**</span></span>  
- <span data-ttu-id="84359-114">**Couper comm. de paiement**</span><span class="sxs-lookup"><span data-stu-id="84359-114">**Cut off Payment Message Texts**</span></span>  

<span data-ttu-id="84359-115">Si vous avez sélectionné la case à cocher **Résumer lignes FS** dans la fenêtre **Configuration de la banque électronique**, [!INCLUDE[navnow](../../includes/navnow_md.md)] résume toutes les lignes feuille paiement pour un fournisseur spécifique sur une ligne feuille comptabilité.</span><span class="sxs-lookup"><span data-stu-id="84359-115">If you have selected the **Summarize Gen. Jnl. Lines** check box in the **Electronic Banking Setup** window, [!INCLUDE[navnow](../../includes/navnow_md.md)] summarizes all payment journal lines for a specific vendor into one general journal line.</span></span> <span data-ttu-id="84359-116">La description générale « Paiement %1 », où %1 est le numéro du fournisseur, est utilisée pour la description de la ligne feuille résumée.</span><span class="sxs-lookup"><span data-stu-id="84359-116">The general description "Payment %1," where %1 is the vendor number, is used for the summarized journal line description.</span></span> <span data-ttu-id="84359-117">Une ligne paiement et une ligne feuille comptabilité distinctes sont créées pour traiter :</span><span class="sxs-lookup"><span data-stu-id="84359-117">A separate payment line and a separate general journal line are created to handle:</span></span>  

- <span data-ttu-id="84359-118">Les lignes feuille paiement qui contiennent des paiements partiels, avec les champs **Paiement partiel** et **Ligne individuelle** sélectionnés.</span><span class="sxs-lookup"><span data-stu-id="84359-118">Payment journal lines that contain partial payments, with both the **Partial Payment** and the **Separate Line** fields selected.</span></span>  

- <span data-ttu-id="84359-119">Les lignes feuille paiement qui contiennent une communication structurée (a réussi le test MOD97), qui définit **Communication structurée** sur True dans la feuille bancaire électronique.</span><span class="sxs-lookup"><span data-stu-id="84359-119">Payment journal lines that contain a standard format message (that is, passes the MOD97 test), which sets **Standard Format Message** to True in the electronic banking journal.</span></span>  

## <a name="example-1"></a><span data-ttu-id="84359-120">Exemple 1</span><span class="sxs-lookup"><span data-stu-id="84359-120">Example 1</span></span>  
<span data-ttu-id="84359-121">Dans cet exemple, vous exportez les lignes paiement et la case à cocher **Résumer lignes FS** est sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="84359-121">In this example, you export payment lines, and the **Summarize Gen. Jnl. Lines** check box is selected.</span></span> [!INCLUDE[navnow](../../includes/navnow_md.md)]<span data-ttu-id="84359-122"> crée :</span><span class="sxs-lookup"><span data-stu-id="84359-122"> creates:</span></span>  

- <span data-ttu-id="84359-123">Une ligne paiement combinée dans un fichier XML qui contient une communication concaténée.</span><span class="sxs-lookup"><span data-stu-id="84359-123">One combined payment line in a XML file that has a concatenated payment message.</span></span> <span data-ttu-id="84359-124">Un espace blanc est le délimiteur.</span><span class="sxs-lookup"><span data-stu-id="84359-124">White space is the delimiter.</span></span>  
- <span data-ttu-id="84359-125">Une ligne paiement dans la feuille comptabilité avec une description générique qui inclut le nom du fournisseur.</span><span class="sxs-lookup"><span data-stu-id="84359-125">One payment line in the general journal with a generic description that ../../includes the vendor name.</span></span>  

## <a name="example-2"></a><span data-ttu-id="84359-126">Exemple 2</span><span class="sxs-lookup"><span data-stu-id="84359-126">Example 2</span></span>  
<span data-ttu-id="84359-127">Dans cet exemple, vous exportez les lignes paiement et la case à cocher **Résumer lignes FS** est sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="84359-127">In this example, you export payment lines, and the **Summarize Gen. Jnl. Lines** check box is selected.</span></span> <span data-ttu-id="84359-128">La case à cocher **Couper comm. de paiement** est désélectionnée, et les lignes paiement SEPA et SEPA non libellées en Euro combinées dépassent 140 caractères dans la communication.</span><span class="sxs-lookup"><span data-stu-id="84359-128">The **Cut off Payment Message Texts** check box is cleared, and combined SEPA and non-euro SEPA payment lines exceed 140 characters in payment message.</span></span> [!INCLUDE[navnow](../../includes/navnow_md.md)]<span data-ttu-id="84359-129"> crée :</span><span class="sxs-lookup"><span data-stu-id="84359-129"> creates:</span></span>  

- <span data-ttu-id="84359-130">Deux lignes paiement combinées dans un fichier XML.</span><span class="sxs-lookup"><span data-stu-id="84359-130">Two combined payment lines in a XML file.</span></span> <span data-ttu-id="84359-131">La première ligne paiement contient les premières communications concaténées.</span><span class="sxs-lookup"><span data-stu-id="84359-131">The first payment line contains the first concatenated payment messages.</span></span> <span data-ttu-id="84359-132">La deuxième ligne paiement contient la communication de la troisième ligne.</span><span class="sxs-lookup"><span data-stu-id="84359-132">The second payment line contains the payment message from the third line.</span></span>  

- <span data-ttu-id="84359-133">Une ligne paiement dans la feuille comptabilité avec une description générique qui inclut le nom du fournisseur.</span><span class="sxs-lookup"><span data-stu-id="84359-133">One payment line in the general journal with a generic description that ../../includes the vendor name.</span></span>  

## <a name="example-3"></a><span data-ttu-id="84359-134">Exemple 3</span><span class="sxs-lookup"><span data-stu-id="84359-134">Example 3</span></span>  
<span data-ttu-id="84359-135">Dans cet exemple, vous exportez les lignes paiement et la case à cocher **Résumer lignes FS** est sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="84359-135">In this example, you export payment lines, and the **Summarize Gen. Jnl. Lines** check box is selected.</span></span> <span data-ttu-id="84359-136">La case à cocher **Couper comm. de paiement** est également sélectionnée, et les lignes paiement SEPA et SEPA non libellées en Euro combinées dépassent 140 caractères dans la communication.</span><span class="sxs-lookup"><span data-stu-id="84359-136">The **Cut off Payment Message Texts** check box is also selected and combined SEPA and non-SEPA payment lines exceed 140 characters in payment message.</span></span> [!INCLUDE[navnow](../../includes/navnow_md.md)]<span data-ttu-id="84359-137"> crée :</span><span class="sxs-lookup"><span data-stu-id="84359-137"> creates:</span></span>  

- <span data-ttu-id="84359-138">Une ligne paiement combinée dans un fichier XML qui contient deux communications concaténées.</span><span class="sxs-lookup"><span data-stu-id="84359-138">One combined payment line in a XML file that has two concatenated payment messages.</span></span> <span data-ttu-id="84359-139">Des points de suspension (...) sont utilisés pour indiquer que le message est tronqué.</span><span class="sxs-lookup"><span data-stu-id="84359-139">An ellipsis (…) is used to indicate that the message is truncated.</span></span>  

- <span data-ttu-id="84359-140">Une ligne paiement dans la feuille comptabilité avec une description générique qui inclut le nom du fournisseur.</span><span class="sxs-lookup"><span data-stu-id="84359-140">One payment line in the general journal with a generic description that includes the vendor name.</span></span>  

<span data-ttu-id="84359-141">Basés sur la structure XML, les paiements sont résumés par numéro de compte, numéro compte bancaire bénéficiaire et numéro compte bancaire. Le filtre compte bancaire peut être vide.</span><span class="sxs-lookup"><span data-stu-id="84359-141">Based on the XML structure, the payments are summarized per account number and beneficiary bank account no and bank account no. The bank account filter can be empty.</span></span>  

<span data-ttu-id="84359-142">Le code EndToEndId dans le message SEPA est prélevé de la communication et peut être tronqué à la longueur maximale de 45 caractères.</span><span class="sxs-lookup"><span data-stu-id="84359-142">The EndToEndId in the SEPA message is taken from the payment message and can be truncated to the maximum length of 45 characters.</span></span>  

## <a name="see-also"></a><span data-ttu-id="84359-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="84359-143">See Also</span></span>  
 <span data-ttu-id="84359-144">[Comment configurer la banque électronique](how-to-set-up-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="84359-144">[How to: Set Up Electronic Banking](how-to-set-up-electronic-banking.md) </span></span>  
 [<span data-ttu-id="84359-145">Paramétrage de Finance</span><span class="sxs-lookup"><span data-stu-id="84359-145">Setting Up Finance</span></span>](../../finance-setup-finance.md)  
 [<span data-ttu-id="84359-146">Comment enregistrer des achats</span><span class="sxs-lookup"><span data-stu-id="84359-146">How to: Record Purchases</span></span>](../../purchasing-how-record-purchases.md) 

