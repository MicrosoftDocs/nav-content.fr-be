---
title: "Procédure : octroyer une priorité à des fournisseurs"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: df14bab26aa0d52e7ad5215862fcef608ba5a7d7
ms.contentlocale: fr-be
ms.lasthandoff: 07/19/2017

---

# <a name="how-to-prioritize-vendors"></a><span data-ttu-id="c8f1d-102">Procédure : octroyer une priorité à des fournisseurs</span><span class="sxs-lookup"><span data-stu-id="c8f1d-102">How to: Prioritize Vendors</span></span>
<span data-ttu-id="c8f1d-103">Dynamics NAV peut proposer différents paiements aux fournisseurs, par exemple les paiements arrivant à échéance ou les paiements donnant lieu à un escompte.</span><span class="sxs-lookup"><span data-stu-id="c8f1d-103">Dynamics NAV can suggest various payments to vendors, for example, payments that will be due soon or payments where a discount is available.</span></span> <span data-ttu-id="c8f1d-104">Pour plus d'informations, reportez vous à [Procédure : proposer des paiements fournisseur](payables-how-suggest-vendor-payments.md).</span><span class="sxs-lookup"><span data-stu-id="c8f1d-104">for more information, see [How to: Suggest Vendor Payments](payables-how-suggest-vendor-payments.md).</span></span>

<span data-ttu-id="c8f1d-105">Tout d'abord, vous devez attribuer une priorité à vos fournisseurs en leur affectant des numéros.</span><span class="sxs-lookup"><span data-stu-id="c8f1d-105">First, you must prioritize your vendors by assigning numbers to them.</span></span>

## <a name="to-prioritize-vendors"></a><span data-ttu-id="c8f1d-106">Pour octroyer une priorité à des fournisseurs</span><span class="sxs-lookup"><span data-stu-id="c8f1d-106">To prioritize vendors</span></span>
1. <span data-ttu-id="c8f1d-107">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Fournisseurs**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="c8f1d-107">In the top right corner, choose the **Search for Page or Report** icon, enter **Vendors**, and then choose the related link.</span></span>
2. <span data-ttu-id="c8f1d-108">Sélectionnez le fournisseur approprié, puis sélectionnez **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="c8f1d-108">Select the relevant vendor, and then choose **Edit**.</span></span>
3. <span data-ttu-id="c8f1d-109">Dans le champ **Priorité**, entrez un numéro.</span><span class="sxs-lookup"><span data-stu-id="c8f1d-109">In the **Priority** field, enter a number.</span></span>

<span data-ttu-id="c8f1d-110">Dynamics NAV donne le degré de priorité le plus élevé au chiffre le plus bas (excepté 0).</span><span class="sxs-lookup"><span data-stu-id="c8f1d-110">Dynamics NAV considers the lowest number, except 0, to have the highest priority.</span></span> <span data-ttu-id="c8f1d-111">Ainsi, si vous utilisez 1, 2 et 3, le chiffre 1 a le degré de priorité le plus élevé.</span><span class="sxs-lookup"><span data-stu-id="c8f1d-111">So, for example, if you use 1, 2, and 3, then 1 will have the highest priority.</span></span>

<span data-ttu-id="c8f1d-112">Si vous ne souhaitez pas attribuer de priorité à un fournisseur, laissez le champ **Priorité** blanc.</span><span class="sxs-lookup"><span data-stu-id="c8f1d-112">If you do not want to prioritize a vendor, leave the **Priority** field blank.</span></span> <span data-ttu-id="c8f1d-113">Par la suite, lorsque vous utilisez la fonction de proposition de paiements, ce fournisseur est répertorié après tous les fournisseurs possédant un numéro prioritaire.</span><span class="sxs-lookup"><span data-stu-id="c8f1d-113">Then, if you use the payment suggestion feature, the vendor will be listed after all the vendors that have a priority number.</span></span> <span data-ttu-id="c8f1d-114">Vous pouvez saisir autant de niveaux de priorité que nécessaire.</span><span class="sxs-lookup"><span data-stu-id="c8f1d-114">You can enter as many priority levels as necessary.</span></span>

## <a name="see-also"></a><span data-ttu-id="c8f1d-115">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c8f1d-115">See Also</span></span>
[<span data-ttu-id="c8f1d-116">Configuration des procédures achat</span><span class="sxs-lookup"><span data-stu-id="c8f1d-116">Set Up Purchasing</span></span>](purchasing-setup-purchasing.md)  
[<span data-ttu-id="c8f1d-117">Gestion des comptes fournisseur</span><span class="sxs-lookup"><span data-stu-id="c8f1d-117">Manage Payables</span></span>](payables-manage-payables.md)

