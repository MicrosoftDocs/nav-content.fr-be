---
title: "Comment utiliser les clés de ventilation dans les feuilles de comptabilité"
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: ca21d9d129dbc98d75371d1b2b7a0ffad4aa2848
ms.contentlocale: fr-be
ms.lasthandoff: 07/19/2017

---

#  <a name="how-to-use-allocation-keys-in-general-journals"></a><span data-ttu-id="7e7f1-102">Comment utiliser les clés de ventilation dans les feuilles de comptabilité</span><span class="sxs-lookup"><span data-stu-id="7e7f1-102">How to: Use Allocation Keys in General Journals</span></span>
<span data-ttu-id="7e7f1-103">Vous pouvez ventiler une écriture dans une feuille comptabilité dans différents comptes lorsque vous validez la feuille.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-103">You can allocate an entry in a general journal to several different accounts when you post the journal.</span></span> <span data-ttu-id="7e7f1-104">La ventilation peut être effectuée par quantité, pourcentage ou montant.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-104">The allocation can be made by quantity, percentage, or amount.</span></span>

## <a name="to-set-up-allocation-keys"></a><span data-ttu-id="7e7f1-105">Pour définir des clés de ventilation</span><span class="sxs-lookup"><span data-stu-id="7e7f1-105">To set up allocation keys</span></span> 
1. <span data-ttu-id="7e7f1-106">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Feuille abonnement**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-106">In the top right corner, choose the **Search for Page or Report** icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="7e7f1-107">Sélectionnez le champ **Nom de la feuille** pour ouvrir la fenêtre **Noms feuilles comptabilité**.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-107">Choose the **Batch Name** field to open the **General Journal Batches** window.</span></span>
3. <span data-ttu-id="7e7f1-108">Vous pouvez soit modifier les ventilations sur un lot existant dans la liste ou créer un lot avec des ventilations.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-108">You can either modify allocations on an existing batch in the list or create a new batch with allocations.</span></span>
  * <span data-ttu-id="7e7f1-109">Pour créer un lot, sélectionnez l'action **Nouveau**, et passez à l'étape suivante.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-109">To create a new batch, choose the **New** action, and go to the next step.</span></span>
  * <span data-ttu-id="7e7f1-110">Pour modifier les ventilations à partir d'une feuille existante, sélectionnez la feuille et passez à l'étape 7.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-110">To change the allocations of an existing journal, select the journal and go to step 7.</span></span>    
4. <span data-ttu-id="7e7f1-111">Dans le champ **Nom**, saisissez le nom du lot, par exemple NETTOYAGE.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-111">In the **Name** field, enter a name for the batch, such as CLEANING.</span></span> <span data-ttu-id="7e7f1-112">Dans le champ **Description**, saisissez une description, par exemple Feuille frais de nettoyage.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-112">In the **Description** field, enter a description, such as Cleaning Expenses Journal.</span></span>
5. <span data-ttu-id="7e7f1-113">Fermez la fenêtre lorsque vous avez terminé.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-113">When you are done, close the window.</span></span> <span data-ttu-id="7e7f1-114">Une nouvelle feuille récurrente vide s'ouvre.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-114">A new, empty recurring journal opens.</span></span> 
6. <span data-ttu-id="7e7f1-115">Renseignez les champs de la ligne.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-115">Fill in the fields in the line.</span></span>
7. <span data-ttu-id="7e7f1-116">Sélectionnez l'action **Ventilations**.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-116">Choose the **Allocations** action.</span></span> 
8. <span data-ttu-id="7e7f1-117">Ajoutez une ligne pour chaque ventilation.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-117">Add a line for each allocation.</span></span> <span data-ttu-id="7e7f1-118">Vous devez renseigner le champ **% ventilation**, **Quantité imputée** ou **Montant**.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-118">You must fill in either the **Allocation %**, **Allocation Quantity**, or **Amount** field.</span></span> <span data-ttu-id="7e7f1-119">Vous devez également renseigner le champ **N° compte**</span><span class="sxs-lookup"><span data-stu-id="7e7f1-119">You must also fill in the **Account No.**</span></span> <span data-ttu-id="7e7f1-120">et, si vous ventilez la transaction sur des axes principaux, les champs de ces axes principaux.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-120">field and, if you are allocating the transaction among global dimensions, the global dimension fields.</span></span>
9. <span data-ttu-id="7e7f1-121">Si vous saisissez un pourcentage dans une ligne, le montant du champ **Montant** est calculé automatiquement.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-121">If you enter a percentage on a line, the amount in the **Amount** field is calculated automatically.</span></span> <span data-ttu-id="7e7f1-122">Ces montants sont dotés du signe opposé à celui du montant total figurant dans le champ **Montant** de la feuille récurrente.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-122">These amounts have the opposite sign from the total amount in the **Amount** field in the recurring journal.</span></span>
10. <span data-ttu-id="7e7f1-123">Après avoir saisi les lignes de ventilation, cliquez sur **OK** pour revenir à la fenêtre **Feuille abonnement**.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-123">After entering the allocations lines, choose **OK** to return to the **Recurring General Journal** window.</span></span> <span data-ttu-id="7e7f1-124">Le champ **Montant imputé DS** est renseigné et correspond au champ **Montant**.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-124">The **Allocated Amt. (USD)** field is filled in and matches the **Amount** field.</span></span>
11. <span data-ttu-id="7e7f1-125">Validez la feuille.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-125">Post the journal.</span></span>

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a><span data-ttu-id="7e7f1-126">Pour modifier une clé de ventilation déjà configurée</span><span class="sxs-lookup"><span data-stu-id="7e7f1-126">To change an allocation key that has already been set up</span></span>
1. <span data-ttu-id="7e7f1-127">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Feuille abonnement**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-127">In the top right corner, choose the **Search for Page or Report** icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="7e7f1-128">Dans la fenêtre **Feuille récurrente**, sélectionnez la feuille contenant la ventilation.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-128">In the **Recurring General Journal** window, select the journal with the allocation.</span></span>
3. <span data-ttu-id="7e7f1-129">Sélectionnez la ligne de la ventilation, puis sélectionnez l'action **Ventilations**.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-129">Choose the line with the allocation, and then choose **Allocations** action.</span></span>
4. <span data-ttu-id="7e7f1-130">Modifiez les champs appropriés, puis fermez la fenêtre.</span><span class="sxs-lookup"><span data-stu-id="7e7f1-130">Change the relevant fields, and close the window.</span></span>

## <a name="see-also"></a><span data-ttu-id="7e7f1-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7e7f1-131">See Also</span></span>
[<span data-ttu-id="7e7f1-132">Utilisation des feuilles comptabilité</span><span class="sxs-lookup"><span data-stu-id="7e7f1-132">Work With General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="7e7f1-133">Valider des documents et des feuilles</span><span class="sxs-lookup"><span data-stu-id="7e7f1-133">Post Documents and Journals</span></span>](ui-post-documents-journals.md)




