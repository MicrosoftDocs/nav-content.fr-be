---
title: "Comment transférer et valider automatiquement les relevés CODA"
description: "Après avoir lettré et traité toutes les lignes relevé CODA, vous pouvez transférer les lignes relevé CODA vers une feuille financière."
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
ms.openlocfilehash: 024ca5788726079d6e6915635ae24ee44b68847b
ms.contentlocale: fr-be
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-automatically-transfer-and-post-coda-statements"></a><span data-ttu-id="cfd67-103">Comment transférer et valider automatiquement les relevés CODA</span><span class="sxs-lookup"><span data-stu-id="cfd67-103">How to: Automatically Transfer and Post CODA Statements</span></span>
<span data-ttu-id="cfd67-104">Après avoir lettré et traité toutes les lignes relevé CODA, vous pouvez transférer les lignes relevé CODA vers une feuille financière.</span><span class="sxs-lookup"><span data-stu-id="cfd67-104">After you have applied and processed all CODA statement lines, you can transfer the CODA statement lines to a financial journal.</span></span>  

<span data-ttu-id="cfd67-105">Après avoir transféré les lignes relevé, vous pouvez valider les lignes vers une feuille comptabilité correspondante.</span><span class="sxs-lookup"><span data-stu-id="cfd67-105">After transferring the statement lines, you can post the lines in a corresponding general journal.</span></span> <span data-ttu-id="cfd67-106">S'il n'existe aucune feuille comptabilité, vous ne pouvez pas transférer les lignes.</span><span class="sxs-lookup"><span data-stu-id="cfd67-106">If no such general journal exists, you cannot transfer the lines.</span></span> <span data-ttu-id="cfd67-107">Vous pouvez créer une feuille pour traiter les relevés CODA.</span><span class="sxs-lookup"><span data-stu-id="cfd67-107">You can create a journal to handle CODA statements.</span></span> <span data-ttu-id="cfd67-108">Pour plus d'informations, voir [Comment créer des feuilles financières](how-to-create-financial-journals.md).</span><span class="sxs-lookup"><span data-stu-id="cfd67-108">For more information, see [How to: Create Financial Journals](how-to-create-financial-journals.md).</span></span>  

<span data-ttu-id="cfd67-109">Vous pouvez aussi transférer et valider manuellement les relevés CODA.</span><span class="sxs-lookup"><span data-stu-id="cfd67-109">Alternatively, you can manually transfer and post CODA statements.</span></span> <span data-ttu-id="cfd67-110">Pour plus d'informations, voir [Comment transférer et valider manuellement les relevés CODA](how-to-manually-transfer-and-post-coda-statements.md).</span><span class="sxs-lookup"><span data-stu-id="cfd67-110">For information, see [How to: Manually Transfer and Post CODA Statements](how-to-manually-transfer-and-post-coda-statements.md).</span></span>  

## <a name="to-automatically-transfer-statement-lines"></a><span data-ttu-id="cfd67-111">Pour transférer automatiquement les lignes relevé</span><span class="sxs-lookup"><span data-stu-id="cfd67-111">To automatically transfer statement lines</span></span>  

1.  <span data-ttu-id="cfd67-112">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Comptes bancaires**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="cfd67-112">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="cfd67-113">Sélectionnez le compte bancaire, puis choisissez l'action **Relevés CODA**.</span><span class="sxs-lookup"><span data-stu-id="cfd67-113">Select the bank account, and then choose **CODA Statements** action.</span></span>  
3.  <span data-ttu-id="cfd67-114">Sélectionnez le relevé CODA, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="cfd67-114">Select the CODA statement, and then choose the **Edit** action.</span></span>  
4.  <span data-ttu-id="cfd67-115">Choisissez l'action **Transférer à FS**.</span><span class="sxs-lookup"><span data-stu-id="cfd67-115">Choose the **Transfer to General Ledger** action.</span></span>  
5.  <span data-ttu-id="cfd67-116">Cliquez sur le bouton **Oui**.</span><span class="sxs-lookup"><span data-stu-id="cfd67-116">Choose the **Yes** button.</span></span>  

<span data-ttu-id="cfd67-117">Le traitement par lots transfèrera à présent les lignes relevé CODA à la feuille financière.</span><span class="sxs-lookup"><span data-stu-id="cfd67-117">The batch job will now transfer the CODA statement lines to the financial journal.</span></span>  

<span data-ttu-id="cfd67-118">Après avoir transféré les lignes relevé vers la feuille, vous pouvez valider les lignes relevé vers la feuille financière correspondante.</span><span class="sxs-lookup"><span data-stu-id="cfd67-118">After transferring the statement lines to the journal, you can post the statement lines in the corresponding financial journal.</span></span>  

## <a name="see-also"></a><span data-ttu-id="cfd67-119">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cfd67-119">See Also</span></span>  
 <span data-ttu-id="cfd67-120">[Relevés bancaires CODA](coda-bank-statements.md) </span><span class="sxs-lookup"><span data-stu-id="cfd67-120">[CODA Bank Statements](coda-bank-statements.md) </span></span>  
 <span data-ttu-id="cfd67-121">[Comment importer les relevés CODA](how-to-import-coda-statements.md) </span><span class="sxs-lookup"><span data-stu-id="cfd67-121">[How to: Import CODA Statements](how-to-import-coda-statements.md) </span></span>  
 <span data-ttu-id="cfd67-122">[Comment lettrer les relevés CODA](how-to-apply-coda-statements.md) </span><span class="sxs-lookup"><span data-stu-id="cfd67-122">[How to: Apply CODA Statements](how-to-apply-coda-statements.md) </span></span>  
 <span data-ttu-id="cfd67-123">[Comment créer des feuilles financières](how-to-create-financial-journals.md) </span><span class="sxs-lookup"><span data-stu-id="cfd67-123">[How to: Create Financial Journals](how-to-create-financial-journals.md) </span></span>  
 <span data-ttu-id="cfd67-124">[Comment transférer et valider manuellement les relevés CODA](how-to-manually-transfer-and-post-coda-statements.md).</span><span class="sxs-lookup"><span data-stu-id="cfd67-124">[How to: Manually Transfer and Post CODA Statements](how-to-manually-transfer-and-post-coda-statements.md)</span></span>

