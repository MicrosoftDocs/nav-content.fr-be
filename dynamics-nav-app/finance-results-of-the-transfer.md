---
title: "Résultats du transfert"
description: "Cette rubrique décrit ce qui se produit après le transfert des écritures comptables vers les écritures de coûts."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: general ledger, transfer, cost entries
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 05da79520b5568a8b8e63f10efce9c8b3c5395b8
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="results-of-transferring-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="f5594-103">Résultats du transfert des écritures comptables vers les écritures de coûts</span><span class="sxs-lookup"><span data-stu-id="f5594-103">Results of Transferring General Ledger Entries to Cost Entries</span></span>
<span data-ttu-id="f5594-104">Lors du transfert des écritures comptables vers les écritures de coûts, [!INCLUDE[d365fin](includes/d365fin_md.md)] crée des connexions dans les écritures dans les tables **Écriture comptable**, **Écriture de coûts** et **Registre de coûts** pour assurer le suivi des connexions entre les écritures de coûts et les écritures comptables.</span><span class="sxs-lookup"><span data-stu-id="f5594-104">During the transfer of general ledger entries to cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] creates connections in the entries in the **G/L Entry** table, the **Cost Entry** table, and the **Cost Register** table to make it possible to trace the connections between cost entries and general ledger entries.</span></span>  

## <a name="general-ledger-entries"></a><span data-ttu-id="f5594-105">Écritures comptables</span><span class="sxs-lookup"><span data-stu-id="f5594-105">General Ledger Entries</span></span>  
<span data-ttu-id="f5594-106">Pour chaque écriture comptable transférée vers la comptabilité analytique, [!INCLUDE[d365fin](includes/d365fin_md.md)] renseigne le champ **N° écriture**</span><span class="sxs-lookup"><span data-stu-id="f5594-106">For each general ledger entry that is transferred to cost accounting, [!INCLUDE[d365fin](includes/d365fin_md.md)] fills the cost **Entry No.** field.</span></span>  

## <a name="cost-entries"></a><span data-ttu-id="f5594-107">Écritures de coûts</span><span class="sxs-lookup"><span data-stu-id="f5594-107">Cost Entries</span></span>  
<span data-ttu-id="f5594-108">Pour chaque écriture de coûts, [!INCLUDE[d365fin](includes/d365fin_md.md)] garde le numéro de l'écriture comptable correspondante dans le champ **N° séquence compta.** de la table **Écriture de coûts**.</span><span class="sxs-lookup"><span data-stu-id="f5594-108">For each cost entry, [!INCLUDE[d365fin](includes/d365fin_md.md)] saves the entry number of the corresponding general ledger entry in the **G/L Entry No.** field in the **Cost Entry** table.</span></span>  

<span data-ttu-id="f5594-109">Pour les écritures de coûts combinées, [!INCLUDE[d365fin](includes/d365fin_md.md)] garde le numéro de la dernière écriture comptable, à savoir l'écriture avec le numéro le plus élevé.</span><span class="sxs-lookup"><span data-stu-id="f5594-109">For combined cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] saves the entry number of the last general ledger entry, which is the entry with the highest entry number.</span></span>  

<span data-ttu-id="f5594-110">Le champ **Compte général** de la table **Écriture de coûts** contient le numéro du compte général, d'où provient l'écriture de coûts.</span><span class="sxs-lookup"><span data-stu-id="f5594-110">The **G/L Account** field in the **Cost Entry** table contains the number of the general ledger account that the cost entry came from.</span></span>  

<span data-ttu-id="f5594-111">Pour les écritures de coûts uniques, [!INCLUDE[d365fin](includes/d365fin_md.md)] transfère le texte de validation depuis l'écriture comptable vers le champ de texte **Description**.</span><span class="sxs-lookup"><span data-stu-id="f5594-111">For single cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] transfers the posting text from the general ledger entry to the **Description** text field.</span></span> <span data-ttu-id="f5594-112">Pour les écritures combinées, le champ de texte indique que ces écritures sont transférées en tant qu'écritures combinées.</span><span class="sxs-lookup"><span data-stu-id="f5594-112">For combined entries, the text field shows these entries are transferred as combined entries.</span></span> <span data-ttu-id="f5594-113">Par exemple, pour une écriture combinée pour octobre 2013, le texte peut être **Écritures combinées, octobre 2013**.</span><span class="sxs-lookup"><span data-stu-id="f5594-113">For example, for a combined entry for the month of October in 2013, the text can be **Combined Entries, October 2013**.</span></span>  

## <a name="cost-register"></a><span data-ttu-id="f5594-114">Registre de coûts</span><span class="sxs-lookup"><span data-stu-id="f5594-114">Cost Register</span></span>  
<span data-ttu-id="f5594-115">Dans la table **Registre de coûts**, [!INCLUDE[d365fin](includes/d365fin_md.md)] crée une écriture à l'aide du transfert source depuis la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="f5594-115">In the **Cost Register** table, [!INCLUDE[d365fin](includes/d365fin_md.md)] creates an entry with the source transfer from general ledger.</span></span> <span data-ttu-id="f5594-116">L'écriture enregistre le premier et le dernier numéros des écritures comptables transférées, outre le premier et le dernier numéros des écritures de coûts créées.</span><span class="sxs-lookup"><span data-stu-id="f5594-116">The entry records the first and last entry numbers of the general ledger entries that are transferred, in addition to the first and last entry numbers of the cost entries that are created.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f5594-117">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f5594-117">See Also</span></span>  
<span data-ttu-id="f5594-118">[Comment transférer les écritures comptables vers les écritures de coûts](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="f5594-118">[How to: Transfer General Ledger Entries to Cost Entries](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span></span>  
<span data-ttu-id="f5594-119">[Critères de transfert des écritures comptables vers les écritures de coûts](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="f5594-119">[Criteria for Transferring General Ledger Entries to Cost Entries](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span></span>  
<span data-ttu-id="f5594-120">[Transfert automatique et écritures combinées](finance-automatic-transfer-combined-entries.md) </span><span class="sxs-lookup"><span data-stu-id="f5594-120">[Automatic Transfer and Combined Entries](finance-automatic-transfer-combined-entries.md) </span></span>  
[<span data-ttu-id="f5594-121">Transfert et validation des écritures de coûts</span><span class="sxs-lookup"><span data-stu-id="f5594-121">Transferring and Posting Cost Entries</span></span>](finance-transfer-and-post-cost-entries.md)  
