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
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 8eab393a0a77f9f1595ca1247c7549e68b491cb2
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="entering-criteria-in-filters"></a>Saisir les critères pour les filtres
Lorsque vous souhaitez rechercher des données, telles que des noms de client, des adresses ou des groupes de produits, vous saisissez des critères. Dans vos critères de recherche, vous pouvez utiliser tous les chiffres et toutes les lettres que vous utilisez habituellement dans ce champ spécifique. En plus, vous pouvez utiliser des symboles spéciaux pour filtrer davantage les résultats.

## <a name="searching-using-the-quick-filter"></a>Rechercher à l'aide du filtre rapide
Vous pouvez ajouter des filtres pour l'ensemble des pages en utilisant le filtre rapide. Vous activez le filtre rapide sélectionnant l'icône de loupe dans le coin supérieur droit d'une page. Ce type de filtre est utilisé pour une saisie rapide des critères.

**Important** : le filtre rapide facilite l'accès aux données de filtre par la saisie de texte simple, mais fournit également un grand nombre d'options de critères de recherche. Selon que vous saisissez du texte simple ou du texte comprenant des symboles, le Filtre rapide se comporte de façon différente.  
- Si vous saisissez du texte simple dans les critères de recherche, le critère de recherche est interprété comme une recherche insensible à la casse qui contient un certain texte.  
- Si vous saisissez du texte comprenant des symboles dans les critères de recherche, le critère de recherche est interprété exactement comme vous l'avez saisi, et la recherche distingue les majuscules et les minuscules.

### <a name="quick-filter-criteria"></a>Critères de filtre rapide
<!-- html syntax because symbols conflict with MarkDown syntax -->
<TABLE>
  <TR>
    <TH>Critères de recherche</TH>
    <TH>Interprété comme...</TH>
    <TH>Renvoie...</TH>
  </TR>
  <TR>
    <TD>>man</TD>
    <TD>@*man*</TD>
    <TD>Tous les enregistrements qui contiennent le texte man et ne respectent pas la casse.</TD>
  </TR>
  <TR>
    <TD>>se</TD>
    <TD>@*se*</TD>
    <TD>Tous les enregistrements qui contiennent le texte se et ne respectent pas la casse.</TD>
  </TR>
  <TR>
    <TD>>Man*</TD>
    <TD>Commence par Man avec respect de la casse.</TD>
    <TD>Tous les enregistrements qui commencent par le texte Man.</TD>
  </TR>
  <TR>
    <TD>'man'</TD>
    <TD>Texte exact avec respect de la casse.</TD>
    <TD>Tous les enregistrements qui correspondent exactement à man.</TD>
  </TR>
  <TR>
    <TD>@*man</TD>
    <TD>Se termine par et respecte la casse.</TD>
    <TD>Tous les enregistrements qui se terminent par man.</TD>
  </TR>
  <TR>
    <TD>@man*</TD>
    <TD>Commence par et ne respecte pas la casse.</TD>
    <TD>Tous les enregistrements qui commencent par man.</TD>
  </TR>
</TABLE>

**Remarque**: vous ne pouvez pas utiliser de caractères génériques lors du filtrage des champs d'énumération, tels que le champ **Statut** sur les commandes vente. Pour entrer un filtre pour ce type de champ, vous pouvez saisir la valeur numérique comme paramètre de filtre. Par exemple, dans le champ **Statut** sur une commande vente qui a les valeurs **Ouvert**, **Lancé**, **Approbation suspendue** et **Acompte suspendu**, utilisez les valeurs **0**, **1**, **2** et **3** pour filtrer ces options.  

## <a name="see-also"></a>Voir aussi
[Utiliser Dynamics NAV](ui-work-product.md)

