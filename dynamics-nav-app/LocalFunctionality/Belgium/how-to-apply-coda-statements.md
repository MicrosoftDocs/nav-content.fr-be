---
title: "Comment lettrer les relevés CODA"
description: "Après l'importation d'un relevé CODA, vous pouvez accéder aux lignes relevé à partir de la fenêtre **Fiche compte bancaire**. Le statut lettrage de chaque ligne sera vide, car les montants du relevé n'ont pas été lettrés à des écritures comptables en attente."
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
ms.openlocfilehash: b0248052d5f2e68edfd66415a64fb5dce7b415a0
ms.contentlocale: fr-be
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-apply-coda-statements"></a><span data-ttu-id="2b8ae-104">Comment lettrer les relevés CODA</span><span class="sxs-lookup"><span data-stu-id="2b8ae-104">How to: Apply CODA Statements</span></span>
<span data-ttu-id="2b8ae-105">Après l'importation d'un relevé CODA, vous pouvez accéder aux lignes relevé à partir de la fenêtre **Fiche compte bancaire**.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-105">After a CODA statement has been imported, the statement lines can be accessed from the **Bank Account Card** window.</span></span> <span data-ttu-id="2b8ae-106">Le statut lettrage de chaque ligne sera vide, car les montants du relevé n'ont pas été lettrés à des écritures comptables en attente.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-106">The application status on each line will be blank because the statement amounts have not been applied to outstanding ledger entries.</span></span>  

<span data-ttu-id="2b8ae-107">Les montants du relevé peuvent être lettrés à des écritures comptables en attente des manières suivantes :</span><span class="sxs-lookup"><span data-stu-id="2b8ae-107">Statement amounts can be applied to outstanding ledger entries by:</span></span>  

-   <span data-ttu-id="2b8ae-108">Lettrage manuel des lignes relevé CODA.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-108">Manually applying CODA statement lines.</span></span>  
-   <span data-ttu-id="2b8ae-109">Lettrage automatique des montants du relevé CODA aux écritures comptables et comptes adéquats.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-109">Automatically applying CODA statement amounts to the appropriate ledger entries and accounts.</span></span> <span data-ttu-id="2b8ae-110">Le traitement automatique des lignes relevé CODA est recommandé.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-110">Automatic processing of CODA statement lines is recommended.</span></span>  

## <a name="to-manually-apply-the-coda-statement-lines"></a><span data-ttu-id="2b8ae-111">Pour lettrer manuellement les lignes relevé CODA</span><span class="sxs-lookup"><span data-stu-id="2b8ae-111">To manually apply the CODA statement lines</span></span>  

1.  <span data-ttu-id="2b8ae-112">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Comptes bancaires**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-112">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="2b8ae-113">Sélectionnez le compte bancaire, puis choisissez l'action **Relevés CODA**.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-113">Select the bank account, and then choose the **CODA Statements** action.</span></span>  
3.  <span data-ttu-id="2b8ae-114">Sélectionnez le relevé CODA, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-114">Select the CODA statement, and then choose the **Edit** action.</span></span>  
4.  <span data-ttu-id="2b8ae-115">Dans le raccourci **Lignes relevé CODA**, pour chaque ligne relevé, remplissez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-115">In the **CODA Statement Lines** FastTab, for each statement line, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="2b8ae-116">Champ</span><span class="sxs-lookup"><span data-stu-id="2b8ae-116">Field</span></span>|<span data-ttu-id="2b8ae-117">Description</span><span class="sxs-lookup"><span data-stu-id="2b8ae-117">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="2b8ae-118">**N° compte**</span><span class="sxs-lookup"><span data-stu-id="2b8ae-118">**Account No.**</span></span>|<span data-ttu-id="2b8ae-119">Entrez le numéro du compte général, la banque, le client, le fournisseur ou l'immobilisation auquel la ligne relevé compte bancaire est liée.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-119">Enter the number of the general ledger account, bank, customer, vendor, or fixed asset, which the bank account statement line is linked to.</span></span>|  
    |<span data-ttu-id="2b8ae-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="2b8ae-120">**Description**</span></span>|[!INCLUDE[navnow](../../includes/navnow_md.md)]<span data-ttu-id="2b8ae-121"> récupère automatiquement la description à partir du fichier CODA importé, mais vous pouvez modifier le contenu de ce champ.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-121"> automatically retrieves the description from the imported CODA file, but you can modify the contents of this field.</span></span>|  

5.  <span data-ttu-id="2b8ae-122">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-122">Choose the **OK** button.</span></span>  

## <a name="to-automatically-apply-the-coda-statement-lines"></a><span data-ttu-id="2b8ae-123">Pour lettrer automatiquement les lignes relevé CODA</span><span class="sxs-lookup"><span data-stu-id="2b8ae-123">To automatically apply the CODA statement lines</span></span>  

1.  <span data-ttu-id="2b8ae-124">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Comptes bancaires**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-124">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="2b8ae-125">Sélectionnez le compte bancaire, puis choisissez l'action **Relevés CODA**.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-125">Select the bank account, and then choose the **CODA Statements** action.</span></span>  
3.  <span data-ttu-id="2b8ae-126">Sélectionnez le relevé CODA, puis choisissez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-126">Select the CODA statement, and then choose the **Edit** action.</span></span>  
4.  <span data-ttu-id="2b8ae-127">Choisissez l'action **Valider lignes relevé CODA**.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-127">Choose the **Process CODA Statement Lines** action.</span></span>  
5.  <span data-ttu-id="2b8ae-128">Remplissez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-128">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="2b8ae-129">Champ</span><span class="sxs-lookup"><span data-stu-id="2b8ae-129">Field</span></span>|<span data-ttu-id="2b8ae-130">Description</span><span class="sxs-lookup"><span data-stu-id="2b8ae-130">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="2b8ae-131">**Validation par défaut**</span><span class="sxs-lookup"><span data-stu-id="2b8ae-131">**Default Posting**</span></span>|<span data-ttu-id="2b8ae-132">Définissez si vous souhaitez que le traitement par lots valide les montants du relevé qui ne peuvent pas être liés à des écritures comptables existantes.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-132">Select if you want the batch job to post statement amounts that cannot be linked to existing ledger entries.</span></span> <span data-ttu-id="2b8ae-133">Pour plus d'informations, voir Encodage CODA.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-133">For more information, see Transaction Coding.</span></span>|  
    |<span data-ttu-id="2b8ae-134">**Imprimer liste**</span><span class="sxs-lookup"><span data-stu-id="2b8ae-134">**Print List**</span></span>|<span data-ttu-id="2b8ae-135">Sélectionnez l'option d'impression d'une liste des montants du relevé qui ne peuvent pas être liés automatiquement.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-135">Select to print a list of statement amounts that cannot be linked automatically.</span></span>|  

6.  <span data-ttu-id="2b8ae-136">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-136">Choose the **OK** button.</span></span>  

    <span data-ttu-id="2b8ae-137">Lorsque vous commencez le traitements par lots, les montants du relevé seront lettrés à des écritures comptables existantes selon les codes transaction.</span><span class="sxs-lookup"><span data-stu-id="2b8ae-137">When you start the batch job, statement amounts will be applied to existing ledger entries based on the transaction codes.</span></span> <span data-ttu-id="2b8ae-138">Pour plus d'informations, voir [Comment configurer des comptes bancaires pour CODA](how-to-set-up-bank-accounts-for-coda.md).</span><span class="sxs-lookup"><span data-stu-id="2b8ae-138">For more information, see [How to: Set Up Bank Accounts for CODA](how-to-set-up-bank-accounts-for-coda.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="2b8ae-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2b8ae-139">See Also</span></span>  
 <span data-ttu-id="2b8ae-140">[Relevés bancaires CODA](coda-bank-statements.md) </span><span class="sxs-lookup"><span data-stu-id="2b8ae-140">[CODA Bank Statements](coda-bank-statements.md) </span></span>  
 <span data-ttu-id="2b8ae-141">[Comment configurer les comptes bancaires pour CODA](how-to-set-up-bank-accounts-for-coda.md) </span><span class="sxs-lookup"><span data-stu-id="2b8ae-141">[How to: Set Up Bank Accounts for CODA](how-to-set-up-bank-accounts-for-coda.md) </span></span>  
 <span data-ttu-id="2b8ae-142">[Comment configurer les codes transaction IBLC/BLWI](how-to-set-up-iblc-blwi-transaction-codes.md) </span><span class="sxs-lookup"><span data-stu-id="2b8ae-142">[How to: Set Up IBLC-BLWI Transaction Codes](how-to-set-up-iblc-blwi-transaction-codes.md) </span></span>  
 <span data-ttu-id="2b8ae-143">[Comment importer les relevés CODA](how-to-import-coda-statements.md) </span><span class="sxs-lookup"><span data-stu-id="2b8ae-143">[How to: Import CODA Statements](how-to-import-coda-statements.md) </span></span>  
 <span data-ttu-id="2b8ae-144">[Comment créer des feuilles financières](how-to-create-financial-journals.md) </span><span class="sxs-lookup"><span data-stu-id="2b8ae-144">[How to: Create Financial Journals](how-to-create-financial-journals.md) </span></span>  
 <span data-ttu-id="2b8ae-145">[Comment transférer et valider automatiquement les relevés CODA](how-to-automatically-transfer-and-post-coda-statements.md) . </span><span class="sxs-lookup"><span data-stu-id="2b8ae-145">[How to: Automatically Transfer and Post CODA Statements](how-to-automatically-transfer-and-post-coda-statements.md) </span></span>  
 <span data-ttu-id="2b8ae-146">[Comment transférer et valider manuellement les relevés CODA](how-to-manually-transfer-and-post-coda-statements.md).</span><span class="sxs-lookup"><span data-stu-id="2b8ae-146">[How to: Manually Transfer and Post CODA Statements](how-to-manually-transfer-and-post-coda-statements.md)</span></span>

