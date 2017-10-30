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
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c8f6f049c3491860e5105456d689e7a3d4718d69
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-automatically-transfer-and-post-coda-statements"></a><span data-ttu-id="89d0f-103">Comment transférer et valider automatiquement les relevés CODA</span><span class="sxs-lookup"><span data-stu-id="89d0f-103">How to: Automatically Transfer and Post CODA Statements</span></span>
<span data-ttu-id="89d0f-104">Après avoir lettré et traité toutes les lignes relevé CODA, vous pouvez transférer les lignes relevé CODA vers une feuille financière.</span><span class="sxs-lookup"><span data-stu-id="89d0f-104">After you have applied and processed all CODA statement lines, you can transfer the CODA statement lines to a financial journal.</span></span>  
  
 <span data-ttu-id="89d0f-105">Après avoir transféré les lignes relevé, vous pouvez valider les lignes vers une feuille comptabilité correspondante.</span><span class="sxs-lookup"><span data-stu-id="89d0f-105">After transferring the statement lines, you can post the lines in a corresponding general journal.</span></span> <span data-ttu-id="89d0f-106">S'il n'existe aucune feuille comptabilité, vous ne pouvez pas transférer les lignes.</span><span class="sxs-lookup"><span data-stu-id="89d0f-106">If no such general journal exists, you cannot transfer the lines.</span></span> <span data-ttu-id="89d0f-107">Vous pouvez créer une feuille pour traiter les relevés CODA.</span><span class="sxs-lookup"><span data-stu-id="89d0f-107">You can create a journal to handle CODA statements.</span></span> <span data-ttu-id="89d0f-108">Pour plus d'informations, voir [Comment créer des feuilles financières](how-to-create-financial-journals.md).</span><span class="sxs-lookup"><span data-stu-id="89d0f-108">For more information, see [How to: Create Financial Journals](how-to-create-financial-journals.md).</span></span>  
  
 <span data-ttu-id="89d0f-109">Vous pouvez aussi transférer et valider manuellement les relevés CODA.</span><span class="sxs-lookup"><span data-stu-id="89d0f-109">Alternatively, you can manually transfer and post CODA statements.</span></span> <span data-ttu-id="89d0f-110">Pour plus d'informations, voir [Comment transférer et valider manuellement les relevés CODA](how-to-manually-transfer-and-post-coda-statements.md).</span><span class="sxs-lookup"><span data-stu-id="89d0f-110">For information, see [How to: Manually Transfer and Post CODA Statements](how-to-manually-transfer-and-post-coda-statements.md).</span></span>  
  
### <a name="to-automatically-transfer-statement-lines"></a><span data-ttu-id="89d0f-111">Pour transférer automatiquement les lignes relevé</span><span class="sxs-lookup"><span data-stu-id="89d0f-111">To automatically transfer statement lines</span></span>  
  
1.  <span data-ttu-id="89d0f-112">Sélectionnez l'icône ![Rechercher une page ou un état](media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Comptes bancaires**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="89d0f-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="89d0f-113">Sélectionnez le compte bancaire, puis, dans l'onglet **Accueil**, dans le groupe **Traiter**, sélectionnez **Relevés CODA**.</span><span class="sxs-lookup"><span data-stu-id="89d0f-113">Select the bank account, and on the **Home** tab, in the **Process** group, choose **CODA Statements**.</span></span>  
  
3.  <span data-ttu-id="89d0f-114">Sélectionnez le relevé CODA, puis, dans l'onglet **Accueil**, dans le groupe **Gérer**, sélectionnez **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="89d0f-114">Select the CODA statement, and on the **Home** tab, in the **Manage** group, choose **Edit**.</span></span>  
  
4.  <span data-ttu-id="89d0f-115">Dans l'onglet **Actions**, dans le groupe **Fonctions**, sélectionnez **Transférer à FS**.</span><span class="sxs-lookup"><span data-stu-id="89d0f-115">On the **Actions** tab, in the **Functions** group, choose **Transfer to General Ledger**.</span></span>  
  
5.  <span data-ttu-id="89d0f-116">Cliquez sur le bouton **Oui**.</span><span class="sxs-lookup"><span data-stu-id="89d0f-116">Choose the **Yes** button.</span></span>  
  
     <span data-ttu-id="89d0f-117">Le traitement par lots transfèrera à présent les lignes relevé CODA à la feuille financière.</span><span class="sxs-lookup"><span data-stu-id="89d0f-117">The batch job will now transfer the CODA statement lines to the financial journal.</span></span>  
  
 <span data-ttu-id="89d0f-118">Après avoir transféré les lignes relevé vers la feuille, vous pouvez valider les lignes relevé vers la feuille financière correspondante.</span><span class="sxs-lookup"><span data-stu-id="89d0f-118">After transferring the statement lines to the journal, you can post the statement lines in the corresponding financial journal.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="89d0f-119">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="89d0f-119">See Also</span></span>  
 <span data-ttu-id="89d0f-120">[Relevés bancaires CODA](coda-bank-statements.md) </span><span class="sxs-lookup"><span data-stu-id="89d0f-120">[CODA Bank Statements](coda-bank-statements.md) </span></span>  
 <span data-ttu-id="89d0f-121">[Comment importer les relevés CODA](how-to-import-coda-statements.md) </span><span class="sxs-lookup"><span data-stu-id="89d0f-121">[How to: Import CODA Statements](how-to-import-coda-statements.md) </span></span>  
 <span data-ttu-id="89d0f-122">[Comment lettrer les relevés CODA](how-to-apply-coda-statements.md) </span><span class="sxs-lookup"><span data-stu-id="89d0f-122">[How to: Apply CODA Statements](how-to-apply-coda-statements.md) </span></span>  
 <span data-ttu-id="89d0f-123">[Comment créer des feuilles financières](how-to-create-financial-journals.md) </span><span class="sxs-lookup"><span data-stu-id="89d0f-123">[How to: Create Financial Journals](how-to-create-financial-journals.md) </span></span>  
 <span data-ttu-id="89d0f-124">[Comment transférer et valider manuellement les relevés CODA](how-to-manually-transfer-and-post-coda-statements.md).</span><span class="sxs-lookup"><span data-stu-id="89d0f-124">[How to: Manually Transfer and Post CODA Statements](how-to-manually-transfer-and-post-coda-statements.md)</span></span>
