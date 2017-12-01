---
title: "Comment tester les paiements électroniques"
description: "Après avoir configuré la banque électronique et généré des propositions de paiement, vous pouvez tester les lignes feuille paiement pour repérer les éventuelles erreurs avant de valider les lignes."
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
ms.openlocfilehash: aa042839fa0add2f8666d0146ef77165fa0c75eb
ms.contentlocale: fr-be
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-test-electronic-payments"></a><span data-ttu-id="79593-103">Comment tester les paiements électroniques</span><span class="sxs-lookup"><span data-stu-id="79593-103">How to: Test Electronic Payments</span></span>
<span data-ttu-id="79593-104">Après avoir configuré la banque électronique et généré des propositions de paiement, vous pouvez tester les lignes feuille paiement pour repérer les éventuelles erreurs avant de valider les lignes.</span><span class="sxs-lookup"><span data-stu-id="79593-104">After you have set up electronic banking and generated payment suggestions, you can test the payment journal lines for errors before posting them.</span></span>  

<span data-ttu-id="79593-105">Les informations validées incluent notamment :</span><span class="sxs-lookup"><span data-stu-id="79593-105">Some of the information that is validated includes:</span></span>  

- <span data-ttu-id="79593-106">Les numéros de comptes bancaires sont valides.</span><span class="sxs-lookup"><span data-stu-id="79593-106">Bank accounts numbers are valid.</span></span>  
- <span data-ttu-id="79593-107">Il y a des lignes paiement positives.</span><span class="sxs-lookup"><span data-stu-id="79593-107">Positive payment lines are present.</span></span>  
- <span data-ttu-id="79593-108">Si les paiements nationaux et internationaux sont effectués depuis un seul compte bancaire.</span><span class="sxs-lookup"><span data-stu-id="79593-108">If domestic and international payments are made from only one bank account.</span></span>  
- <span data-ttu-id="79593-109">Si un seul compte bancaire peut être utilisé pour Isabel.</span><span class="sxs-lookup"><span data-stu-id="79593-109">If only one bank account can be used for Isabel.</span></span>  
- <span data-ttu-id="79593-110">Si les lignes paiement sont en Euro pour SEPA.</span><span class="sxs-lookup"><span data-stu-id="79593-110">If payment lines are in Euro for SEPA.</span></span>  
- <span data-ttu-id="79593-111">Si une souche de numéros a été définie pour SEPA.</span><span class="sxs-lookup"><span data-stu-id="79593-111">If a number series has been defined for SEPA.</span></span>  

<span data-ttu-id="79593-112">Vous pouvez consulter les éventuelles erreurs dans la fenêtre **Exporter les journaux d'erreur de chèque**.</span><span class="sxs-lookup"><span data-stu-id="79593-112">You can view any errors in the **Export Check Error Logs** window.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="79593-113">Vous devez corriger toutes les erreurs avant de pouvoir valider les lignes.</span><span class="sxs-lookup"><span data-stu-id="79593-113">You have to correct all errors before you can post the lines.</span></span>  

## <a name="to-test-payment-journal-lines"></a><span data-ttu-id="79593-114">Pour tester les lignes feuille paiement</span><span class="sxs-lookup"><span data-stu-id="79593-114">To test payment journal lines</span></span>  

1.  <span data-ttu-id="79593-115">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Feuilles paiement**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="79593-115">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="79593-116">Dans le champ **Nom feuille**, sélectionnez la feuille concernée.</span><span class="sxs-lookup"><span data-stu-id="79593-116">In the **Batch Name** field, select the required journal batch.</span></span>  
3.  <span data-ttu-id="79593-117">Dans le champ **Protocole d'exportation**, sélectionnez le protocole d'exportation.</span><span class="sxs-lookup"><span data-stu-id="79593-117">In the **Export Protocol** field, select the export protocol.</span></span>  
4.  <span data-ttu-id="79593-118">Entrez les informations ligne feuille paiement, puis choisissez l'action **Vérifier les lignes de paiement** pour valider les lignes feuille paiement.</span><span class="sxs-lookup"><span data-stu-id="79593-118">Enter the payment journal line information, and then choose the **Check Payment Lines** action to validate the payment journal lines.</span></span> <span data-ttu-id="79593-119">La validation effectuée sur les lignes feuille dépend du type de contrôle indiqué dans la fenêtre **Protocoles d'exportation**.</span><span class="sxs-lookup"><span data-stu-id="79593-119">The validation that is performed on the journal lines depends on the type of check that is specified in the **Export Protocols** window.</span></span>  

## <a name="see-also"></a><span data-ttu-id="79593-120">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="79593-120">See Also</span></span>  
 <span data-ttu-id="79593-121">[Paiements électroniques belges](belgian-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="79593-121">[Belgian Electronic Payments](belgian-electronic-payments.md) </span></span>  
 <span data-ttu-id="79593-122">[Comment configurer les fournisseurs pour les propositions de paiement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="79593-122">[How to: Set Up Vendors for Automatic Payment Suggestions](how-to-set-up-vendors-for-automatic-payment-suggestions.md) </span></span>  
 <span data-ttu-id="79593-123">[Comment générer des propositions de paiement](how-to-generate-payment-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="79593-123">[How to: Generate Payment Suggestions](how-to-generate-payment-suggestions.md) </span></span>  
 [<span data-ttu-id="79593-124">Comment imprimer les fichiers paiement</span><span class="sxs-lookup"><span data-stu-id="79593-124">How to: Print Payment Files</span></span>](how-to-print-payment-files.md)

