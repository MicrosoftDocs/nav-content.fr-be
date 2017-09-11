---
title: "Saisir les critères pour les filtres"
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: df386e1195db385ee053b69fec0f5082d8df4116
ms.contentlocale: fr-be
ms.lasthandoff: 07/19/2017

---

# <a name="entering-criteria-in-filters"></a><span data-ttu-id="a0ca7-102">Saisir les critères pour les filtres</span><span class="sxs-lookup"><span data-stu-id="a0ca7-102">Entering Criteria in Filters</span></span>
<span data-ttu-id="a0ca7-103">Lorsque vous souhaitez rechercher des données, telles que des noms de client, des adresses ou des groupes de produits, vous saisissez des critères.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-103">When you want to search for data, such as customer names, addresses, or product groups, you enter criteria.</span></span> <span data-ttu-id="a0ca7-104">Dans vos critères de recherche, vous pouvez utiliser tous les chiffres et toutes les lettres que vous utilisez habituellement dans ce champ spécifique.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-104">In search criteria you can use all the numbers and letters that you normally use in the specific field.</span></span> <span data-ttu-id="a0ca7-105">En plus, vous pouvez utiliser des symboles spéciaux pour filtrer davantage les résultats.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-105">In addition, you can use special symbols to further filter the results.</span></span>

## <a name="searching-using-the-quick-filter"></a><span data-ttu-id="a0ca7-106">Rechercher à l'aide du filtre rapide</span><span class="sxs-lookup"><span data-stu-id="a0ca7-106">Searching using the Quick Filter</span></span>
<span data-ttu-id="a0ca7-107">Vous pouvez ajouter des filtres pour l'ensemble des pages en utilisant le filtre rapide.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-107">You can add filters to all pages by using the Quick Filter.</span></span> <span data-ttu-id="a0ca7-108">Vous activez le filtre rapide sélectionnant l'icône de loupe dans le coin supérieur droit d'une page.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-108">The Quick Filter is enabled by choosing the magnifier icon in the top right corner of a page.</span></span> <span data-ttu-id="a0ca7-109">Ce type de filtre est utilisé pour une saisie rapide des critères.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-109">This filtering type is used for a fast entry of criteria.</span></span>

<span data-ttu-id="a0ca7-110">**Important** : le filtre rapide facilite l'accès aux données de filtre par la saisie de texte simple, mais fournit également un grand nombre d'options de critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-110">**Important**: The Quick Filter provides an easy access to filter data by entering plain text, but does also provide a lot of search criteria options.</span></span> <span data-ttu-id="a0ca7-111">Selon que vous saisissez du texte simple ou du texte comprenant des symboles, le Filtre rapide se comporte de façon différente.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-111">Depending on whether you enter plain text or text including symbols, the Quick Filter behaves differently.</span></span>  
- <span data-ttu-id="a0ca7-112">Si vous saisissez du texte simple dans les critères de recherche, le critère de recherche est interprété comme une recherche insensible à la casse qui contient un certain texte.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-112">If you enter plain text in the search criteria, the search criteria is interpreted as a case insensitive search that contains certain text.</span></span>  
- <span data-ttu-id="a0ca7-113">Si vous saisissez du texte comprenant des symboles dans les critères de recherche, le critère de recherche est interprété exactement comme vous l'avez saisi, et la recherche distingue les majuscules et les minuscules.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-113">If you enter text including symbols in the search criteria, the search criteria is interpreted exactly as you entered it, and the search is case sensitive.</span></span>

### <a name="quick-filter-criteria"></a><span data-ttu-id="a0ca7-114">Critères de filtre rapide</span><span class="sxs-lookup"><span data-stu-id="a0ca7-114">Quick filter criteria</span></span>
<!-- html syntax because symbols conflict with MarkDown syntax -->
<TABLE>
  <TR>
    <TH><span data-ttu-id="a0ca7-115">Critères de recherche</span><span class="sxs-lookup"><span data-stu-id="a0ca7-115">Search Criteria</span></span></TH>
    <TH><span data-ttu-id="a0ca7-116">Interprété comme...</span><span class="sxs-lookup"><span data-stu-id="a0ca7-116">Interpreted as...</span></span></TH>
    <TH><span data-ttu-id="a0ca7-117">Renvoie...</span><span class="sxs-lookup"><span data-stu-id="a0ca7-117">Returns...</span></span></TH>
  </TR>
  <TR>
    <TD><span data-ttu-id="a0ca7-118">>man</span><span class="sxs-lookup"><span data-stu-id="a0ca7-118">>man</span></span></TD>
    <TD><span data-ttu-id="a0ca7-119">@*man*</span><span class="sxs-lookup"><span data-stu-id="a0ca7-119">@*man*</span></span></TD>
    <TD><span data-ttu-id="a0ca7-120">Tous les enregistrements qui contiennent le texte man et ne respectent pas la casse.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-120">All records that contain the text man and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="a0ca7-121">>se</span><span class="sxs-lookup"><span data-stu-id="a0ca7-121">>se</span></span></TD>
    <TD><span data-ttu-id="a0ca7-122">@*se*</span><span class="sxs-lookup"><span data-stu-id="a0ca7-122">@*se*</span></span></TD>
    <TD><span data-ttu-id="a0ca7-123">Tous les enregistrements qui contiennent le texte se et ne respectent pas la casse.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-123">All records that contain the text se and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="a0ca7-124">>Man*</span><span class="sxs-lookup"><span data-stu-id="a0ca7-124">>Man*</span></span></TD>
    <TD><span data-ttu-id="a0ca7-125">Commence par Man avec respect de la casse.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-125">Starts with Man and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="a0ca7-126">Tous les enregistrements qui commencent par le texte Man.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-126">All records that start with the text Man.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="a0ca7-127">'man'</span><span class="sxs-lookup"><span data-stu-id="a0ca7-127">'man'</span></span></TD>
    <TD><span data-ttu-id="a0ca7-128">Texte exact avec respect de la casse.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-128">An exact text and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="a0ca7-129">Tous les enregistrements qui correspondent exactement à man.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-129">All records that match man exactly.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="a0ca7-130">@*man</span><span class="sxs-lookup"><span data-stu-id="a0ca7-130">@*man</span></span></TD>
    <TD><span data-ttu-id="a0ca7-131">Se termine par et respecte la casse.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-131">Ends with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="a0ca7-132">Tous les enregistrements qui se terminent par man.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-132">All records that end with man.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="a0ca7-133">@man*</span><span class="sxs-lookup"><span data-stu-id="a0ca7-133">@man*</span></span></TD>
    <TD><span data-ttu-id="a0ca7-134">Commence par et ne respecte pas la casse.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-134">Starts with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="a0ca7-135">Tous les enregistrements qui commencent par man.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-135">All records that start with man.</span></span></TD>
  </TR>
</TABLE>

<span data-ttu-id="a0ca7-136">**Remarque**: vous ne pouvez pas utiliser de caractères génériques lors du filtrage des champs d'énumération, tels que le champ **Statut** sur les commandes vente.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-136">**Note**: You cannot use a wildcard when filtering on enumeration fields, such as the **Status** field on sales orders.</span></span> <span data-ttu-id="a0ca7-137">Pour entrer un filtre pour ce type de champ, vous pouvez saisir la valeur numérique comme paramètre de filtre.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-137">To enter a filter for this type of field, you can enter the numeric value as a filtering parameter.</span></span> <span data-ttu-id="a0ca7-138">Par exemple, dans le champ **Statut** sur une commande vente qui a les valeurs **Ouvert**, **Lancé**, **Approbation suspendue** et **Acompte suspendu**, utilisez les valeurs **0**, **1**, **2** et **3** pour filtrer ces options.</span><span class="sxs-lookup"><span data-stu-id="a0ca7-138">For example, in the **Status** field on a sales order that has the values **Open**, **Released**, **Pending Approval**, and **Pending Prepayment**, use the values **0**, **1**, **2**, and **3** to filter for these options.</span></span>  

## <a name="see-also"></a><span data-ttu-id="a0ca7-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a0ca7-139">See Also</span></span>
[<span data-ttu-id="a0ca7-140">Utiliser Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="a0ca7-140">Work with Dynamics NAV</span></span>](ui-work-product.md)

