---
title: "Comment transférer les écritures comptables vers les écritures de coûts"
description: "Vous pouvez transférer les écritures comptables aux écritures de coûts."
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
ms.openlocfilehash: b7a78fb1023e8b664fd866eb1a8b5e42ff0de265
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-transfer-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="7edde-103">Comment transférer les écritures comptables vers les écritures de coûts</span><span class="sxs-lookup"><span data-stu-id="7edde-103">How to: Transfer General Ledger Entries to Cost Entries</span></span>
<span data-ttu-id="7edde-104">Vous pouvez transférer les écritures comptables aux écritures de coûts.</span><span class="sxs-lookup"><span data-stu-id="7edde-104">You can transfer general ledger entries to cost entries.</span></span>  

<span data-ttu-id="7edde-105">Avant d'exécuter le transfert des écritures comptables vers des écritures de coûts, vous devez vous y préparer pour éviter toute validation manuelle de correction.</span><span class="sxs-lookup"><span data-stu-id="7edde-105">Before you run the process for transferring general ledger entries to cost entries, you must prepare the transfer to avoid manual correction posting.</span></span>  

## <a name="to-prepare-the-transfer"></a><span data-ttu-id="7edde-106">Pour préparer le transfert</span><span class="sxs-lookup"><span data-stu-id="7edde-106">To prepare the transfer</span></span>  

1.  <span data-ttu-id="7edde-107">Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Paramètres comptabilité analytique**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="7edde-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Cost Accounting Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="7edde-108">Dans la fenêtre **Paramètres comptabilité analytique**, vérifiez que le champ **Date début pour transfert comptabilité** est défini sur la valeur appropriée.</span><span class="sxs-lookup"><span data-stu-id="7edde-108">In the **Cost Accounting Setup** window, verify that the **Starting Date for G/L Transfer** field is set to the correct value.</span></span>  
3.  <span data-ttu-id="7edde-109">Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Plan comptable des types de coûts**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="7edde-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Cost Types**, and then choose the related link.</span></span>  
4.  <span data-ttu-id="7edde-110">Dans la fenêtre **Fiche type de coût**, vérifiez que le champ **Plage compte général** est lié correctement de sorte que chaque type de coût récupère les écritures de la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="7edde-110">In the **Cost Type Card** window, verify that the **G/L Account Range** field is linked correctly for each cost type to take entries from the general ledger.</span></span>  
5.  <span data-ttu-id="7edde-111">Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Plan comptable**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="7edde-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
6.  <span data-ttu-id="7edde-112">Pour chaque compte général approprié, dans la fenêtre **Fiche compte général**, dans le raccourci Comptabilité analytique, vérifiez que le champ **N° type coût**</span><span class="sxs-lookup"><span data-stu-id="7edde-112">For each relevant general ledger account, in the **G/L Account Card** window, verify that the **Cost Type No.**</span></span> <span data-ttu-id="7edde-113">est lié correctement à un type de coût.</span><span class="sxs-lookup"><span data-stu-id="7edde-113">field is linked correctly to a cost type.</span></span> <span data-ttu-id="7edde-114">Pour plus d'informations, voir [Définition de la relation entre les types de coûts et les comptes généraux](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="7edde-114">For more information, see [Defining the Relationship Between Cost Types and General Ledger Accounts](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md).</span></span>  
7.  <span data-ttu-id="7edde-115">Vérifiez que toutes les écritures comptables appropriées comprennent des sections analytiques correspondant à un centre de coûts et à un coût associé.</span><span class="sxs-lookup"><span data-stu-id="7edde-115">Verify that all relevant general ledger entries have dimension values that correspond to a cost center and a cost object.</span></span>  

## <a name="to-transfer-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="7edde-116">Pour transférer les écritures comptables vers les écritures de coûts</span><span class="sxs-lookup"><span data-stu-id="7edde-116">To transfer general ledger entries to cost entries</span></span>  
1.  <span data-ttu-id="7edde-117">Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Transférer les écritures comptables vers CA**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="7edde-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Transfer GL Entries to CA**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="7edde-118">Cliquez sur le bouton **Oui** pour démarrer le transfert.</span><span class="sxs-lookup"><span data-stu-id="7edde-118">Choose the **Yes** button to start the transfer.</span></span> <span data-ttu-id="7edde-119">Le processus transfère toutes les écritures comptables qui n'ont pas déjà été transférées.</span><span class="sxs-lookup"><span data-stu-id="7edde-119">The process transfers all general ledger entries that have not already been transferred.</span></span>  

    <span data-ttu-id="7edde-120">Lors du transfert, le processus crée des connexions dans les écritures des tables **Écriture de coûts** et **Registre de coûts**.</span><span class="sxs-lookup"><span data-stu-id="7edde-120">During the transfer, the process creates connections in the entries in the **Cost Entry** table and the **Cost Register** table.</span></span> <span data-ttu-id="7edde-121">Cela permet d'identifier l'origine des écritures de coûts.</span><span class="sxs-lookup"><span data-stu-id="7edde-121">This makes it possible to trace the source of cost entries.</span></span>  

## <a name="see-also"></a><span data-ttu-id="7edde-122">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7edde-122">See Also</span></span>  
 <span data-ttu-id="7edde-123">[Critères de transfert des écritures comptables vers les écritures de coûts](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="7edde-123">[Criteria for Transferring General Ledger Entries to Cost Entries](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="7edde-124">[Transfert automatique et écritures combinées](finance-automatic-transfer-combined-entries.md) </span><span class="sxs-lookup"><span data-stu-id="7edde-124">[Automatic Transfer and Combined Entries](finance-automatic-transfer-combined-entries.md) </span></span>  
 <span data-ttu-id="7edde-125">[Résultats du transfert](finance-results-of-the-transfer.md) </span><span class="sxs-lookup"><span data-stu-id="7edde-125">[Results of the Transfer](finance-results-of-the-transfer.md) </span></span>  
 <span data-ttu-id="7edde-126">[Transfert et validation des écritures de coûts](finance-transfer-and-post-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="7edde-126">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span></span>  
 [<span data-ttu-id="7edde-127">Définition de la relation entre les types de coûts et les comptes généraux</span><span class="sxs-lookup"><span data-stu-id="7edde-127">Defining the Relationship Between Cost Types and General Ledger Accounts</span></span>](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md)   
