---
title: "Comment classer les paiements SEPA non libellés en Euro"
description: "Dans [!INCLUDE[navnow](../../includes/navnow_md.md)], vous pouvez classer les paiements SEPA non libellés en Euro avec la banque. Cette fonction est utile lorsque vous effectuez des paiements vers d'autres pays qui n'utilisent pas le format SEPA et pour des devises autres que l'euro."
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
ms.openlocfilehash: 3c41faf5f82176074d5c0c04e3d5a7b244d20f24
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-file-non-euro-sepa-payments"></a><span data-ttu-id="40b78-104">Comment classer les paiements SEPA non libellés en Euro</span><span class="sxs-lookup"><span data-stu-id="40b78-104">How to: File Non-Euro SEPA Payments</span></span>
<span data-ttu-id="40b78-105">Dans [!INCLUDE[navnow](../../includes/navnow_md.md)], vous pouvez classer les paiements SEPA non libellés en Euro avec la banque.</span><span class="sxs-lookup"><span data-stu-id="40b78-105">In [!INCLUDE[navnow](../../includes/navnow_md.md)], you can file non-euro SEPA payments with the bank.</span></span> <span data-ttu-id="40b78-106">Cette fonction est utile lorsque vous effectuez des paiements vers d'autres pays qui n'utilisent pas le format SEPA et pour des devises autres que l'euro.</span><span class="sxs-lookup"><span data-stu-id="40b78-106">This is useful when you make payments to other countries that do not use SEPA and for currencies other than the euro.</span></span>  
  
 <span data-ttu-id="40b78-107">Avant de classer un paiement non libellé en Euro, vous devez remplir les tâches administratives suivantes :</span><span class="sxs-lookup"><span data-stu-id="40b78-107">Before you can file a non-euro SEPA payment you must complete the following administration tasks:</span></span>  
  
-   <span data-ttu-id="40b78-108">Configurer un nouveau protocole d'exportation pour un paiement SEPA non libellé en Euro.</span><span class="sxs-lookup"><span data-stu-id="40b78-108">Set up a new export protocol for a non-euro SEPA.</span></span> <span data-ttu-id="40b78-109">Pour plus d'informations, voir Protocole d'exportation.</span><span class="sxs-lookup"><span data-stu-id="40b78-109">For more information, see Export Protocol.</span></span>  
  
-   <span data-ttu-id="40b78-110">Dans la table **Pays/Région**, effacez le champ **SEPA autorisé** pour chaque pays appartenant à la zone EEA.</span><span class="sxs-lookup"><span data-stu-id="40b78-110">In the **Country/Region** table, clear the **SEPA Allowed** field for each country that belongs to the EEA zone.</span></span>  
  
-   <span data-ttu-id="40b78-111">Vérifiez que le champ **Devise Euro** de la table **Paramètres comptabilité** n'est pas en Euro.</span><span class="sxs-lookup"><span data-stu-id="40b78-111">Verify that the **Currency Euro** field in the **General Ledger Setup** table is not in euro currency.</span></span>  
  
-   <span data-ttu-id="40b78-112">Vérifiez que le champ **Compte bancaire préféré** du fournisseur dans la table **Fournisseur** contient les codes IBAN et SWIFT.</span><span class="sxs-lookup"><span data-stu-id="40b78-112">Verify that the vendor’s **Preferred Bank Account** field in the **Vendor** table contains the IBAN and SWIFT code.</span></span>  
  
### <a name="to-file-a-non-euro-sepa-payment"></a><span data-ttu-id="40b78-113">Pour classer un paiement SEPA non libellé en Euro</span><span class="sxs-lookup"><span data-stu-id="40b78-113">To file a non-euro SEPA payment</span></span>  
  
1.  <span data-ttu-id="40b78-114">Sélectionnez l'icône ![Rechercher une page ou un état](media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Classer les paiements SEPA non libellés en Euro**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="40b78-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **File Non Euro SEPA Payments**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="40b78-115">Remplissez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="40b78-115">Fill in the fields as described in the following table.</span></span>  
  
    |<span data-ttu-id="40b78-116">Champ</span><span class="sxs-lookup"><span data-stu-id="40b78-116">Field</span></span>|<span data-ttu-id="40b78-117">Description</span><span class="sxs-lookup"><span data-stu-id="40b78-117">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="40b78-118">**Nom modèle feuille**</span><span class="sxs-lookup"><span data-stu-id="40b78-118">**Journal Template Name**</span></span>|<span data-ttu-id="40b78-119">Spécifiez le modèle feuille comptabilité pour l'état de paiement SEPA non libellé en Euro.</span><span class="sxs-lookup"><span data-stu-id="40b78-119">Specify the general journal template for the non-euro SEPA payment report.</span></span>|  
    |<span data-ttu-id="40b78-120">**Feuille**</span><span class="sxs-lookup"><span data-stu-id="40b78-120">**Journal Batch**</span></span>|<span data-ttu-id="40b78-121">Spécifiez le nom feuille comptabilité pour l'état de paiement SEPA non libellé en Euro.</span><span class="sxs-lookup"><span data-stu-id="40b78-121">Specify the general journal batch for the non-euro SEPA payment report.</span></span>|  
    |<span data-ttu-id="40b78-122">**Valider lignes FS**</span><span class="sxs-lookup"><span data-stu-id="40b78-122">**Post General Journal Lines**</span></span>|<span data-ttu-id="40b78-123">Spécifiez si vous souhaitez transférer les lignes de paiement dans la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="40b78-123">Specify if you want to transfer the payment lines to the general ledger.</span></span>|  
    |<span data-ttu-id="40b78-124">**Inclure axes**</span><span class="sxs-lookup"><span data-stu-id="40b78-124">**Include Dimensions**</span></span>|<span data-ttu-id="40b78-125">Entrez les axes analytiques que vous souhaitez inclure dans l'état de paiement SEPA non libellé en Euro.</span><span class="sxs-lookup"><span data-stu-id="40b78-125">Enter the dimensions that you want to include in the non-euro SEPA payment report.</span></span> <span data-ttu-id="40b78-126">Cette option est uniquement disponible si le champ **Résumer lignes FS** de la fenêtre **Configuration de la banque électronique** est sélectionné.</span><span class="sxs-lookup"><span data-stu-id="40b78-126">The option is only available if the **Summarize Gen. Jnl. Lines** field in the **Electronic Banking Setup** window is selected.</span></span>|  
    |<span data-ttu-id="40b78-127">**Date d'exécution**</span><span class="sxs-lookup"><span data-stu-id="40b78-127">**Execution Date**</span></span>|<span data-ttu-id="40b78-128">Entrez une date d'exécution si vous souhaitez que la date d'exécution soit différente de la date de validation sur les lignes paiement.</span><span class="sxs-lookup"><span data-stu-id="40b78-128">Enter an execution date if you want an execution date that differs from the posting date on the payment lines.</span></span>|  
    |<span data-ttu-id="40b78-129">**Nom du fichier**</span><span class="sxs-lookup"><span data-stu-id="40b78-129">**File Name**</span></span>|<span data-ttu-id="40b78-130">Entrez le nom du fichier, y compris le disque et le dossier, à partir duquel vous souhaitez imprimer l'état.</span><span class="sxs-lookup"><span data-stu-id="40b78-130">Enter the name of the file, including the drive and folder, to which you want to print the report.</span></span>|  
  
3.  <span data-ttu-id="40b78-131">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="40b78-131">Choose the **OK** button.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="40b78-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="40b78-132">See Also</span></span>  
 <span data-ttu-id="40b78-133">Classer les paiements SEPA non libellés en Euro</span><span class="sxs-lookup"><span data-stu-id="40b78-133">File Non Euro SEPA Payments</span></span>   
 <span data-ttu-id="40b78-134">Classer les paiements SEPA</span><span class="sxs-lookup"><span data-stu-id="40b78-134">File SEPA Payments</span></span>   
 <span data-ttu-id="40b78-135">[Comment classer les paiements SEPA](how-to-file-sepa-payments.md) </span><span class="sxs-lookup"><span data-stu-id="40b78-135">[How to: File SEPA Payments](how-to-file-sepa-payments.md) </span></span>  
 <span data-ttu-id="40b78-136">[Comment activer les paiements SEPA](how-to-activate-sepa-payments.md) </span><span class="sxs-lookup"><span data-stu-id="40b78-136">[How to: Activate SEPA Payments](how-to-activate-sepa-payments.md) </span></span>  
 [<span data-ttu-id="40b78-137">Paiements SEPA</span><span class="sxs-lookup"><span data-stu-id="40b78-137">SEPA Payments</span></span>](sepa-payments.md)
