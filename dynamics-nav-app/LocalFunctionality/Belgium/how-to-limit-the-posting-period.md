---
title: "Comment limiter la période de validation"
description: "Vous pouvez limiter la période au cours de laquelle la validation est autorisée selon trois niveaux différents : **par société**, **par utilisateur** et **par modèle**."
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
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 0fd8eca40a1b057458dac369931f7f4a39c832d4
ms.contentlocale: fr-be
ms.lasthandoff: 10/26/2017

---
# <a name="how-to-limit-the-posting-period"></a><span data-ttu-id="bd312-103">Comment limiter la période de validation</span><span class="sxs-lookup"><span data-stu-id="bd312-103">How to: Limit the Posting Period</span></span>
<span data-ttu-id="bd312-104">Dans [!INCLUDE[navnow](../../includes/navnow_md.md)], vous pouvez limiter la période au cours de laquelle la validation est autorisée selon trois niveaux différents : **par société**, **par utilisateur** et **par modèle**.</span><span class="sxs-lookup"><span data-stu-id="bd312-104">In [!INCLUDE[navnow](../../includes/navnow_md.md)], you can limit the period by which posting is permitted on three different levels: **by company**, **by user**, and **by template**.</span></span>  

<span data-ttu-id="bd312-105">Il peut être utile de limiter les périodes de validation lorsqu'une société clôture sa feuille vente à la fin de chaque mois.</span><span class="sxs-lookup"><span data-stu-id="bd312-105">Limiting posting periods can be useful when a company closes its sales journal at the end of each month.</span></span> <span data-ttu-id="bd312-106">Cela empêche les vendeurs d'enregistrer des documents vente du mois précédent.</span><span class="sxs-lookup"><span data-stu-id="bd312-106">This keeps salespeople from registering sales documents from the previous month.</span></span> <span data-ttu-id="bd312-107">Dans le même temps, la feuille achat peut rester ouverte pour enregistrer les factures achat entrantes du mois précédent.</span><span class="sxs-lookup"><span data-stu-id="bd312-107">At the same time, the purchase journal may stay open to register incoming purchase invoices from the previous month.</span></span>  

<span data-ttu-id="bd312-108">Lorsque vous effectuez une validation dans la fenêtre **Modèles feuille comptabilité**, le contenu des champs **Début période validation** et **Fin période validation** est vérifié pour obtenir un intervalle de dates.</span><span class="sxs-lookup"><span data-stu-id="bd312-108">When you post in the **General Journal Templates** window, the contents of the **Allow Posting From** field and **Allow Posting To** field are checked for a date interval.</span></span> <span data-ttu-id="bd312-109">L'intervalle de date indique à quel moment vous pouvez valider sur un modèle feuille.</span><span class="sxs-lookup"><span data-stu-id="bd312-109">The date interval indicates when you can post to a journal template.</span></span> <span data-ttu-id="bd312-110">Si le champ est vide, la fenêtre **Paramètres utilisateur** est vérifiée pour obtenir un intervalle de dates pour l'utilisateur actuel.</span><span class="sxs-lookup"><span data-stu-id="bd312-110">If the field is blank, the **User Setup** window is checked for a date interval for the current user.</span></span> <span data-ttu-id="bd312-111">Si la fenêtre **Paramètres utilisateur** ne contient pas d'intervalle, les champs **Début période validation** et **Fin période validation** dans la fenêtre **Paramètres comptabilité** sont vérifiés pour obtenir un intervalle de dates au niveau de la société.</span><span class="sxs-lookup"><span data-stu-id="bd312-111">If the **User Setup** window does not contain an interval, the **Allow Posting From** field and the **Allow Posting To** field in the **General Ledger Setup** window is checked for a date interval at the company level.</span></span>  

## <a name="to-limit-the-posting-periods-by-company"></a><span data-ttu-id="bd312-112">Pour limiter les périodes de validation par société</span><span class="sxs-lookup"><span data-stu-id="bd312-112">To limit the posting periods by company</span></span>  

1.  <span data-ttu-id="bd312-113">Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Paramètres comptabilité**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="bd312-113">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="bd312-114">Pour spécifier le début de la période, choisissez le champ **Début période validation**, puis entrez la première date à laquelle la validation sur la société est autorisée.</span><span class="sxs-lookup"><span data-stu-id="bd312-114">To specify the start of the period, choose the **Allow Posting From** field, and then enter the earliest date on which posting to the company is enabled.</span></span>  
3.  <span data-ttu-id="bd312-115">Pour spécifier la fin de la période, choisissez le champ **Fin période validation**, puis entrez la dernière date à laquelle la validation sur la société est autorisée.</span><span class="sxs-lookup"><span data-stu-id="bd312-115">To specify the end of the period, choose the **Allow Posting To** field, and then enter the last date on which posting to the company is enabled.</span></span>  

## <a name="to-limit-the-posting-periods-by-user"></a><span data-ttu-id="bd312-116">Pour limiter les périodes de validation par utilisateur</span><span class="sxs-lookup"><span data-stu-id="bd312-116">To limit the posting periods by user</span></span>  

1.  <span data-ttu-id="bd312-117">Choisissiez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Paramètres utilisateur**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="bd312-117">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **User Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="bd312-118">Pour spécifier le début de la période, choisissez le champ **Début période validation**, puis entrez la première date à laquelle l'utilisateur peut effectuer la validation sur la société.</span><span class="sxs-lookup"><span data-stu-id="bd312-118">To specify the start of the period, choose the **Allow Posting From** field, and then enter the earliest date on which the user can post to the company.</span></span>  
3.  <span data-ttu-id="bd312-119">Pour spécifier la fin de la période, choisissez le champ **Fin période validation**, puis entrez la dernière date à laquelle l'utilisateur peut effectuer la validation sur la société.</span><span class="sxs-lookup"><span data-stu-id="bd312-119">To specify the end of the period, choose the **Allow Posting To** field, and then enter the last date the user will be able to post to the company.</span></span>  

## <a name="to-limit-the-posting-periods-by-template"></a><span data-ttu-id="bd312-120">Pour limiter les périodes de validation par modèle</span><span class="sxs-lookup"><span data-stu-id="bd312-120">To limit the posting periods by template</span></span>  

1.  <span data-ttu-id="bd312-121">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Modèles feuille comptabilité**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="bd312-121">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journal Templates**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="bd312-122">Pour spécifier le début de la période, choisissez le champ **Début période validation**, puis entrez la première date à laquelle l'utilisateur peut effectuer la validation sur la société.</span><span class="sxs-lookup"><span data-stu-id="bd312-122">To specify the start of the period, choose the **Allow Posting From** field, and then enter the earliest date on which the user can post to the company.</span></span>  
3.  <span data-ttu-id="bd312-123">Pour spécifier la fin de la période, choisissez le champ **Fin période validation**, puis entrez la dernière date à laquelle l'utilisateur peut effectuer la validation sur la société.</span><span class="sxs-lookup"><span data-stu-id="bd312-123">To specify the end of the period, choose the **Allow Posting To** field, and then enter the last date the user will be able to post to the company.</span></span>  

## <a name="see-also"></a><span data-ttu-id="bd312-124">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bd312-124">See Also</span></span>  
 <span data-ttu-id="bd312-125">[Fonctionnalité locale pour la Belgique](belgium-local-functionality.md) </span><span class="sxs-lookup"><span data-stu-id="bd312-125">[Belgium Local Functionality](belgium-local-functionality.md) </span></span>  
 [<span data-ttu-id="bd312-126">Comment spécifier des périodes de validation</span><span class="sxs-lookup"><span data-stu-id="bd312-126">How to: Specify Posting Periods</span></span>](../France/how-to-specify-posting-periods.md)

